---
swagger: "2.0"
x-collection-name: RingCentral
x-complete: 0
info:
  title: RingCentral Create SMS Message
  description: "Creates and sends new SMS message. Sending SMS messages simultaneously
    to different recipients is limited up to 50 requests per minute; relevant for
    all client applications.\nApp Permission\nSMS\nUser Permission\nOutboundSMS\nUsage
    Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
    Message\n   \n \n\n400\nCMN-101\nParameter [] value is invalid\n\n\n400\nCMN-406\nDuplicate
    value for parameter to: +13476733173 found in request\n\n\n400\nMSG-243\nParameter
    [to] value [18882049692] is invalid [Phone number is blocked]\n\n\n400\nMSG-245\nParameter
    [from] value [88121002330] is invalid [Cannot find the phone number which belongs
    to user]\n\n\n400\nMSG-246\nSending SMS from/to extension numbers is not available\n\n\n400\nMSG-247\nSending
    SMS to short numbers is not available\n\n\n400\nMSG-365\nParameters [country.id]
    and [country.isoCode] can not be specified simultaneously\n\n\n400\nMSG-376\nAttachment
    size limit exceeded\n\n\n400\nMSG-379\nToo many attachments\n\n\n400\nMSG-381\nExceeded
    maximum number of recipients for a Group MMS: [10]\n\n\n403\nBIL-103\nFeature
    [MMS] is not available for current account\n\n\n403\nCMN-401\nIn order to call
    this API endpoint, application needs to have [SMS] permission\n\n\n403\nCMN-408\nIn
    order to call this API endpoint, user needs to have [OutboundSMS] permission for
    requested resource.\n\n\n403\nMSG-240\nInternational SMS is not available for
    account.\n\n\n403\nMSG-241\nCannot send SMS from Fax number\n\n\n403\nMSG-242\nThe
    requested feature is not available\n\n\n403\nMSG-314\nExtension is of inappropriate
    type\n\n\n403\nMSG-367\n\"from\" phone number does not support SMS\n\n\n403\nMSG-383\nInternational
    MMS feature is not available\n\n\n403\nMSG-384\nAccount limits exceeded. Cannot
    send the message.\n\n\n403\nMSG-388\nThe destination is prohibited\n\n\n404\nCMN-102\nResource
    for parameter [accountId] is not found\n\n\n415\nMSG-348\nUnsupported attachment
    media type, attachment [3]: [stuff.smil]"
  version: 1.0.0
