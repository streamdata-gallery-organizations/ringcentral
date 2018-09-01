---
swagger: "2.0"
x-collection-name: RingCentral
x-complete: 0
info:
  title: RingCentral Create User Custom Greeting
  description: "Creates custom greeting for an extension user.\nApp Permission\nEditExtensions\nUser
    Permission\nEditUserAnsweringRules\nUsage Plan Group\nHeavy\nError Codes\n\n \n
    \ \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nAWR-128\nAttachment
    body is empty\n\n\n400\nAWR-129\nInvalid attachment media type\n\n\n400\nAWR-165\nHold
    music can be set for business hours rule only: the same value will be applied
    to all rules\n\n\n400\nCLR-103\nCompany level greeting cannot be created on user
    level.\n\n\n400\nCMN-101\nParameter [type] value is invalid\n\n\n400\nCMN-102\nResource
    for parameter [answeringRule.id] is not found\n\n\n400\nCMN-111\nBusiness operation
    is not supported"
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
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/company-pager:
    post:
      summary: Create Pager Message
      description: "Creates and sends a pager message.\nApp Permission\nInternalMessages\nUser
        Permission\nInternalSMS\nUsage Plan Group\nMedium\nError Codes\n\n \n  \n
        \  HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
        [to.phoneNumber] value is invalid\n\n\n400\nCMN-102\nResource for parameter
        [to] is not found\n\n\n400\nMSG-316\nParameter [to] value [102] is invalid
        [Target extension not found]\n\n\n400\nMSG-324\nExtension is of unappropriate
        state\n\n\n400\nMSG-331\nParameter [from] value [11111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111]
        is invalid [Sender extension number does not correspond to logged in extension]\n\n\n400\nMSG-332\nParameter
        [from] value [404544780008] is invalid [Sender extension id does not correspond
        to logged in extension]\n\n\n400\nMSG-335\nRecipient extension number does
        not correspond to ID\n\n\n403\nCMN-401\nIn order to call this API endpoint,
        application needs to have [InternalMessages] permission\n\n\n403\nCMN-408\nIn
        order to call this API endpoint, user needs to have [InternalSMS] permission
        for requested resource.\n\n\n403\nMSG-325\nReply is forbidden for old message
        threads\n\n\n403\nMSG-326\nReply is denied for user, who is no longer a thread
        participant\n\n\n403\nMSG-330\nSender extension is of unappropriate type\n\n\n404\nCMN-102\nResource
        for parameter [extensionId] is not found"
      operationId: sendInternalMessage
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidcompanypager-post
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
      - Pager
      - Message
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/fax:
    post:
      summary: Create Fax Message
      description: "Creates and sends/resends new fax message. Resend can be done
        if sending failed.\nApp Permission\nFaxes\nUser Permission\nOutboundFaxes\nUsage
        Plan Group\nHeavy\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n400\nCMN-101\nParameter [to] value is invalid\n\n\n400\nMSG-344\nSending
        fax to extension numbers is not available\n\n\n400\nMSG-347\nAttachment [t.txt]
        body is empty\n\n\n400\nMSG-355\nFor binary data filename with extension should
        be specified, attachment [1]: []\n\n\n400\nMSG-356\nEither filename or content
        type should be specified, attachment [1]: []\n\n\n400\nMSG-365\nParameters
        [country.id] and [country.isoCode] can not be specified simultaneously\n\n\n400\nMSG-370\nfilename
        is too long, 256 characters allowed\n\n\n403\nCMN-401\nIn order to call this
        API endpoint, application needs to have [Faxes] permission\n\n\n403\nCMN-408\nIn
        order to call this API endpoint, user needs to have [OutboundFaxes] permission
        for requested resource.\n\n\n404\nCMN-102\nResource for parameter [extensionId]
        is not found\n\n\n415\nMSG-348\nUnsupported attachment media type, attachment
        [1]: [.jfif]\n\n\n415\nMSG-353\nNo file extension or content type specified,
        attachment [1]: [filename,txt]"
      operationId: sendFaxMessage
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidfax-post
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account (integer) or tilde
          (~) to indicate the account which was logged-in within the current session
      - in: formData
        name: attachment
        description: File to upload
      - in: formData
        name: coverIndex
        description: Cover page identifier
      - in: formData
        name: coverPageText
        description: Cover page text, entered by the fax sender and printed on the
          cover page
      - in: path
        name: extensionId
        description: Internal identifier of an extension (integer) or tilde (~) to
          indicate the extension assigned to the account logged-in within the current
          session
      - in: formData
        name: faxResolution
        description: Resolution of Fax
      - in: formData
        name: isoCode
        description: ISO Code
      - in: formData
        name: sendTime
        description: Timestamp to send fax at
      - in: formData
        name: to
        description: To Phone Number
      responses:
        200:
          description: OK
      tags:
      - Fax
      - Message
  /restapi/v1.0/dictionary/fax-cover-page:
    get:
      summary: Get Available Fax Cover Pages
      description: "Returns fax cover pages available for the current extension.\nUsage
        Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n400\nCMN-101\nParameter [page] value is invalid\n\n\n401\nCMN-405\nLogin
        to extension required"
      operationId: listFaxCoverPages
      x-api-path-slug: restapiv1-0dictionaryfaxcoverpage-get
      parameters:
      - in: query
        name: page
        description: Indicates the page number to retrieve
      - in: query
        name: perPage
        description: Indicates the page size (number of items)
      responses:
        200:
          description: OK
      tags:
      - Available
      - Fax
      - Cover
      - Pages
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/message-store:
    get:
      summary: Get Message List
      description: "Returns the list of messages from an extension mailbox.\nApp Permission\nReadMessages\nUser
        Permission\nReadMessages\nUsage Plan Group\nLight\nError Codes\n\n \n  \n
        \  HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
        [readStatus] value is invalid\n\n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-151\nAuthorization
        method not supported\n\n\n403\nCMN-401\nIn order to call this API endpoint,
        application needs to have [ReadMessages] permission\n\n\n403\nCMN-408\nIn
        order to call this API endpoint, user needs to have [ReadMessages] permission
        for requested resource.\n\n\n404\nCMN-102\nResource for parameter [extensionId]
        is not found"
      operationId: listMessages
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidmessagestore-get
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: query
        name: availability
        description: Specifies the availability status for the resulting messages
      - in: query
        name: conversationId
        description: Specifies the conversation identifier for the resulting messages
      - in: query
        name: dateFrom
        description: The start datetime for resulting messages in ISO 8601 format
          including timezone, for example 2016-03-10T18:07:52
      - in: query
        name: dateTo
        description: The end datetime for resulting messages in ISO 8601 format including
          timezone, for example 2016-03-10T18:07:52
      - in: query
        name: direction
        description: The direction for the resulting messages
      - in: query
        name: distinctConversations
        description: If True, then the latest messages per every conversation ID are
          returned
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      - in: query
        name: messageType
        description: The type of the resulting messages
      - in: query
        name: page
        description: Indicates the page number to retrieve
      - in: query
        name: perPage
        description: Indicates the page size (number of items)
      - in: query
        name: phoneNumber
        description: The phone number
      - in: query
        name: readStatus
        description: The read status for the resulting messages
      responses:
        200:
          description: OK
      tags:
      - Message
      - List
    delete:
      summary: Delete Conversations by ID's
      description: "Deletes conversation(s) by conversation ID(s). Batch request is
        supported.\nApp Permission\nEditMessages\nUser Permission\nEditMessages\nUsage
        Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n400\nCMN-101\nParameter [conversationId] value is invalid\n\n\n403\nCMN-401\nIn
        order to call this API endpoint, application needs to have [EditMessages]
        permission"
      operationId: deleteMessagesByFilter
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidmessagestore-delete
      parameters:
      - in: path
        name: accountId
      - in: query
        name: conversationId
      - in: path
        name: extensionId
      responses:
        200:
          description: OK
      tags:
      - Conversations
      - By
      - IDs
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/message-store/{messageId}:
    get:
      summary: Get Message(s) by ID
      description: "Returns individual message record(s) by the given message ID(s).
        The length of inbound messages is unlimited. Batch request is supported.\nApp
        Permission\nReadMessages\nUser Permission\nReadMessages\nUsage Plan Group\nLight\nError
        Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n401\nCMN-405\nLogin
        to extension required\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n403\nCMN-401\nIn
        order to call this API endpoint, application needs to have [ReadMessages]
        permission\n\n\n403\nCMN-408\nIn order to call this API endpoint, user needs
        to have [ReadMessages] permission for requested resource.\n\n\n404\nCMN-102\nResource
        for parameter [extensionId] is not found"
      operationId: loadMessage
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidmessagestoremessageid-get
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      - in: path
        name: messageId
        description: Internal identifier of a message
      responses:
        200:
          description: OK
      tags:
      - Message(s)
      - By
      - ID
    put:
      summary: Update Message(s) by ID
      description: "Updates message(s) by ID(s). Batch request is supported, see Batch
        Requests for details. Currently, only the message read status updating is
        supported.\nApp Permission\nEditMessages\nUser Permission\nEditMessages\nUsage
        Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n400\nCMN-101\nParameter [] value is invalid\n\n\n403\nCMN-401\nIn
        order to call this API endpoint, application needs to have [EditMessages]
        permission\n\n\n403\nCMN-408\nIn order to call this API endpoint, user needs
        to have [EditMessages] permission for requested resource.\n\n\n404\nCMN-102\nResource
        for parameter [extensionId] is not found"
      operationId: updateMessage
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidmessagestoremessageid-put
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
      - in: path
        name: messageId
        description: Internal identifier of a message
      responses:
        200:
          description: OK
      tags:
      - Message(s)
      - By
      - ID
    delete:
      summary: Delete Message(s) by ID
      description: "Deletes message(s) by the given message ID(s). The first call
        of this method transfers the message to the &#39;Delete&#39; status. The second
        call transfers the deleted message to the &#39;Purged&#39; status. If it is
        required to make the message &#39;Purged&#39; immediately (from the first
        call), then set the query parameter purge to &#39;True&#39;.\nApp Permission\nEditMessages\nUser
        Permission\nEditMessages\nUsage Plan Group\nMedium\nError Codes\n\n \n  \n
        \  HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
        [purge] value is invalid\n\n\n403\nCMN-401\nIn order to call this API endpoint,
        application needs to have [EditMessages] permission\n\n\n403\nCMN-408\nIn
        order to call this API endpoint, user needs to have [EditMessages] permission
        for requested resource.\n\n\n404\nCMN-102\nResource for parameter [extensionId]
        is not found"
      operationId: deleteMessage
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidmessagestoremessageid-delete
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: query
        name: conversationId
        description: Internal identifier of a message thread
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      - in: path
        name: messageId
        description: Internal identifier of a message
      - in: query
        name: purge
        description: If the value is True, then the message is purged immediately
          with all the attachments
      responses:
        200:
          description: OK
      tags:
      - Message(s)
      - By
      - ID
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/message-store/{messageId}/content/{attachmentId}:
    get:
      summary: Get Message Attachment
      description: "Returns a specific message attachment data as a media stream.\nApp
        Permission\nReadMessages\nUser Permission\nReadMessageContent\nUsage Plan
        Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n401\nAGW-402\nInvalid Authorization header\n\n\n401\nCMN-405\nLogin
        to extension required\n\n\n401\nOAU-149\nUnparsable access token\n\n\n401\nOAU-151\nAuthorization
        method not supported\n\n\n403\nCMN-401\nIn order to call this API endpoint,
        application needs to have [ReadMessages] permission\n\n\n403\nCMN-408\nIn
        order to call this API endpoint, user needs to have [ReadMessageContent] permission
        for requested resource.\n\n\n404\nCMN-102\nResource for parameter [extensionId]
        is not found\n\n\n416\nCMN-107\nRequested range not satisfiable"
      operationId: preturns-a-specific-message-attachment-data-as-a-media-streamph4app-permissionh4preadmessagesph4user
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidmessagestoremessageidcontentattachmentid-get
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: path
        name: attachmentId
        description: Internal identifier of a message attachment
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      - in: path
        name: messageId
        description: Internal identifier of a message
      - in: header
        name: Range
      responses:
        200:
          description: OK
      tags:
      - Message
      - Attachment
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/message-sync:
    get:
      summary: Get Message Sync
      description: "Synchronizes messages.\nApp Permission\nReadMessages\nUser Permission\nReadMessages\nUsage
        Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n400\nCMN-101\nParameter [messageType] value is invalid\n\n\n400\nMSG-333\nParameter
        [syncToken] is invalid\n\n\n403\nCMN-401\nIn order to call this API endpoint,
        application needs to have [ReadMessages] permission\n\n\n403\nCMN-408\nIn
        order to call this API endpoint, user needs to have [ReadMessages] permission
        for requested resource.\n\n\n404\nCMN-102\nResource for parameter [extensionId]
        is not found"
      operationId: syncMessages
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidmessagesync-get
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: query
        name: conversationId
        description: Conversation identifier for the resulting messages
      - in: query
        name: dateFrom
        description: The start datetime for resulting messages in ISO 8601 format
          including timezone, for example 2016-03-10T18:07:52
      - in: query
        name: dateTo
        description: The end datetime for resulting messages in ISO 8601 format including
          timezone, for example 2016-03-10T18:07:52
      - in: query
        name: direction
        description: Direction for the resulting messages
      - in: query
        name: distinctConversations
        description: If True, then the latest messages per every conversation ID are
          returned
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      - in: query
        name: messageType
        description: Type for the resulting messages
      - in: query
        name: recordCount
        description: Limits the number of records to be returned (works in combination
          with dateFrom and dateTo if specified)
      - in: query
        name: syncToken
        description: Value of syncToken property of last sync request response
      - in: query
        name: syncType
        description: Type of message synchronization
      responses:
        200:
          description: OK
      tags:
      - Message
      - Sync
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/ring-out:
    post:
      summary: Make RingOut Call
      description: "Makes a 2-leg RingOut call.\nApp Permission\nRingOut\nUsage Plan
        Group\nHeavy\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n400\nCMN-101\nParameter [phoneNumber] value is invalid\n\n\n400\nTEL-107\nCaller
        ID: [+18609411729] is not allowed\n\n\n400\nTEL-108\nphoneNumber specified
        in the from field is empty or invalid\n\n\n400\nTEL-109\nphoneNumber specified
        in the to field is empty or invalid\n\n\n403\nBIL-103\nFeature [RingOut] is
        not available for current account\n\n\n403\nCMN-112\nFeature [RingOut] is
        not available for current extension type\n\n\n403\nCMN-113\nFeature [DomesticCalls]
        is not available for current extension\n\n\n403\nRNG-102\nCaller ID should
        be one of company direct numbers\n\n\n403\nTEL-101\nphoneNumber specified
        in the to field: [17176704078] is in blocked list\n\n\n403\nTEL-102\nphoneNumber
        specified in the from field: [17176704078] is in blocked list\n\n\n403\nTEL-107\nCaller
        ID: [+12094441763] is not allowed\n\n\n404\nCMN-102\nResource for parameter
        [forwardingNumberId] is not found"
      operationId: makeRingOutCallNew
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidringout-post
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
      - Make
      - RingOut
      - Call
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/ring-out/{ringoutId}:
    get:
      summary: Get Status of RingOut Call
      description: "Returns the status of a 2-leg RingOut call.\nApp Permission\nRingOut\nUsage
        Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n503\nCMN-201\nService Temporary Unavailable"
      operationId: getRingOutCallStatusNew
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidringoutringoutid-get
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      - in: path
        name: ringoutId
        description: Internal identifier of a RingOut call
      responses:
        200:
          description: OK
      tags:
      - Status
      - Of
      - RingOut
      - Call
    delete:
      summary: Cancel RingOut Call
      description: "Cancels a 2-leg RingOut call.\nApp Permission\nRingOut\nUsage
        Plan Group\nHeavy\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n404\nCMN-102\nResource for parameter [ringOutId] is not
        found"
      operationId: cancelRingOutCallNew
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidringoutringoutid-delete
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      - in: path
        name: ringoutId
        description: Internal identifier of a RingOut call
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - RingOut
      - Call
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/ringout:
    post:
      summary: Make RingOut Call
      description: "Makes a 2-leg RingOut call.\nApp Permission\nRingOut\nUsage Plan
        Group\nHeavy\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n400\nCMN-101\nParameter [phoneNumber] value is invalid\n\n\n400\nTEL-107\nCaller
        ID: [+14152961727] is not allowed\n\n\n400\nTEL-108\nphoneNumber specified
        in the from field is empty or invalid\n\n\n400\nTEL-109\nphoneNumber specified
        in the to field is empty or invalid\n\n\n403\nBIL-103\nFeature [RingOut] is
        not available for current account\n\n\n403\nCMN-112\nFeature [RingOut] is
        not available for current extension type\n\n\n403\nCMN-113\nFeature [DomesticCalls]
        is not available for current extension\n\n\n403\nCMN-401\nIn order to call
        this API endpoint, application needs to have [RingOut] permission\n\n\n403\nRNG-102\nCaller
        ID should be one of company direct numbers\n\n\n403\nTEL-101\nphoneNumber
        specified in the to field: [17176704073] is in blocked list\n\n\n403\nTEL-102\nphoneNumber
        specified in the from field: [17172302150] is in blocked list\n\n\n403\nTEL-107\nCaller
        ID: [+12094441789] is not allowed\n\n\n404\nCMN-102\nResource for parameter
        [extensionId] is not found"
      operationId: makeRingOutCall
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidringout-post
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
      - Make
      - RingOut
      - Call
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/ringout/{ringoutId}:
    get:
      summary: Get Status of RingOut Call
      description: "Returns status of a 2-leg RingOut call.\nApp Permission\nRingOut\nUsage
        Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-151\nAuthorization
        method not supported\n\n\n403\nCMN-401\nIn order to call this API endpoint,
        application needs to have [RingOut] permission\n\n\n404\nCMN-102\nResource
        for parameter [extensionId] is not found"
      operationId: getRingOutCallStatus
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidringoutringoutid-get
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      - in: path
        name: ringoutId
        description: Internal identifier of a RingOut call
      responses:
        200:
          description: OK
      tags:
      - Status
      - Of
      - RingOut
      - Call
    delete:
      summary: Cancel RingOut Call
      description: "Cancels a 2-leg RingOut call.\nApp Permission\nRingOut\nUsage
        Plan Group\nHeavy\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n404\nCMN-102\nResource for parameter [extensionId] is not
        found"
      operationId: cancelRingOutCall
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidringoutringoutid-delete
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      - in: path
        name: ringoutId
        description: Internal identifier of a RingOut call
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - RingOut
      - Call
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/address-book/contact:
    get:
      summary: Get Contacts
      description: "Returns user personal contacts.\nApp Permission\nReadContacts\nUser
        Permission\nReadPersonalContacts\nUsage Plan Group\nHeavy\nError Codes\n\n
        \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
        [perPage] value is invalid\n\n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-151\nAuthorization
        method not supported\n\n\n403\nCMN-401\nIn order to call this API endpoint,
        application needs to have [ReadContacts] permission\n\n\n404\nCMN-102\nResource
        for parameter [accountId] is not found"
      operationId: listContacts
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidaddressbookcontact-get
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
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
        name: phoneNumber
      - in: query
        name: sortBy
        description: Sorts results by the specified property
      - in: query
        name: startsWith
        description: If specified, only contacts whose First name or Last name start
          with the mentioned substring are returned
      responses:
        200:
          description: OK
      tags:
      - Contacts
    post:
      summary: Create Contact
      description: "Creates personal user contact.\nApp Permission\nContacts\nUser
        Permission\nEditPersonalContacts\nUsage Plan Group\nHeavy\nError Codes\n\n
        \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
        [notes] value is invalid\n\n\n400\nPAB-102\nParameter [assistantPhone] is
        invalid. Failed to parse phone number.\n\n\n400\nPAB-103\nParameter [assistantPhone]
        is invalid. The phone number is too long.\n\n\n400\nPAB-104\nParameter [assistantPhone]
        is invalid. The phone numbers starting with the asterisk are not supported.\n\n\n400\nPAB-105\nParameter
        [assistantPhone] is invalid. The extensions longer than 10 digits are not
        supported.\n\n\n400\nPAB-106\nParameter [assistantPhone] is invalid. The DTMF
        sequences longer than 64 digits are not supported.\n\n\n403\nCMN-401\nIn order
        to call this API endpoint, application needs to have [Contacts] permission\n\n\n403\nCMN-408\nIn
        order to call this API endpoint, user needs to have [EditPersonalContacts]
        permission for requested resource.\n\n\n404\nCMN-102\nResource for parameter
        [accountId] is not found"
      operationId: createContact
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidaddressbookcontact-post
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: dialingPlan
        description: A country code value complying with the [ISO 3166-1 alpha-2](https://ru
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      responses:
        200:
          description: OK
      tags:
      - Contact
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/address-book/contact/{contactId}:
    get:
      summary: Get Contact(s) by ID
      description: "Returns contact(s) by ID(s). Batch request is supported.\nApp
        Permission\nReadContacts\nUser Permission\nReadPersonalContacts\nUsage Plan
        Group\nHeavy\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n403\nCMN-401\nIn order to call this API endpoint, application
        needs to have [ReadContacts] permission\n\n\n404\nCMN-102\nResource for parameter
        [extensionId] is not found"
      operationId: loadContact
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidaddressbookcontactcontactid-get
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: path
        name: contactId
        description: Internal identifier of a contact record in the RingCentral database
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      responses:
        200:
          description: OK
      tags:
      - Contact(s)
      - By
      - ID
    put:
      summary: Update Contact(s) by ID
      description: "Updates personal contact information by contact ID(s). Batch request
        is supported\nApp Permission\nContacts\nUser Permission\nEditPersonalContacts\nUsage
        Plan Group\nHeavy\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n400\nCMN-101\nParameter [notes] value is invalid\n\n\n403\nCMN-401\nIn
        order to call this API endpoint, application needs to have [Contacts] permission\n\n\n403\nCMN-408\nIn
        order to call this API endpoint, user needs to have [EditPersonalContacts]
        permission for requested resource.\n\n\n404\nCMN-102\nResource for parameter
        [extensionId] is not found"
      operationId: updateContact
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidaddressbookcontactcontactid-put
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: contactId
        description: Internal identifier of a contact record in the RingCentral database
      - in: query
        name: dialingPlan
        description: A country code value complying with the [ISO 3166-1 alpha-2](https://ru
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      responses:
        200:
          description: OK
      tags:
      - Contact(s)
      - By
      - ID
    delete:
      summary: Delete Contact(s) by ID
      description: "Deletes contact(s) by ID(s). Batch request is supported.\nApp
        Permission\nContacts\nUser Permission\nEditPersonalContacts\nUsage Plan Group\nHeavy\nError
        Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n403\nCMN-401\nIn
        order to call this API endpoint, application needs to have [Contacts] permission\n\n\n403\nCMN-408\nIn
        order to call this API endpoint, user needs to have [EditPersonalContacts]
        permission for requested resource.\n\n\n404\nCMN-102\nResource for parameter
        [extensionId] is not found"
      operationId: deleteContact
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidaddressbookcontactcontactid-delete
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: path
        name: contactId
        description: Internal identifier of a contact record in the RingCentral database
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      responses:
        200:
          description: OK
      tags:
      - Contact(s)
      - By
      - ID
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/favorite:
    get:
      summary: Get Favorite Contacts
      description: "Returns favorite contacts of the current extension. Favorite contacts
        include both company contacts (extensions) and personal contacts (address
        book records).\nApp Permission\nReadContacts\nUser Permission\nReadPersonalContacts\nUsage
        Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n403\nCMN-401\nIn order to call this API endpoint, application
        needs to have [ReadContacts] permission\n\n\n403\nCMN-408\nIn order to call
        this API endpoint, user needs to have [ReadPersonalContacts] permission for
        requested resource.\n\n\n404\nCMN-102\nResource for parameter [accountId]
        is not found"
      operationId: listFavoriteContacts
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidfavorite-get
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      responses:
        200:
          description: OK
      tags:
      - Favorite
      - Contacts
    put:
      summary: Update Favorite Contacts
      description: "Updates favorite contacts of the current extension. Favorite contacts
        include both company contacts (extensions) and personal contacts (address
        book records).**Please note**: currently personal address book size is limited
        to 10 000 contacts.\nApp Permission\nContacts\nUser Permission\nEditPersonalContacts\nUsage
        Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n400\nCMN-101\nParameter [records.extensionId] value is
        invalid\n\n\n400\nFAV-100\nContact not found\n\n\n400\nFAV-101\nMore than
        one contact with the same [records.extensionId]\n\n\n400\nFAV-102\n[records.extensionId]
        and [records.contactId] could not be specified for one contact simultaneously\n\n\n400\nFAV-103\nMore
        than one contact with the same [records.id]\n\n\n400\nFAV-104\nContact limit
        exceeded\n\n\n400\nFAV-105\nContact not found in federated directory\n\n\n403\nCMN-401\nIn
        order to call this API endpoint, application needs to have [Contacts] permission\n\n\n404\nCMN-102\nResource
        for parameter [accountId] is not found"
      operationId: updateFavoriteContacts
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidfavorite-put
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: body
        name: body
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
      - Favorite
      - Contacts
  /restapi/v1.0/account/{accountId}/directory/contacts:
    get:
      summary: Get Corporate Directory Contacts
      description: |-
        Returns contact information on corporate users of federated accounts. Please note: 1. User, DigitalUser, VirtualUser and FaxUser types are returned as User type. 2.ApplicationExtension type is not returned. 3. Only extensions in Enabled, Disabled and NotActivated state are returned.
        App Permission
        ReadAccounts
        Usage Plan Group
        Medium
      operationId: listDirectoryContacts
      x-api-path-slug: restapiv1-0accountaccountiddirectorycontacts-get
      parameters:
      - in: path
        name: accountId
        description: accountId
      - in: query
        name: excludeFederatedContacts
        description: excludeFederatedContacts
      - in: header
        name: If-None-Match
        description: If-None-Match
      - in: query
        name: page
        description: page
      - in: query
        name: perPage
        description: perPage
      - in: query
        name: siteId
        description: Internal identifier of the business site to which extensions
          belongs
      - in: query
        name: type
        description: Type of an extension
      responses:
        200:
          description: OK
      tags:
      - Corporate
      - Directory
      - Contacts
  /restapi/v1.0/account/{accountId}/directory/contacts/{contactId}:
    get:
      summary: Get Corporate Directory Contact
      description: |-
        Returns contact information on a particular corporate user of a federated account.
        App Permission
        ReadAccounts
        Usage Plan Group
        Medium
      operationId: loadDirectoryContact
      x-api-path-slug: restapiv1-0accountaccountiddirectorycontactscontactid-get
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of owning account
      - in: path
        name: contactId
        description: Internal identifier of extension to read information for
      responses:
        200:
          description: OK
      tags:
      - Corporate
      - Directory
      - Contact
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/presence:
    get:
      summary: Get User Status
      description: "Returns presence status of an extension or several extensions
        by their ID(s). Batch request is supported. The &#39;presenceStatus&#39; is
        returned as Offline (the parameters &#39;telephonyStatus&#39;, &#39;message&#39;,
        &#39;userStatus&#39; and &#39;dndStatus&#39; are not returned at all) for
        the following extension types: Department/Announcement Only/Take Messages
        Only (Voicemail)/Fax User/Paging Only Group/Shared Lines Group/IVR Menu/Application
        Extension/Park Location.If the user requests his/her own presence status,
        the response contains actual presence status even if the status publication
        is turned off. Batch request is supported. For batch requests the number of
        extensions in one request is limited to 30. If more extensions are included
        in the request, the error code 400 Bad Request is returned with the logical
        error code InvalidMultipartRequest and the corresponding message &#39;Extension
        Presence Info multipart request is limited to 30 extensions&#39;.\nApp Permission\nReadPresence\nUser
        Permission\nReadPresenceStatus\nUsage Plan Group\nLight\nError Codes\n\n \n
        \ \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n403\nCMN-408\nIn
        order to call this API endpoint, user needs to have [ReadPresenceStatus] permission
        for requested resource.\n\n\n404\nCMN-102\nResource for parameter [extensionId]
        is not found"
      operationId: getPresenceStatus
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidpresence-get
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: query
        name: detailedTelephonyState
        description: Whether to return detailed telephony state
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      - in: query
        name: sipData
        description: Whether to return SIP data
      responses:
        200:
          description: OK
      tags:
      - User
      - Status
    put:
      summary: Update User Status
      description: "Updates user-defined extension presence status, status message
        and DnD status by extension ID. Supported for regular User extensions only.
        The extension types listed do not support presence status: Department, Announcement
        Only, Take Messages Only (Voicemail), Fax User, Paging Only Group, Shared
        Lines Group, IVR Menu, Application Extension.\nApp Permission\nEditPresence\nUsage
        Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n400\nCMN-101\nParameter [allowSeeMyPresence] value is invalid\n\n\n403\nBIL-103\nFeature
        [DND] is not available for current account\n\n\n403\nCMN-408\nIn order to
        call this API endpoint, user needs to have [EditPresenceSettings] permission
        for requested resource.\n\n\n403\nPRS-105\nNot allowed update presence for
        extensions having Disabled state\n\n\n403\nPRS-106\nNot allowed update presence
        for extensions of Department type\n\n\n404\nCMN-102\nResource for parameter
        [accountId] is not found"
      operationId: updatePresenceStatus
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidpresence-put
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: body
        name: body
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
      - User
      - Status
  /restapi/v1.0/glip/groups:
    get:
      summary: Get User Groups
      description: |-
        Returns the list of groups associated with the user.
        App Permission
        Glip
        User Permission
        Glip
        Usage Plan Group
        Medium
      operationId: listGlipGroups
      x-api-path-slug: restapiv1-0glipgroups-get
      parameters:
      - in: query
        name: pageToken
        description: Token of a page to be returned
      - in: query
        name: recordCount
        description: Max numbers of records to be returned
      - in: query
        name: type
        description: Type of a group
      responses:
        200:
          description: OK
      tags:
      - User
      - Groups
    post:
      summary: Create Group
      description: |-
        Creates a group.
        App Permission
        Glip
        User Permission
        Glip
        Usage Plan Group
        Medium
      operationId: createGlipGroup
      x-api-path-slug: restapiv1-0glipgroups-post
      parameters:
      - in: body
        name: body
        description: JSON body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Group
  /restapi/v1.0/glip/groups/{groupId}:
    get:
      summary: Get Group
      description: |-
        Returns a group or multiple groups by their ID(s). Batch request is supported.
        App Permission
        Glip
        User Permission
        Glip
        Usage Plan Group
        Light
      operationId: loadGlipGroup
      x-api-path-slug: restapiv1-0glipgroupsgroupid-get
      parameters:
      - in: path
        name: groupId
        description: Internal identifier of a group to be returned, the maximum number
          of IDs is 30
      responses:
        200:
          description: OK
      tags:
      - Group
  /restapi/v1.0/glip/groups/{groupId}/bulk-assign:
    post:
      summary: Edit Group Members
      description: |-
        Updates group members. Please note: Only groups of &#39;Team&#39; type can be updated. Currently only one operation at a time (either adding or removal) is supported.
        App Permission
        Glip
        User Permission
        Glip
        Usage Plan Group
        Medium
      operationId: assignGlipGroupMembers
      x-api-path-slug: restapiv1-0glipgroupsgroupidbulkassign-post
      parameters:
      - in: body
        name: body
        description: JSON body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: groupId
        description: Internal identifier of a group
      responses:
        200:
          description: OK
      tags:
      - Edit
      - Group
      - Members
  /restapi/v1.0/glip/groups/{groupId}/posts:
    get:
      summary: Get Group Posts
      description: |-
        Returns posts which are available for the current user (by group ID). The maximum number of posts returned is 250.
        Usage Plan Group
        Medium
      operationId: listGlipGroupPosts
      x-api-path-slug: restapiv1-0glipgroupsgroupidposts-get
      parameters:
      - in: path
        name: groupId
        description: Internal identifier of a group
      - in: query
        name: pageToken
        description: Pagination token
      - in: query
        name: recordCount
        description: Max number of records to be returned
      responses:
        200:
          description: OK
      tags:
      - Group
      - S
    post:
      summary: Create Post in Group
      description: |-
        Creates a new post in a group specified.
        Usage Plan Group
        Medium
      operationId: createGlipGroupPost
      x-api-path-slug: restapiv1-0glipgroupsgroupidposts-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: groupId
        description: Internal identifier of a group
      responses:
        200:
          description: OK
      tags:
      - In
      - Group
  /restapi/v1.0/glip/groups/{groupId}/posts/{postId}/text:
    put:
      summary: Update Post
      description: |-
        Modifies text of a post
        Usage Plan Group
        Medium
      operationId: updateGlipPostText
      x-api-path-slug: restapiv1-0glipgroupsgroupidpostspostidtext-put
      parameters:
      - in: path
        name: groupId
        description: Internal identifier of a group
      - in: path
        name: postId
        description: Internal identifier of a post
      - in: body
        name: text
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - ""
  /restapi/v1.0/glip/posts:
    get:
      summary: Get Posts
      description: |-
        Returns list of posts.
        App Permission
        Glip
        User Permission
        Glip
        Usage Plan Group
        Light
      operationId: listGlipPosts
      x-api-path-slug: restapiv1-0glipposts-get
      parameters:
      - in: query
        name: groupId
        description: Identifier of a group to filter posts
      - in: query
        name: pageToken
        description: Token of a page to be returned
      - in: query
        name: recordCount
        description: Max number of records to be returned
      responses:
        200:
          description: OK
      tags:
      - S
    post:
      summary: Create Post
      description: |-
        Creates a post.
        App Permission
        Glip
        User Permission
        Glip
        Usage Plan Group
        Light
      operationId: createPost
      x-api-path-slug: restapiv1-0glipposts-post
      parameters:
      - in: body
        name: body
        description: JSON body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - ""
  /restapi/v1.0/glip/files:
    post:
      summary: Upload File
      description: |-
        Posts a file.
        App Permission
        Glip
        User Permission
        Glip
        Usage Plan Group
        Heavy
      operationId: createGlipFile
      x-api-path-slug: restapiv1-0glipfiles-post
      parameters:
      - in: formData
        name: body
        description: The file to upload
      - in: query
        name: groupId
        description: Internal identifier of a group to which the post with attachement
          will be added to
      - in: formData
        name: name
        description: Name of a file attached
      responses:
        200:
          description: OK
      tags:
      - Upload
      - File
  /restapi/v1.0/glip/persons/{personId}:
    get:
      summary: Get Person
      description: |-
        Returns a user or multiple users by their ID(s). Batch request is supported.
        App Permission
        Glip
        User Permission
        Glip
        Usage Plan Group
        Light
      operationId: loadGlipPerson
      x-api-path-slug: restapiv1-0glippersonspersonid-get
      parameters:
      - in: path
        name: personId
        description: Internal identifier of a user to be returned, the maximum number
          of IDs is 30
      responses:
        200:
          description: OK
      tags:
      - Person
  /restapi/v1.0/glip/companies/{companyId}:
    get:
      summary: Get Company Info
      description: |-
        Returns a company by ID.
        App Permission
        Glip
        User Permission
        Glip
        Usage Plan Group
        Light
      operationId: loadGlipCompany
      x-api-path-slug: restapiv1-0glipcompaniescompanyid-get
      parameters:
      - in: path
        name: companyId
        description: Internal identifier of an RC account/Glip company, or tilde (~)
          to indicate a company the current user belongs to
      responses:
        200:
          description: OK
      tags:
      - Company
      - Info
  /restapi/v1.0/glip/groups/{groupId}/webhooks:
    post:
      summary: Create Webhook in Group
      description: |-
        Create new Webhook
        Usage Plan Group
        Medium
      operationId: createGlipGroupWebhook
      x-api-path-slug: restapiv1-0glipgroupsgroupidwebhooks-post
      parameters:
      - in: path
        name: groupId
        description: Group id
      responses:
        200:
          description: OK
      tags:
      - Webhook
      - In
      - Group
    get:
      summary: Get Webhooks in Group
      description: |-
        Returns webhooks which are available for the current user (by group ID).
        Usage Plan Group
        Medium
      operationId: listGlipGroupWebhooks
      x-api-path-slug: restapiv1-0glipgroupsgroupidwebhooks-get
      parameters:
      - in: path
        name: groupId
        description: Internal identifier of a group
      responses:
        200:
          description: OK
      tags:
      - Webhooks
      - In
      - Group
  /restapi/v1.0/glip/webhooks:
    get:
      summary: Get Webhooks
      description: |-
        Returns all webhooks.
        Usage Plan Group
        Medium
      operationId: listGlipWebhooks
      x-api-path-slug: restapiv1-0glipwebhooks-get
      responses:
        200:
          description: OK
      tags:
      - Webhooks
  /restapi/v1.0/glip/webhooks/{webhookId}:
    get:
      summary: Get Webhook
      description: |-
        Returns webhooks(s) with the specified id(s).
        Usage Plan Group
        Medium
      operationId: loadGlipWebhook
      x-api-path-slug: restapiv1-0glipwebhookswebhookid-get
      parameters:
      - in: path
        name: webhookId
        description: Internal identifier of a webhook or comma separated list of webhooks
          IDs
      responses:
        200:
          description: OK
      tags:
      - Webhook
    delete:
      summary: Delete Webhook
      description: |-
        Deletes the webhook by ID.
        Usage Plan Group
        Medium
      operationId: deleteGlipWebhook
      x-api-path-slug: restapiv1-0glipwebhookswebhookid-delete
      parameters:
      - in: path
        name: webhookId
        description: Internal identifier of a webhook
      responses:
        200:
          description: OK
      tags:
      - Webhook
  /restapi/v1.0/glip/webhooks/{webhookId}/activate:
    post:
      summary: Activate Webhook
      description: |-
        Activates webhooks by ID.
        Usage Plan Group
        Medium
      operationId: activateGlipWebhook
      x-api-path-slug: restapiv1-0glipwebhookswebhookidactivate-post
      parameters:
      - in: path
        name: webhookId
        description: Internal identifier of a webhook
      responses:
        200:
          description: OK
      tags:
      - Activate
      - Webhook
  /restapi/v1.0/glip/webhooks/{webhookId}/suspend:
    post:
      summary: Suspend Webhook
      description: |-
        Suspends webhooks by ID.
        Usage Plan Group
        Medium
      operationId: suspendGlipWebhook
      x-api-path-slug: restapiv1-0glipwebhookswebhookidsuspend-post
      parameters:
      - in: path
        name: webhookId
        description: Internal identifier of a webhook
      responses:
        200:
          description: OK
      tags:
      - Suspend
      - Webhook
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/meeting:
    get:
      summary: Get Scheduled Meetings [Beta]
      description: |-
        Returns a list of meetings for a particular extension. The list of meetings does not include meetings of &#39;Instant&#39; type.
        App Permission
        Meetings
        User Permission
        Meetings
        Usage Plan Group
        Light
      operationId: listMeetings
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidmeeting-get
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      responses:
        200:
          description: OK
      tags:
      - Scheduled
      - Meetings
      - '[Beta]'
    post:
      summary: Create Meetings [Beta]
      description: "Creates a new meeting.\nApp Permission\nMeetings\nUser Permission\nMeetings\nUsage
        Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n400\nCMN-101\nParameter [schedule] value is invalid\n\n\n404\nCMN-102\nResource
        for parameter [extensionId] is not found"
      operationId: createMeeting
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidmeeting-post
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: body
        name: body
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
      - Meetings
      - '[Beta]'
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/meeting/{meetingId}:
    get:
      summary: Get Meeting Info [Beta]
      description: "Returns a particular meetings details by ID.\nApp Permission\nMeetings\nUser
        Permission\nMeetings\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP
        Code\n   Error Code\n   Error Message\n   \n \n\n404\nCMN-102\nResource for
        parameter [meetingId] is not found"
      operationId: loadMeeting
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidmeetingmeetingid-get
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      - in: path
        name: meetingId
        description: Internal identifier of a RingCentral meeting
      responses:
        200:
          description: OK
      tags:
      - Meeting
      - Info
      - '[Beta]'
    put:
      summary: Update Meeting
      description: "Modifies a particular meeting.\nApp Permission\nMeetings\nUser
        Permission\nMeetings\nUsage Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP
        Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter [password]
        value is invalid\n\n\n404\nCMN-102\nResource for parameter [extensionId] is
        not found"
      operationId: updateMeeting
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidmeetingmeetingid-put
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      - in: path
        name: meetingId
        description: Internal identifier of a RingCentral meeting
      responses:
        200:
          description: OK
      tags:
      - Meeting
    delete:
      summary: Delete Meeting
      description: |-
        Deletes a scheduled meeting.
        App Permission
        Meetings
        User Permission
        Meetings
        Usage Plan Group
        Medium
      operationId: deleteMeeting
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidmeetingmeetingid-delete
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      - in: path
        name: meetingId
        description: Internal identifier of a RingCentral meeting
      responses:
        200:
          description: OK
      tags:
      - Meeting
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/meeting/{meetingId}/end:
    post:
      summary: End Meeting
      description: "Ends a meetings which is in progress.\nApp Permission\nMeetings\nUser
        Permission\nMeetings\nUsage Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP
        Code\n   Error Code\n   Error Message\n   \n \n\n404\nCMN-102\nResource for
        parameter [meetingId] is not found"
      operationId: endMeeting
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidmeetingmeetingidend-post
      parameters:
      - in: path
        name: accountId
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      - in: path
        name: meetingId
        description: Internal identifier of a RingCentral meeting
      responses:
        200:
          description: OK
      tags:
      - End
      - Meeting
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/meeting/service-info:
    get:
      summary: Get Meeting Service Info
      description: "Returns information on dial-in numbers for meetings, support and
        international dial-in numbers URIs and meeting account information.\nApp Permission\nMeetings\nUser
        Permission\nMeetings\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP
        Code\n   Error Code\n   Error Message\n   \n \n\n403\nCMN-401\nIn order to
        call this API endpoint, application needs to have [Meetings] permission\n\n\n403\nCMN-408\nIn
        order to call this API endpoint, user needs to have [Meetings] permission
        for requested resource."
      operationId: loadMeetingServiceInfo
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidmeetingserviceinfo-get
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      responses:
        200:
          description: OK
      tags:
      - Meeting
      - Service
      - Info
  /restapi/v1.0/subscription:
    get:
      summary: Get Subscriptions
      description: |-
        Returns a list of subscriptions created by a particular user on a particular client app.
        Usage Plan Group
        Light
      operationId: listSubscriptions
      x-api-path-slug: restapiv1-0subscription-get
      responses:
        200:
          description: OK
      tags:
      - Subscriptions
    post:
      summary: Create Subscription
      description: "Creates a new subscription.\nUsage Plan Group\nMedium\nError Codes\n\n
        \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
        [deliveryMode.verificationToken] value is invalid\n\n\n400\nSUB-515\nSubscription
        containing only reminder filter is not allowed\n\n\n400\nSUB-522\nWebHook
        responds with incorrect HTTP status. HTTP status is 500\n\n\n400\nSUB-525\nWebHook
        server response is invalid\n\n\n401\nAGW-401\nAuthorization header is not
        specified\n\n\n401\nAGW-402\nInvalid Authorization header\n\n\n401\nCMN-405\nLogin
        to extension required\n\n\n403\nSUB-406\nNot allowed subscribe for events
        to extensions of other account\n\n\n403\nSUB-408\nNot allowed subscribe for
        unknown user\n\n\n403\nSUB-505\nSubscriptions limit exceeded\n\n\n403\nSUB-518\nNot
        allowed subscribe for favorite contacts list changes of another extension\n\n\n403\nSUB-527\nNot
        allowed subscribe for missed calls of another extension\n\n\n403\nSUB-528\n[SubscriptionAPNS]
        application permission is required for [PubNub/APNS] transport\n\n\n403\nSUB-530\nNot
        allowed subscribe for incoming calls of another extension\n\n\n403\nSUB-531\nNot
        allowed subscribe for presence of presence-lines of another extension\n\n\n404\nCMN-102\nResource
        for parameter [dashboardId] is not found"
      operationId: createSubscription
      x-api-path-slug: restapiv1-0subscription-post
      parameters:
      - in: body
        name: body
        description: JSON body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Subscription
  /restapi/v1.0/subscription/{subscriptionId}:
    get:
      summary: Get Subscription
      description: "Returns the requested subscription.\nUsage Plan Group\nLight\nError
        Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n401\nCMN-405\nLogin
        to extension required\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n404\nCMN-102\nResource
        for parameter [subscriptionId] is not found\n\n\n404\nCMN-120\nInvalid URI"
      operationId: loadSubscription
      x-api-path-slug: restapiv1-0subscriptionsubscriptionid-get
      parameters:
      - in: path
        name: subscriptionId
        description: Internal identifier of a subscription
      responses:
        200:
          description: OK
      tags:
      - Subscription
    put:
      summary: Renew Subscription / Update Event Filters
      description: "Renews the existent subscription if the request body is empty.
        If event filters are specified, calling this method modifies the event filters
        for the existing subscription. The client application can extend or narrow
        the events for which it receives notifications in the frame of one subscription.\nUsage
        Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n404\nCMN-102\nResource for parameter [subscriptionId] is
        not found"
      operationId: updateSubscription
      x-api-path-slug: restapiv1-0subscriptionsubscriptionid-put
      parameters:
      - in: query
        name: aggregated
        description: If True then aggregated presence status is returned in a notification
          payload
      - in: body
        name: body
        description: JSON body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: subscriptionId
        description: Internal identifier of a subscription
      responses:
        200:
          description: OK
      tags:
      - Renew
      - Subscription
      - ""
      - ""
      - ""
      - Event
      - Filters
    delete:
      summary: Cancel Subscription
      description: "Cancels the existent subscription.\nUsage Plan Group\nMedium\nError
        Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n404\nCMN-102\nResource
        for parameter [subscriptionId] is not found"
      operationId: deleteSubscription
      x-api-path-slug: restapiv1-0subscriptionsubscriptionid-delete
      parameters:
      - in: path
        name: subscriptionId
        description: Internal identifier of a subscription
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Subscription
  /restapi/v1.0/subscription/{subscriptionId}/renew:
    post:
      summary: Renew Subscription
      description: |-
        Renews an existent subscription by ID by posting request with an empty body.
        Usage Plan Group
        Light
      operationId: renewSubscription
      x-api-path-slug: restapiv1-0subscriptionsubscriptionidrenew-post
      parameters:
      - in: path
        name: subscriptionId
      responses:
        200:
          description: OK
      tags:
      - Renew
      - Subscription
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/authz-profile:
    get:
      summary: Get User Permissions
      description: "Returns a list of user permissions granted at authorization procedure.
        Please note: Some permissions may be restricted by extension type.\nUsage
        Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n403\nCMN-404\nAttempt to access another extension\n\n\n404\nCMN-102\nResource
        for parameter [accountId] is not found"
      operationId: getAuthorizationProfile
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidauthzprofile-get
      parameters:
      - in: path
        name: accountId
      - in: path
        name: extensionId
      responses:
        200:
          description: OK
      tags:
      - User
      - Permissions
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/authz-profile/check:
    get:
      summary: Check User Permissions
      description: "Checks if a certain user permission is activated for a particular
        extension.\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n
        \  Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter [targetExtensionId]
        value is invalid\n\n\n403\nCMN-404\nAttempt to access another extension\n\n\n404\nCMN-102\nResource
        for parameter [accountId] is not found"
      operationId: checkUserPermission
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidauthzprofilecheck-get
      parameters:
      - in: path
        name: accountId
      - in: path
        name: extensionId
      - in: query
        name: permissionId
      - in: query
        name: targetExtensionId
      responses:
        200:
          description: OK
      tags:
      - Check
      - User
      - Permissions
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/business-hours:
    get:
      summary: Get User Business Hours
      description: "Returns the extension user hours when answering rules are to be
        applied.\nApp Permission\nReadAccounts\nUser Permission\nReadExtensions\nUsage
        Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-151\nAuthorization
        method not supported\n\n\n403\nCMN-401\nIn order to call this API endpoint,
        application needs to have [ReadAccounts] permission\n\n\n403\nCMN-408\nIn
        order to call this API endpoint, user needs to have [ReadUserAnsweringRules]
        permission for requested resource.\n\n\n404\nCMN-102\nResource for parameter
        [extensionId] is not found"
      operationId: loadUserBusinessHours
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidbusinesshours-get
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      responses:
        200:
          description: OK
      tags:
      - User
      - Business
      - Hours
    put:
      summary: Update User Business Hours
      description: "Updates the extension user hours when answering rules are to be
        applied.\nApp Permission\nEditExtensions\nUser Permission\nEditUserAnsweringRules\nUsage
        Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n400\nCMN-101\nParameter [ranges] value is invalid\n\n\n403\nCMN-401\nIn
        order to call this API endpoint, application needs to have [EditExtensions]
        permission\n\n\n404\nCMN-102\nResource for parameter [extensionId] is not
        found"
      operationId: updateUserBusinessHours
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidbusinesshours-put
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
      - User
      - Business
      - Hours
  /restapi/v1.0/account/{accountId}/business-hours:
    get:
      summary: Get Company Business Hours
      description: |-
        Returns company hours when answering rules are to be applied.
        App Permission
        ReadAccounts
        User Permission
        ReadUserAnsweringRules
        Usage Plan Group
        Light
      operationId: loadBusinesshoursInfo
      x-api-path-slug: restapiv1-0accountaccountidbusinesshours-get
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      responses:
        200:
          description: OK
      tags:
      - Company
      - Business
      - Hours
    put:
      summary: Update Company Business Hours
      description: "Updates company hours when answering rules are to be applied.\nApp
        Permission\nEditExtensions\nUser Permission\nEditUserAnsweringRules\nUsage
        Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n400\nAWR-176\nAt least one time range for [monday] required\n\n\n400\nAWR-177\nTime
        ranges limit for [monday] exceeded\n\n\n400\nCMN-101\nParameter [schedule.weeklyRanges]
        value is invalid"
      operationId: updateCompanyBusinessHours
      x-api-path-slug: restapiv1-0accountaccountidbusinesshours-put
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
      responses:
        200:
          description: OK
      tags:
      - Company
      - Business
      - Hours
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/blocked-number:
    get:
      summary: Get Blocked Numbers
      description: "Returns the list of phone numbers which are specified by the user
        to block inbound calls and SMS messages.\nApp Permission\nReadAccounts\nUser
        Permission\nReadBlockedNumbers\nUsage Plan Group\nLight\nError Codes\n\n \n
        \ \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
        [perPage] value is invalid\n\n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-151\nAuthorization
        method not supported\n\n\n403\nCMN-401\nIn order to call this API endpoint,
        application needs to have [ReadAccounts] permission\n\n\n403\nCMN-408\nIn
        order to call this API endpoint, user needs to have [ReadBlockedNumbers] permission
        for requested resource.\n\n\n404\nCMN-102\nResource for parameter [extensionId]
        is not found"
      operationId: listBlockedNumbers
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidblockednumber-get
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      responses:
        200:
          description: OK
      tags:
      - Blocked
      - Numbers
    post:
      summary: Add Blocked Numbers
      description: "Adds a new phone number to the blocked number list.\nApp Permission\nEditExtensions\nUser
        Permission\nEditBlockedNumbers\nUsage Plan Group\nMedium\nError Codes\n\n
        \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
        [phoneNumber] value is invalid\n\n\n403\nCMN-401\nIn order to call this API
        endpoint, application needs to have [EditExtensions] permission\n\n\n403\nCMN-408\nIn
        order to call this API endpoint, user needs to have [EditBlockedNumbers] permission
        for requested resource.\n\n\n404\nCMN-102\nResource for parameter [extensionId]
        is not found"
      operationId: blockNumber
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidblockednumber-post
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: body
        name: body
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
      - Blocked
      - Numbers
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/blocked-number/{blockedNumberId}:
    get:
      summary: Get Blocked Number
      description: "Returns specific information on blocked phone number(s) by their
        ID(s). Batch request is supported.\nApp Permission\nReadAccounts\nUser Permission\nReadBlockedNumbers\nUsage
        Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n403\nCMN-401\nIn order to call this API endpoint, application
        needs to have [ReadAccounts] permission\n\n\n403\nCMN-408\nIn order to call
        this API endpoint, user needs to have [ReadBlockedNumbers] permission for
        requested resource.\n\n\n404\nCMN-102\nResource for parameter [accountId]
        is not found"
      operationId: loadBlockedNumber
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidblockednumberblockednumberid-get
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: path
        name: blockedNumberId
        description: Internal identifiers of a blocked number list entry
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      responses:
        200:
          description: OK
      tags:
      - Blocked
      - Number
    put:
      summary: Update Blocked Number
      description: "Updates blocked number(s) by their ID(s). Currently only the name
        can be updated. Batch request is supported.\nApp Permission\nEditExtensions\nUser
        Permission\nEditBlockedNumbers\nUsage Plan Group\nMedium\nError Codes\n\n
        \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
        [] value is invalid\n\n\n403\nCMN-401\nIn order to call this API endpoint,
        application needs to have [EditExtensions] permission\n\n\n403\nCMN-408\nIn
        order to call this API endpoint, user needs to have [EditBlockedNumbers] permission
        for requested resource.\n\n\n404\nCMN-102\nResource for parameter [extensionId]
        is not found"
      operationId: updateBlockedNumber
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidblockednumberblockednumberid-put
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: path
        name: blockedNumberId
        description: Internal identifier of a blocked number list entry
      - in: body
        name: body
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
      - Blocked
      - Number
    delete:
      summary: Delete Blocked Number
      description: "Deletes a phone number from the blocked number list. Batch request
        is supported.\nApp Permission\nEditExtensions\nUser Permission\nEditBlockedNumbers\nUsage
        Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n403\nCMN-401\nIn order to call this API endpoint, application
        needs to have [EditExtensions] permission\n\n\n403\nCMN-408\nIn order to call
        this API endpoint, user needs to have [EditBlockedNumbers] permission for
        requested resource.\n\n\n404\nCMN-102\nResource for parameter [extensionId]
        is not found"
      operationId: unblockNumber
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidblockednumberblockednumberid-delete
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: path
        name: blockedNumberId
        description: Internal identifiers of a blocked number list entry
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      responses:
        200:
          description: OK
      tags:
      - Blocked
      - Number
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/caller-blocking:
    get:
      summary: Get Caller Blocking Settings
      description: |-
        Returns the current call blocking settings of a user.
        App Permission
        ReadAccounts
        User Permission
        ReadBlockedNumbers
        Usage Plan Group
        Light
      operationId: listCallBlockingSettings
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidcallerblocking-get
      parameters:
      - in: path
        name: accountId
      - in: path
        name: extensionId
      responses:
        200:
          description: OK
      tags:
      - Caller
      - Blocking
      - Settings
    put:
      summary: Update Caller Blocking Settings
      description: "Updates the current call blocking settings of a user.\nApp Permission\nEditExtensions\nUser
        Permission\nEditBlockedNumbers\nUsage Plan Group\nLight\nError Codes\n\n \n
        \ \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
        [greetings] value is invalid"
      operationId: updateCallBlockingSettings
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidcallerblocking-put
      parameters:
      - in: path
        name: accountId
      - in: path
        name: extensionId
      responses:
        200:
          description: OK
      tags:
      - Caller
      - Blocking
      - Settings
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/caller-blocking/phone-numbers:
    get:
      summary: Get Blocked Numbers
      description: "Returns the lists of blocked and allowed phone numbers.\nApp Permission\nReadAccounts\nUser
        Permission\nReadBlockedNumbers\nUsage Plan Group\nLight\nError Codes\n\n \n
        \ \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n404\nCMN-102\nResource
        for parameter [accountId] is not found"
      operationId: listBlockedAllowedPhoneNumberLists
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidcallerblockingphonenumbers-get
      parameters:
      - in: path
        name: accountId
      - in: path
        name: extensionId
      - in: query
        name: page
      - in: query
        name: perPage
      - in: query
        name: status
      responses:
        200:
          description: OK
      tags:
      - Blocked
      - Numbers
    post:
      summary: Add Blocked Number
      description: |-
        Updates either blocked or allowed phone number list with a new phone number.
        App Permission
        EditExtensions
        User Permission
        EditBlockedNumbers
        Usage Plan Group
        Medium
      operationId: createBlockedAllowedPhoneNumberLists
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidcallerblockingphonenumbers-post
      parameters:
      - in: path
        name: accountId
      - in: path
        name: extensionId
      responses:
        200:
          description: OK
      tags:
      - Blocked
      - Number
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/caller-blocking/phone-numbers/{blockedNumberId}:
    get:
      summary: Get Blocked Number
      description: "Returns blocked or allowed phone number(s) by their ID(s). Batch
        request is supported.\nApp Permission\nReadAccounts\nUser Permission\nReadBlockedNumbers\nUsage
        Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n404\nCMN-102\nResource for parameter [accountId] is not
        found"
      operationId: listBlockedAllowedPhoneNumber
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidcallerblockingphonenumbersblockednumberid-get
      parameters:
      - in: path
        name: accountId
      - in: path
        name: blockedNumberId
      - in: path
        name: extensionId
      responses:
        200:
          description: OK
      tags:
      - Blocked
      - Number
    delete:
      summary: Delete Blocked Number
      description: |-
        Deletes blocked or allowed phone number(s) by their ID(s). Batch request is supported.
        App Permission
        EditExtensions
        User Permission
        EditBlockedNumbers
        Usage Plan Group
        Medium
      operationId: deleteBlockedAllowedPhoneNumber
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidcallerblockingphonenumbersblockednumberid-delete
      parameters:
      - in: path
        name: accountId
      - in: path
        name: blockedNumberId
      - in: path
        name: extensionId
      responses:
        200:
          description: OK
      tags:
      - Blocked
      - Number
    put:
      summary: Update Blocked Number
      description: |-
        Updates blocked or allowed phone number(s) by their ID(s). Batch request is supported.
        App Permission
        EditExtensions
        User Permission
        EditBlockedNumbers
        Usage Plan Group
        Medium
      operationId: updateBlockedAllowedPhoneNumber
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidcallerblockingphonenumbersblockednumberid-put
      parameters:
      - in: path
        name: accountId
      - in: path
        name: blockedNumberId
      - in: path
        name: extensionId
      responses:
        200:
          description: OK
      tags:
      - Blocked
      - Number
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/forwarding-number:
    get:
      summary: Get Forwarding Numbers
      description: "Returns the list of extension phone numbers used for call forwarding
        and call flip. The returned list contains all the extension phone numbers
        used for call forwarding and call flip.\nApp Permission\nReadAccounts\nUser
        Permission\nReadUserForwardingFlipNumbers\nUsage Plan Group\nLight\nError
        Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
        [perPage] value is invalid\n\n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-151\nAuthorization
        method not supported\n\n\n403\nCMN-401\nIn order to call this API endpoint,
        application needs to have [ReadAccounts] permission\n\n\n403\nCMN-403\nThe
        feature is not available for this extension type\n\n\n403\nCMN-408\nIn order
        to call this API endpoint, user needs to have [ReadUserForwardingFlipNumbers]
        permission for requested resource.\n\n\n404\nCMN-102\nResource for parameter
        [accountId] is not found"
      operationId: listExtensionForwardingNumbers
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidforwardingnumber-get
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
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
      responses:
        200:
          description: OK
      tags:
      - Forwarding
      - Numbers
    post:
      summary: Create Forwarding Numbers
      description: "Adds a new forwarding number to the forwarding number list.\nApp
        Permission\nEditExtensions\nUser Permission\nEditUserForwardingFlipNumbers\nUsage
        Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n400\nAWR-180\nCall handling settings not available for
        Fax tiers\n\n\n400\nCMN-101\nParameter [phoneNumber] value is invalid\n\n\n400\nFPN-102\nLabel
        of number Work duplicates with existing forwarding number label\n\n\n400\nFPN-103\nLimit
        of available forwarding numbers (10) exceeded\n\n\n400\nFPN-104\nLimit of
        available custom labeled forwarding numbers (7) exceeded\n\n\n400\nFPN-105\nNumber
        +18442015485 duplicates with company/extension direct number\n\n\n400\nFPN-108\nInternational
        calling is currently disabled\n\n\n403\nCMN-401\nIn order to call this API
        endpoint, application needs to have [EditExtensions] permission\n\n\n403\nCMN-403\nThe
        feature is not available for this extension type\n\n\n404\nCMN-102\nResource
        for parameter [extensionId] is not found"
      operationId: createExtensionForwardingNumber
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidforwardingnumber-post
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
      - Forwarding
      - Numbers
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/forwarding-number/{forwardingNumberId}:
    get:
      summary: Get Forwarding Number
      description: "Returns a specific forwarding number.\nApp Permission\nReadAccounts\nUser
        Permission\nReadUserForwardingFlipNumbers\nUsage Plan Group\nLight\nError
        Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n403\nCMN-401\nIn
        order to call this API endpoint, application needs to have [ReadAccounts]
        permission\n\n\n403\nCMN-403\nThe feature is not available for this extension
        type\n\n\n403\nCMN-408\nIn order to call this API endpoint, user needs to
        have [ReadUserForwardingFlipNumbers] permission for requested resource.\n\n\n404\nCMN-102\nResource
        for parameter [accountId] is not found"
      operationId: getForwardingNumber
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidforwardingnumberforwardingnumberid-get
      parameters:
      - in: path
        name: accountId
      - in: path
        name: extensionId
      - in: path
        name: forwardingNumberId
      responses:
        200:
          description: OK
      tags:
      - Forwarding
      - Number
    put:
      summary: Update Forwarding Numbers
      description: "Updates the existing forwarding number from the forwarding number
        list.\nApp Permission\nEditExtensions\nUser Permission\nEditUserForwardingFlipNumbers\nUsage
        Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n400\nCMN-101\nParameter [flipNumber] value is invalid\n\n\n400\nFPN-102\nLabel
        of number Home duplicates with existing forwarding number label\n\n\n400\nFPN-105\nNumber
        +18552050457 duplicates with company/extension direct number\n\n\n400\nFPN-106\nFlip
        number 2 is already in use\n\n\n400\nFPN-108\nInternational calling is currently
        disabled\n\n\n403\nCMN-401\nIn order to call this API endpoint, application
        needs to have [EditExtensions] permission\n\n\n403\nCMN-408\nIn order to call
        this API endpoint, user needs to have [EditUserForwardingFlipNumbers] permission
        for requested resource.\n\n\n404\nCMN-102\nResource for parameter [forwardingNumberId]
        is not found"
      operationId: updateExtensionForwardingNumber
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidforwardingnumberforwardingnumberid-put
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
      - in: path
        name: forwardingNumberId
        description: Internal identifier of a forwarding number; returned in response
          in the id field
      responses:
        200:
          description: OK
      tags:
      - Forwarding
      - Numbers
    delete:
      summary: Delete Forwarding Number
      description: "Deletes a forwarding number from the forwarding number list by
        its ID.\nApp Permission\nEditExtensions\nUser Permission\nEditUserForwardingFlipNumbers\nUsage
        Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n403\nCMN-408\nIn order to call this API endpoint, user
        needs to have [EditUserForwardingFlipNumbers] permission for requested resource.\n\n\n403\nFPN-107\nDevice
        number cannot be deleted from the forwarding number list\n\n\n404\nCMN-102\nResource
        for parameter [forwardingNumberId] is not found"
      operationId: deleteExtensionForwardingNumber
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidforwardingnumberforwardingnumberid-delete
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      - in: path
        name: forwardingNumberId
        description: Internal identifier of a forwarding number
      responses:
        200:
          description: OK
      tags:
      - Forwarding
      - Number
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/answering-rule:
    get:
      summary: Get Call Handling Rules
      description: "Returns the extension answering rules.\nApp Permission\nReadAccounts\nUser
        Permission\nReadUserAnsweringRules\nUsage Plan Group\nMedium\nError Codes\n\n
        \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
        [perPage] value is invalid\n\n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-151\nAuthorization
        method not supported\n\n\n403\nCMN-401\nIn order to call this API endpoint,
        application needs to have [ReadAccounts] permission\n\n\n403\nCMN-408\nIn
        order to call this API endpoint, user needs to have [ReadUserAnsweringRules]
        permission for requested resource.\n\n\n404\nCMN-102\nResource for parameter
        [accountId] is not found"
      operationId: loadAnsweringRulesList
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidansweringrule-get
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      - in: query
        name: page
      - in: query
        name: perPage
      responses:
        200:
          description: OK
      tags:
      - Call
      - Handling
      - Rules
    post:
      summary: Create Custom Call Handling Rules
      description: "Creates a custom answering rule for a particular caller ID.\nApp
        Permission\nEditExtensions\nUser Permission\nEditUserAnsweringRules\nUsage
        Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n400\nAWR-100\nRule indexes should be sequential\n\n\n400\nAWR-101\nParameter
        [forwarding.rules[].forwardingNumbers[].id] are duplicated\n\n\n400\nAWR-106\nGreeting
        [Voicemail] is duplicated\n\n\n400\nAWR-107\nMore than one caller with the
        same [callerId]\n\n\n400\nAWR-108\nOnly custom rule can be created\n\n\n400\nAWR-111\nAt
        least one condition should be specified\n\n\n400\nAWR-113\nMore than one called
        number with the same [calledNumbers.phoneNumber]\n\n\n400\nAWR-121\nBusiness
        Hours not specified for current user\n\n\n400\nAWR-123\nPreset [131840] can
        not be used for greeting type [Voicemail]\n\n\n400\nAWR-124\npresetId specified
        for greeting type [Voicemail] is not found\n\n\n400\nAWR-125\nCustom greeting
        presetId specified for greeting type [Introductory]. Custom greeting uploading
        method should be used\n\n\n400\nAWR-126\nThe amount of schedule ranges exceeds
        1000\n\n\n400\nAWR-136\nRing group with index 1 is not found\n\n\n400\nAWR-137\nRule
        index should be greater than 0\n\n\n400\nAWR-138\nContact center number cannot
        be used as called number\n\n\n400\nAWR-139\nHold audio interruption period
        not specified\n\n\n400\nAWR-140\nHold audio interruption period should be
        empty for interruption mode specified\n\n\n400\nAWR-144\nCall Queue agent
        with index 1 is not found\n\n\n400\nAWR-147\nPreset [65792] can not be used
        for extension type [Department]\n\n\n400\nAWR-148\nCall Queue agents should
        be the same as call queue members\n\n\n400\nAWR-149\nOnly user, voicemail
        or shared line group extension can be a voicemail recipient\n\n\n400\nAWR-150\nOnly
        user, voicemail, shared line group extension or current department can be
        a voicemail recipient\n\n\n400\nAWR-152\nVoicemail cannot be turned off for
        call queue extension\n\n\n400\nAWR-177\nTime ranges limit for [monday] exceeded\n\n\n400\nAWR-179\n[name]
        is too long: up to 127 symbols supported\n\n\n400\nCMN-101\nParameter [name]
        value is invalid\n\n\n400\nFPN-105\nNumber +16196093249 duplicates with company/extension
        direct number\n\n\n400\nFPN-108\nInternational calling is currently disabled\n\n\n403\nCMN-401\nIn
        order to call this API endpoint, application needs to have [EditExtensions]
        permission\n\n\n403\nCMN-408\nIn order to call this API endpoint, user needs
        to have [EditUserAnsweringRules] permission for requested resource.\n\n\n404\nCMN-102\nResource
        for parameter [accountId] is not found"
      operationId: createAnsweringRuleInfo
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidansweringrule-post
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
      - Custom
      - Call
      - Handling
      - Rules
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/answering-rule/{ruleId}:
    get:
      summary: Get Call Handling Rule
      description: "Returns an answering rule by ID.\nApp Permission\nReadAccounts\nUser
        Permission\nReadUserAnsweringRules\nUsage Plan Group\nLight\nError Codes\n\n
        \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
        [showInactiveNumbers] value is invalid\n\n\n403\nCMN-401\nIn order to call
        this API endpoint, application needs to have [ReadAccounts] permission\n\n\n404\nCMN-102\nResource
        for parameter [answering-rule] is not found"
      operationId: loadAnsweringRuleInfo
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidansweringruleruleid-get
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      - in: path
        name: ruleId
        description: Internal identifier of an answering rule
      - in: query
        name: showInactiveNumbers
        description: Indicates whether invactive numbers should be returned or not
      responses:
        200:
          description: OK
      tags:
      - Call
      - Handling
      - Rule
    put:
      summary: Update Custom Call Handling Rule
      description: "Updates a custom answering rule for a particular caller ID.\nApp
        Permission\nEditExtensions\nUser Permission\nEditUserAnsweringRules\nUsage
        Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n400\nAWR-100\nRule indexes should be sequential\n\n\n400\nAWR-106\nGreeting
        [Voicemail] is duplicated\n\n\n400\nAWR-111\nAt least one condition should
        be specified\n\n\n400\nAWR-113\nMore than one called number with the same
        [calledNumbers.phoneNumber]\n\n\n400\nAWR-120\nBusiness Hours/After Hours
        schedule condition is allowed only with other answering rule conditions\n\n\n400\nAWR-123\nPreset
        [131840] can not be used for greeting type [Voicemail]\n\n\n400\nAWR-124\npresetId
        specified for greeting type [Voicemail] is not found\n\n\n400\nAWR-136\nRing
        group with index 1 is not found\n\n\n400\nAWR-137\nRule index should be greater
        than 0\n\n\n400\nAWR-138\nContact center number cannot be used as called number\n\n\n400\nAWR-139\nHold
        audio interruption period not specified\n\n\n400\nAWR-140\nHold audio interruption
        period should be empty for interruption mode specified\n\n\n400\nAWR-144\nCall
        Queue agent with index 1 is not found\n\n\n400\nAWR-147\nPreset [65792] can
        not be used for extension type [Department]\n\n\n400\nAWR-148\nCall Queue
        agents should be the same as call queue members\n\n\n400\nAWR-179\n[name]
        is too long: up to 127 symbols supported\n\n\n400\nCMN-101\nParameter [callHandlingAction]
        value is invalid\n\n\n400\nFPN-105\nNumber +18332051179 duplicates with company/extension
        direct number\n\n\n400\nFPN-108\nInternational calling is currently disabled\n\n\n403\nCMN-401\nIn
        order to call this API endpoint, application needs to have [EditExtensions]
        permission\n\n\n404\nCMN-102\nResource for parameter [accountId] is not found"
      operationId: updateAnsweringRuleInfo
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidansweringruleruleid-put
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
      - in: path
        name: ruleId
        description: Internal identifier of an answering rule
      responses:
        200:
          description: OK
      tags:
      - Custom
      - Call
      - Handling
      - Rule
    delete:
      summary: Delete Call Handling Rule
      description: "Deletes a custom answering rule by a particular ID.\nApp Permission\nEditExtensions\nUser
        Permission\nEditUserAnsweringRules\nUsage Plan Group\nMedium\nError Codes\n\n
        \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n403\nAWR-110\nBusiness
        Hours/After Hours rule cannot be deleted\n\n\n403\nCMN-401\nIn order to call
        this API endpoint, application needs to have [EditExtensions] permission\n\n\n403\nCMN-408\nIn
        order to call this API endpoint, user needs to have [EditUserAnsweringRules]
        permission for requested resource.\n\n\n404\nCMN-102\nResource for parameter
        [answering-rule] is not found"
      operationId: deleteAnsweringRule
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidansweringruleruleid-delete
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      - in: path
        name: ruleId
        description: Internal identifier of an answering rule
      responses:
        200:
          description: OK
      tags:
      - Call
      - Handling
      - Rule
  /restapi/v1.0/account/{accountId}/answering-rule:
    post:
      summary: Create Company Call Handling Rule
      description: "Creates a company answering rule for a particular caller ID.\nApp
        Permission\nEditAccounts\nUser Permission\nEditCompanyAnsweringRules\nUsage
        Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n400\nAWR-106\nGreeting [Company] is duplicated\n\n\n400\nAWR-108\nOnly
        custom rule can be created\n\n\n400\nAWR-120\nBusiness Hours/After Hours schedule
        condition is allowed only with other answering rule conditions\n\n\n400\nAWR-121\nBusiness
        Hours not specified for current user\n\n\n400\nAWR-170\nInvalid greeting type:
        preset with [CompanyGreeting] must be used\n\n\n400\nAWR-172\n[extension]
        must be specified for [Bypass] call handling action\n\n\n400\nAWR-173\n[extension]
        can be specified for [Bypass] call handling action only\n\n\n400\nAWR-179\n[name]
        is too long: up to 127 symbols supported\n\n\n400\nAWR-182\nOnly bypass action
        is available in multi-level IVR mode\n\n\n400\nCMN-101\nParameter [callHandlingAction]
        value is invalid"
      operationId: createCompanyAnsweringRuleInfo
      x-api-path-slug: restapiv1-0accountaccountidansweringrule-post
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
      responses:
        200:
          description: OK
      tags:
      - Company
      - Call
      - Handling
      - Rule
    get:
      summary: Get Company Call Handling Rules
      description: |-
        Returns a list of company answering rules.
        App Permission
        ReadAccounts
        User Permission
        ReadCompanyAnsweringRules
        Usage Plan Group
        Medium
      operationId: listCompanyAnsweringRule
      x-api-path-slug: restapiv1-0accountaccountidansweringrule-get
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      responses:
        200:
          description: OK
      tags:
      - Company
      - Call
      - Handling
      - Rules
  /restapi/v1.0/account/{accountId}/answering-rule/{ruleId}:
    get:
      summary: Get Company Call Handling Rule
      description: |-
        Returns a company answering rule by ID.
        App Permission
        ReadAccounts
        User Permission
        ReadCompanyAnsweringRules
        Usage Plan Group
        Light
      operationId: loadCompanyAnsweringRuleInfo
      x-api-path-slug: restapiv1-0accountaccountidansweringruleruleid-get
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: path
        name: ruleId
        description: Internal identifier of an answering rule
      responses:
        200:
          description: OK
      tags:
      - Company
      - Call
      - Handling
      - Rule
    put:
      summary: Update Company Call Handling Rule
      description: "Updates a company answering rule.\nApp Permission\nEditAccounts\nUser
        Permission\nEditCompanyAnsweringRules\nUsage Plan Group\nMedium\nError Codes\n\n
        \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nAWR-164\nRule
        type cannot be changed\n\n\n400\nAWR-170\nInvalid greeting type: preset with
        [CompanyGreeting] must be used\n\n\n400\nAWR-172\n[extension] must be specified
        for [Bypass] call handling action\n\n\n400\nAWR-173\n[extension] can be specified
        for [Bypass] call handling action only\n\n\n400\nAWR-179\n[name] is too long:
        up to 127 symbols supported\n\n\n400\nAWR-182\nOnly bypass action is available
        in multi-level IVR mode\n\n\n400\nCMN-101\nParameter [callHandlingAction]
        value is invalid"
      operationId: updateCompanyAnsweringRuleInfo
      x-api-path-slug: restapiv1-0accountaccountidansweringruleruleid-put
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
        name: ruleId
        description: Internal identifier of an answering rule
      responses:
        200:
          description: OK
      tags:
      - Company
      - Call
      - Handling
      - Rule
  /restapi/v1.0/dictionary/greeting:
    get:
      summary: Get Standard Greetings
      description: "Returns a list of predefined standard greetings. Custom greetings
        recorded by user are not returned in response to this request. See Get Extension
        Custom Greetings.\nUsage Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP
        Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter [type]
        value is invalid"
      operationId: getGreetings
      x-api-path-slug: restapiv1-0dictionarygreeting-get
      parameters:
      - in: query
        name: page
        description: Indicates the page number to retrieve
      - in: query
        name: perPage
        description: Indicates the page size (number of items)
      - in: query
        name: type
        description: Type of a greeting, specifying the case when the greeting is
          played
      - in: query
        name: usageType
        description: Usage type of a greeting, specifying if the greeting is applied
          for user extension or department extension
      responses:
        200:
          description: OK
      tags:
      - Standard
      - Greetings
  /restapi/v1.0/dictionary/greeting/{greetingId}:
    get:
      summary: Get Greeting Info
      description: "Returns a standard greeting by ID.\nUsage Plan Group\nMedium\nError
        Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n404\nCMN-102\nResource
        for parameter [greetingId] is not found"
      operationId: getGreeting
      x-api-path-slug: restapiv1-0dictionarygreetinggreetingid-get
      parameters:
      - in: path
        name: greetingId
      responses:
        200:
          description: OK
      tags:
      - Greeting
      - Info
  /restapi/v1.0/account/{accountId}/greeting:
    post:
      summary: Create Custom Company Greeting
      description: "Creates a custom company greeting.\nApp Permission\nEditAccounts\nUser
        Permission\nReadUserInfo\nUsage Plan Group\nMedium\nError Codes\n\n \n  \n
        \  HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nAWR-129\nInvalid
        attachment media type\n\n\n400\nAWR-178\nGreeting type [Voicemail] is not
        applicable to company rule\n\n\n400\nCMN-101\nParameter [type] value is invalid\n\n\n400\nCMN-102\nResource
        for parameter [answeringRule.id] is not found"
      operationId: getCompanyGreeting
      x-api-path-slug: restapiv1-0accountaccountidgreeting-post
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
      responses:
        200:
          description: OK
      tags:
      - Custom
      - Company
      - Greeting
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/greeting:
    post:
      summary: Create User Custom Greeting
      description: "Creates custom greeting for an extension user.\nApp Permission\nEditExtensions\nUser
        Permission\nEditUserAnsweringRules\nUsage Plan Group\nHeavy\nError Codes\n\n
        \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nAWR-128\nAttachment
        body is empty\n\n\n400\nAWR-129\nInvalid attachment media type\n\n\n400\nAWR-165\nHold
        music can be set for business hours rule only: the same value will be applied
        to all rules\n\n\n400\nCLR-103\nCompany level greeting cannot be created on
        user level.\n\n\n400\nCMN-101\nParameter [type] value is invalid\n\n\n400\nCMN-102\nResource
        for parameter [answeringRule.id] is not found\n\n\n400\nCMN-111\nBusiness
        operation is not supported"
      operationId: createGreeting
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidgreeting-post
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: body
        name: body
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
      - User
      - Custom
      - Greeting
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