host: platform.ringcentral.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /restapi/:
    get:
      summary: Get API Versions
      description: |-
        Returns current API version(s) and server info.
        Usage Plan Group
        NoThrottling
      operationId: getAllVersions
      x-api-path-slug: restapi-get
      responses:
        200:
          description: OK
      tags:
      - Versions
  /restapi/{apiVersion}:
    get:
      summary: Get Version Info
      description: |-
        Returns current API version info by apiVersion.
        Usage Plan Group
        NoThrottling
      operationId: getApiVersion
      x-api-path-slug: restapiapiversion-get
      parameters:
      - in: path
        name: apiVersion
        description: API version to be requested, for example v1
      responses:
        200:
          description: OK
      tags:
      - Version
      - Info
  /restapi/v1.0/status:
    get:
      summary: Get Service status
      description: |-
        Returns current PAS service status.
        Usage Plan Group
        NoThrottling
      operationId: loadAPIStatus
      x-api-path-slug: restapiv1-0status-get
      responses:
        200:
          description: OK
      tags:
      - Service
      - Status
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/call-log:
    get:
      summary: Get Call Log Records by Filter
      description: "Returns call log records filtered by parameters specified.\nApp
        Permission\nReadCallLog\nUser Permission\nReadCallLog\nUsage Plan Group\nHeavy\nError
        Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCLG-110\nParameter
        [sessionId] is not allowed for usage along with parameter [extensionNumber]\n\n\n400\nCMN-101\nParameter
        [transport] value is invalid\n\n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-129\nAccess
        token corrupted\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n401\nOAU-213\nToken
        not found\n\n\n403\nCMN-401\nIn order to call this API endpoint, application
        needs to have [ReadCallLog] permission\n\n\n403\nCMN-408\nIn order to call
        this API endpoint, user needs to have [ReadCallLog] permission for requested
        resource.\n\n\n404\nCMN-102\nResource for parameter [extensionId] is not found\n\n\n429\nCMN-301\nRequest
        rate exceeded"
      operationId: loadExtensionCallLog
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidcalllog-get
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: query
        name: dateFrom
        description: The start datetime for resulting records in ISO 8601 format including
          timezone, for example 2016-03-10T18:07:52
      - in: query
        name: dateTo
        description: The end datetime for resulting records in ISO 8601 format including
          timezone, for example 2016-03-10T18:07:52
      - in: query
        name: direction
        description: The direction for the resulting records
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      - in: query
        name: extensionNumber
        description: Extension number of a user
      - in: query
        name: page
        description: Indicates the page number to retrieve
      - in: query
        name: perPage
        description: Indicates the page size (number of items)
      - in: query
        name: phoneNumber
        description: Phone number of a caller/callee
      - in: query
        name: sessionId
      - in: query
        name: showBlocked
        description: If True then calls from/to blocked numbers are returned
      - in: query
        name: transport
        description: Call transport type
      - in: query
        name: type
        description: Call type of a record
      - in: query
        name: view
        description: The default value is Simple for both account and extension call
          log
      - in: query
        name: withRecording
        description: True should be specified to return recorded calls only
      responses:
        200:
          description: OK
      tags:
      - Call
      - Log
      - Records
      - By
      - Filter
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/call-log/{callRecordId}:
    get:
      summary: Get Call Records by ID
      description: "Returns filtered call log records.\nApp Permission\nReadCallLog\nUser
        Permission\nReadCallLog\nUsage Plan Group\nHeavy\nError Codes\n\n \n  \n   HTTP
        Code\n   Error Code\n   Error Message\n   \n \n\n403\nCMN-401\nIn order to
        call this API endpoint, application needs to have [ReadCallLog] permission\n\n\n403\nCMN-408\nIn
        order to call this API endpoint, user needs to have [ReadCallLog] permission
        for requested resource.\n\n\n404\nCMN-102\nResource for parameter [extensionId]
        is not found"
      operationId: getCallRecords
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidcalllogcallrecordid-get
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: path
        name: callRecordId
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      - in: query
        name: view
      responses:
        200:
          description: OK
      tags:
      - Call
      - Records
      - By
      - ID
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/active-calls:
    get:
      summary: Get User Active Calls
      description: "Returns records of all extension calls that are in progress, ordered
        by start time in descending order.\nApp Permission\nReadCallLog\nUser Permission\nReadCallLog\nUsage
        Plan Group\nHeavy\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n400\nCMN-101\nParameter [direction] value is invalid\n\n\n401\nCMN-405\nLogin
        to extension required\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n403\nCMN-401\nIn
        order to call this API endpoint, application needs to have [ReadCallLog] permission\n\n\n403\nCMN-408\nIn
        order to call this API endpoint, user needs to have [ReadCallLog] permission
        for requested resource.\n\n\n404\nCMN-102\nResource for parameter [accountId]
        is not found"
      operationId: listExtensionActiveCalls
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidactivecalls-get
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: query
        name: direction
        description: The direction for the result records
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      - in: query
        name: page
        description: Indicates the page number to retrieve
      - in: query
        name: perPage
        description: Indicates the page size (number of items)
      - in: query
        name: type
        description: Call type of a record
      responses:
        200:
          description: OK
      tags:
      - User
      - Active
      - Calls
  /restapi/v1.0/account/{accountId}/call-log:
    get:
      summary: Get Call Log Records by Filter
      description: "Returns call log records filtered by parameters specified.\nApp
        Permission\nReadCallLog\nUser Permission\nFullCompanyCallLog\nUsage Plan Group\nHeavy\nError
        Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCLG-110\nParameter
        [sessionId] is not allowed for usage along with parameter [extensionNumber]\n\n\n400\nCMN-101\nParameter
        [dateFrom] value is invalid\n\n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-151\nAuthorization
        method not supported\n\n\n403\nCMN-401\nIn order to call this API endpoint,
        application needs to have [ReadCallLog] permission\n\n\n403\nCMN-408\nIn order
        to call this API endpoint, user needs to have [ReadCompanyCallLog] permission
        for requested resource.\n\n\n404\nCMN-102\nResource for parameter [accountId]
        is not found"
      operationId: loadAccountCallLog
      x-api-path-slug: restapiv1-0accountaccountidcalllog-get
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: query
        name: dateFrom
        description: The start datetime for resulting records in ISO 8601 format including
          timezone, for example 2016-03-10T18:07:52
      - in: query
        name: dateTo
        description: The end datetime for resulting records in ISO 8601 format including
          timezone, for example 2016-03-10T18:07:52
      - in: query
        name: direction
        description: The direction for the result records
      - in: query
        name: extensionNumber
        description: Extension number of a user
      - in: query
        name: page
        description: Indicates the page number to retrieve
      - in: query
        name: perPage
        description: Indicates the page size (number of items)
      - in: query
        name: phoneNumber
        description: Phone number of a caller/call recipient
      - in: query
        name: sessionId
      - in: query
        name: type
        description: Call type of a record
      - in: query
        name: view
        description: The default value is Simple for both account and extension call
          log
      - in: query
        name: withRecording
        description: True if only recorded calls have to be returned
      responses:
        200:
          description: OK
      tags:
      - Call
      - Log
      - Records
      - By
      - Filter
  /restapi/v1.0/account/{accountId}/recording/{recordingId}:
    get:
      summary: Get Call Recordings
      description: "Returns call recording metadata by ID.\nApp Permission\nReadCallRecording\nUser
        Permission\nReadCallRecording\nUsage Plan Group\nHeavy\nError Codes\n\n \n
        \ \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n401\nCMN-405\nLogin
        to extension required\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n403\nCMN-401\nIn
        order to call this API endpoint, application needs to have [ReadCallRecording]
        permission\n\n\n404\nCMN-102\nResource for parameter [accountId] is not found"
      operationId: listCallRecordings
      x-api-path-slug: restapiv1-0accountaccountidrecordingrecordingid-get
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: path
        name: recordingId
        description: Internal identifier of a recording (returned in Call Log)
      responses:
        200:
          description: OK
      tags:
      - Call
      - Recordings
  /restapi/v1.0/account/{accountId}/recording/{recordingId}/content:
    get:
      summary: Get Call Recordings Data
      description: "Returns media content of a call recording.\nApp Permission\nReadCallRecording\nUser
        Permission\nReadCallRecording\nUsage Plan Group\nHeavy\nError Codes\n\n \n
        \ \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n401\nAGW-402\nInvalid
        Authorization header\n\n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-149\nUnparsable
        access token\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n403\nCMN-401\nIn
        order to call this API endpoint, application needs to have [ReadCallRecording]
        permission\n\n\n404\nCMN-102\nResource for parameter [accountId] is not found\n\n\n416\nCMN-107\nRequested
        range not satisfiable"
      operationId: listCallRecordingData
      x-api-path-slug: restapiv1-0accountaccountidrecordingrecordingidcontent-get
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: path
        name: recordingId
        description: Internal identifier of a recording (returned in Call Log)
      responses:
        200:
          description: OK
      tags:
      - Call
      - Recordings
      - Data
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/sms:
    post:
      summary: Create SMS Message
      description: "Creates and sends new SMS message. Sending SMS messages simultaneously
        to different recipients is limited up to 50 requests per minute; relevant
        for all client applications.\nApp Permission\nSMS\nUser Permission\nOutboundSMS\nUsage
        Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n400\nCMN-101\nParameter [] value is invalid\n\n\n400\nCMN-406\nDuplicate
        value for parameter to: +13476733173 found in request\n\n\n400\nMSG-243\nParameter
        [to] value [18882049692] is invalid [Phone number is blocked]\n\n\n400\nMSG-245\nParameter
        [from] value [88121002330] is invalid [Cannot find the phone number which
        belongs to user]\n\n\n400\nMSG-246\nSending SMS from/to extension numbers
        is not available\n\n\n400\nMSG-247\nSending SMS to short numbers is not available\n\n\n400\nMSG-365\nParameters
        [country.id] and [country.isoCode] can not be specified simultaneously\n\n\n400\nMSG-376\nAttachment
        size limit exceeded\n\n\n400\nMSG-379\nToo many attachments\n\n\n400\nMSG-381\nExceeded
        maximum number of recipients for a Group MMS: [10]\n\n\n403\nBIL-103\nFeature
        [MMS] is not available for current account\n\n\n403\nCMN-401\nIn order to
        call this API endpoint, application needs to have [SMS] permission\n\n\n403\nCMN-408\nIn
        order to call this API endpoint, user needs to have [OutboundSMS] permission
        for requested resource.\n\n\n403\nMSG-240\nInternational SMS is not available
        for account.\n\n\n403\nMSG-241\nCannot send SMS from Fax number\n\n\n403\nMSG-242\nThe
        requested feature is not available\n\n\n403\nMSG-314\nExtension is of inappropriate
        type\n\n\n403\nMSG-367\n\"from\" phone number does not support SMS\n\n\n403\nMSG-383\nInternational
        MMS feature is not available\n\n\n403\nMSG-384\nAccount limits exceeded. Cannot
        send the message.\n\n\n403\nMSG-388\nThe destination is prohibited\n\n\n404\nCMN-102\nResource
        for parameter [accountId] is not found\n\n\n415\nMSG-348\nUnsupported attachment
        media type, attachment [3]: [stuff.smil]"
      operationId: sendSMS
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidsms-post
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: body
        name: body
        description: JSON body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      responses:
        200:
          description: OK
      tags:
      - SMS
      - Message
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---