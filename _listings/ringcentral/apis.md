---
name: RingCentral
x-slug: ringcentral
description: 'RingCentral, Inc. (NYSE: RNG) is a global provider of cloud enterprise
  unified communications and collaboration solutions. More flexible and cost-effective
  than legacy on-premise systems, RingCentral empowers today&rsquo;s mobile and distributed
  workforces to be connected anywhere and on any device through voice, video, team
  messaging, collaboration, SMS, conferencing, online meetings, contact center, and
  fax. RingCentral provides an open platform that integrates with today&rsquo;s leading
  business apps while giving customers the flexibility to customize their own workflows.'
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
x-kinRank: "7"
x-alexaRank: "7180"
tags: RingCentral
created: "2018-08-31"
modified: "2018-08-31"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/apis.md
specificationVersion: "0.14"
apis:
- name: RingCentral Connect Platform API Explorer - Get API Versions
  x-api-slug: restapi-get
  description: |-
    Returns current API version(s) and server info.
    Usage Plan Group
    NoThrottling
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapi-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapi-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Version Info
  x-api-slug: restapiapiversion-get
  description: |-
    Returns current API version info by apiVersion.
    Usage Plan Group
    NoThrottling
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiapiversion-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiapiversion-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Service status
  x-api-slug: restapiv1-0status-get
  description: |-
    Returns current PAS service status.
    Usage Plan Group
    NoThrottling
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0status-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0status-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Call Log Records by Filter
  x-api-slug: restapiv1-0accountaccountidextensionextensionidcalllog-get
  description: "Returns call log records filtered by parameters specified.\nApp Permission\nReadCallLog\nUser
    Permission\nReadCallLog\nUsage Plan Group\nHeavy\nError Codes\n\n \n  \n   HTTP
    Code\n   Error Code\n   Error Message\n   \n \n\n400\nCLG-110\nParameter [sessionId]
    is not allowed for usage along with parameter [extensionNumber]\n\n\n400\nCMN-101\nParameter
    [transport] value is invalid\n\n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-129\nAccess
    token corrupted\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n401\nOAU-213\nToken
    not found\n\n\n403\nCMN-401\nIn order to call this API endpoint, application needs
    to have [ReadCallLog] permission\n\n\n403\nCMN-408\nIn order to call this API
    endpoint, user needs to have [ReadCallLog] permission for requested resource.\n\n\n404\nCMN-102\nResource
    for parameter [extensionId] is not found\n\n\n429\nCMN-301\nRequest rate exceeded"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidcalllog-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidcalllog-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Call Records by ID
  x-api-slug: restapiv1-0accountaccountidextensionextensionidcalllogcallrecordid-get
  description: "Returns filtered call log records.\nApp Permission\nReadCallLog\nUser
    Permission\nReadCallLog\nUsage Plan Group\nHeavy\nError Codes\n\n \n  \n   HTTP
    Code\n   Error Code\n   Error Message\n   \n \n\n403\nCMN-401\nIn order to call
    this API endpoint, application needs to have [ReadCallLog] permission\n\n\n403\nCMN-408\nIn
    order to call this API endpoint, user needs to have [ReadCallLog] permission for
    requested resource.\n\n\n404\nCMN-102\nResource for parameter [extensionId] is
    not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidcalllogcallrecordid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidcalllogcallrecordid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get User Active Calls
  x-api-slug: restapiv1-0accountaccountidextensionextensionidactivecalls-get
  description: "Returns records of all extension calls that are in progress, ordered
    by start time in descending order.\nApp Permission\nReadCallLog\nUser Permission\nReadCallLog\nUsage
    Plan Group\nHeavy\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
    Message\n   \n \n\n400\nCMN-101\nParameter [direction] value is invalid\n\n\n401\nCMN-405\nLogin
    to extension required\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n403\nCMN-401\nIn
    order to call this API endpoint, application needs to have [ReadCallLog] permission\n\n\n403\nCMN-408\nIn
    order to call this API endpoint, user needs to have [ReadCallLog] permission for
    requested resource.\n\n\n404\nCMN-102\nResource for parameter [accountId] is not
    found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidactivecalls-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidactivecalls-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Call Log Records by Filter
  x-api-slug: restapiv1-0accountaccountidcalllog-get
  description: "Returns call log records filtered by parameters specified.\nApp Permission\nReadCallLog\nUser
    Permission\nFullCompanyCallLog\nUsage Plan Group\nHeavy\nError Codes\n\n \n  \n
    \  HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCLG-110\nParameter
    [sessionId] is not allowed for usage along with parameter [extensionNumber]\n\n\n400\nCMN-101\nParameter
    [dateFrom] value is invalid\n\n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-151\nAuthorization
    method not supported\n\n\n403\nCMN-401\nIn order to call this API endpoint, application
    needs to have [ReadCallLog] permission\n\n\n403\nCMN-408\nIn order to call this
    API endpoint, user needs to have [ReadCompanyCallLog] permission for requested
    resource.\n\n\n404\nCMN-102\nResource for parameter [accountId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidcalllog-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidcalllog-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Call Recordings
  x-api-slug: restapiv1-0accountaccountidrecordingrecordingid-get
  description: "Returns call recording metadata by ID.\nApp Permission\nReadCallRecording\nUser
    Permission\nReadCallRecording\nUsage Plan Group\nHeavy\nError Codes\n\n \n  \n
    \  HTTP Code\n   Error Code\n   Error Message\n   \n \n\n401\nCMN-405\nLogin to
    extension required\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n403\nCMN-401\nIn
    order to call this API endpoint, application needs to have [ReadCallRecording]
    permission\n\n\n404\nCMN-102\nResource for parameter [accountId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidrecordingrecordingid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidrecordingrecordingid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Call Recordings Data
  x-api-slug: restapiv1-0accountaccountidrecordingrecordingidcontent-get
  description: "Returns media content of a call recording.\nApp Permission\nReadCallRecording\nUser
    Permission\nReadCallRecording\nUsage Plan Group\nHeavy\nError Codes\n\n \n  \n
    \  HTTP Code\n   Error Code\n   Error Message\n   \n \n\n401\nAGW-402\nInvalid
    Authorization header\n\n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-149\nUnparsable
    access token\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n403\nCMN-401\nIn
    order to call this API endpoint, application needs to have [ReadCallRecording]
    permission\n\n\n404\nCMN-102\nResource for parameter [accountId] is not found\n\n\n416\nCMN-107\nRequested
    range not satisfiable"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidrecordingrecordingidcontent-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidrecordingrecordingidcontent-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Create SMS Message
  x-api-slug: restapiv1-0accountaccountidextensionextensionidsms-post
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidsms-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Create Pager Message
  x-api-slug: restapiv1-0accountaccountidextensionextensionidcompanypager-post
  description: "Creates and sends a pager message.\nApp Permission\nInternalMessages\nUser
    Permission\nInternalSMS\nUsage Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP
    Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter [to.phoneNumber]
    value is invalid\n\n\n400\nCMN-102\nResource for parameter [to] is not found\n\n\n400\nMSG-316\nParameter
    [to] value [102] is invalid [Target extension not found]\n\n\n400\nMSG-324\nExtension
    is of unappropriate state\n\n\n400\nMSG-331\nParameter [from] value [11111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111]
    is invalid [Sender extension number does not correspond to logged in extension]\n\n\n400\nMSG-332\nParameter
    [from] value [404544780008] is invalid [Sender extension id does not correspond
    to logged in extension]\n\n\n400\nMSG-335\nRecipient extension number does not
    correspond to ID\n\n\n403\nCMN-401\nIn order to call this API endpoint, application
    needs to have [InternalMessages] permission\n\n\n403\nCMN-408\nIn order to call
    this API endpoint, user needs to have [InternalSMS] permission for requested resource.\n\n\n403\nMSG-325\nReply
    is forbidden for old message threads\n\n\n403\nMSG-326\nReply is denied for user,
    who is no longer a thread participant\n\n\n403\nMSG-330\nSender extension is of
    unappropriate type\n\n\n404\nCMN-102\nResource for parameter [extensionId] is
    not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidcompanypager-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Create Fax Message
  x-api-slug: restapiv1-0accountaccountidextensionextensionidfax-post
  description: "Creates and sends/resends new fax message. Resend can be done if sending
    failed.\nApp Permission\nFaxes\nUser Permission\nOutboundFaxes\nUsage Plan Group\nHeavy\nError
    Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
    [to] value is invalid\n\n\n400\nMSG-344\nSending fax to extension numbers is not
    available\n\n\n400\nMSG-347\nAttachment [t.txt] body is empty\n\n\n400\nMSG-355\nFor
    binary data filename with extension should be specified, attachment [1]: []\n\n\n400\nMSG-356\nEither
    filename or content type should be specified, attachment [1]: []\n\n\n400\nMSG-365\nParameters
    [country.id] and [country.isoCode] can not be specified simultaneously\n\n\n400\nMSG-370\nfilename
    is too long, 256 characters allowed\n\n\n403\nCMN-401\nIn order to call this API
    endpoint, application needs to have [Faxes] permission\n\n\n403\nCMN-408\nIn order
    to call this API endpoint, user needs to have [OutboundFaxes] permission for requested
    resource.\n\n\n404\nCMN-102\nResource for parameter [extensionId] is not found\n\n\n415\nMSG-348\nUnsupported
    attachment media type, attachment [1]: [.jfif]\n\n\n415\nMSG-353\nNo file extension
    or content type specified, attachment [1]: [filename,txt]"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidfax-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Available Fax Cover Pages
  x-api-slug: restapiv1-0dictionaryfaxcoverpage-get
  description: "Returns fax cover pages available for the current extension.\nUsage
    Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
    Message\n   \n \n\n400\nCMN-101\nParameter [page] value is invalid\n\n\n401\nCMN-405\nLogin
    to extension required"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0dictionaryfaxcoverpage-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0dictionaryfaxcoverpage-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Message List
  x-api-slug: restapiv1-0accountaccountidextensionextensionidmessagestore-get
  description: "Returns the list of messages from an extension mailbox.\nApp Permission\nReadMessages\nUser
    Permission\nReadMessages\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP
    Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter [readStatus]
    value is invalid\n\n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-151\nAuthorization
    method not supported\n\n\n403\nCMN-401\nIn order to call this API endpoint, application
    needs to have [ReadMessages] permission\n\n\n403\nCMN-408\nIn order to call this
    API endpoint, user needs to have [ReadMessages] permission for requested resource.\n\n\n404\nCMN-102\nResource
    for parameter [extensionId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmessagestore-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Delete Conversations by ID's
  x-api-slug: restapiv1-0accountaccountidextensionextensionidmessagestore-delete
  description: "Deletes conversation(s) by conversation ID(s). Batch request is supported.\nApp
    Permission\nEditMessages\nUser Permission\nEditMessages\nUsage Plan Group\nMedium\nError
    Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
    [conversationId] value is invalid\n\n\n403\nCMN-401\nIn order to call this API
    endpoint, application needs to have [EditMessages] permission"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmessagestore-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmessagestore-delete-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Message(s) by ID
  x-api-slug: restapiv1-0accountaccountidextensionextensionidmessagestoremessageid-get
  description: "Returns individual message record(s) by the given message ID(s). The
    length of inbound messages is unlimited. Batch request is supported.\nApp Permission\nReadMessages\nUser
    Permission\nReadMessages\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP
    Code\n   Error Code\n   Error Message\n   \n \n\n401\nCMN-405\nLogin to extension
    required\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n403\nCMN-401\nIn
    order to call this API endpoint, application needs to have [ReadMessages] permission\n\n\n403\nCMN-408\nIn
    order to call this API endpoint, user needs to have [ReadMessages] permission
    for requested resource.\n\n\n404\nCMN-102\nResource for parameter [extensionId]
    is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmessagestoremessageid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Update Message(s) by ID
  x-api-slug: restapiv1-0accountaccountidextensionextensionidmessagestoremessageid-put
  description: "Updates message(s) by ID(s). Batch request is supported, see Batch
    Requests for details. Currently, only the message read status updating is supported.\nApp
    Permission\nEditMessages\nUser Permission\nEditMessages\nUsage Plan Group\nMedium\nError
    Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
    [] value is invalid\n\n\n403\nCMN-401\nIn order to call this API endpoint, application
    needs to have [EditMessages] permission\n\n\n403\nCMN-408\nIn order to call this
    API endpoint, user needs to have [EditMessages] permission for requested resource.\n\n\n404\nCMN-102\nResource
    for parameter [extensionId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmessagestoremessageid-put-openapi.md
- name: RingCentral Connect Platform API Explorer - Delete Message(s) by ID
  x-api-slug: restapiv1-0accountaccountidextensionextensionidmessagestoremessageid-delete
  description: "Deletes message(s) by the given message ID(s). The first call of this
    method transfers the message to the &#39;Delete&#39; status. The second call transfers
    the deleted message to the &#39;Purged&#39; status. If it is required to make
    the message &#39;Purged&#39; immediately (from the first call), then set the query
    parameter purge to &#39;True&#39;.\nApp Permission\nEditMessages\nUser Permission\nEditMessages\nUsage
    Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
    Message\n   \n \n\n400\nCMN-101\nParameter [purge] value is invalid\n\n\n403\nCMN-401\nIn
    order to call this API endpoint, application needs to have [EditMessages] permission\n\n\n403\nCMN-408\nIn
    order to call this API endpoint, user needs to have [EditMessages] permission
    for requested resource.\n\n\n404\nCMN-102\nResource for parameter [extensionId]
    is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmessagestoremessageid-delete-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Message Attachment
  x-api-slug: restapiv1-0accountaccountidextensionextensionidmessagestoremessageidcontentattachmentid-get
  description: "Returns a specific message attachment data as a media stream.\nApp
    Permission\nReadMessages\nUser Permission\nReadMessageContent\nUsage Plan Group\nMedium\nError
    Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n401\nAGW-402\nInvalid
    Authorization header\n\n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-149\nUnparsable
    access token\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n403\nCMN-401\nIn
    order to call this API endpoint, application needs to have [ReadMessages] permission\n\n\n403\nCMN-408\nIn
    order to call this API endpoint, user needs to have [ReadMessageContent] permission
    for requested resource.\n\n\n404\nCMN-102\nResource for parameter [extensionId]
    is not found\n\n\n416\nCMN-107\nRequested range not satisfiable"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmessagestoremessageidcontentattachmentid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmessagestoremessageidcontentattachmentid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Message Sync
  x-api-slug: restapiv1-0accountaccountidextensionextensionidmessagesync-get
  description: "Synchronizes messages.\nApp Permission\nReadMessages\nUser Permission\nReadMessages\nUsage
    Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
    Message\n   \n \n\n400\nCMN-101\nParameter [messageType] value is invalid\n\n\n400\nMSG-333\nParameter
    [syncToken] is invalid\n\n\n403\nCMN-401\nIn order to call this API endpoint,
    application needs to have [ReadMessages] permission\n\n\n403\nCMN-408\nIn order
    to call this API endpoint, user needs to have [ReadMessages] permission for requested
    resource.\n\n\n404\nCMN-102\nResource for parameter [extensionId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmessagesync-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Make RingOut Call
  x-api-slug: restapiv1-0accountaccountidextensionextensionidringout-post
  description: "Makes a 2-leg RingOut call.\nApp Permission\nRingOut\nUsage Plan Group\nHeavy\nError
    Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
    [phoneNumber] value is invalid\n\n\n400\nTEL-107\nCaller ID: [+18609411729] is
    not allowed\n\n\n400\nTEL-108\nphoneNumber specified in the from field is empty
    or invalid\n\n\n400\nTEL-109\nphoneNumber specified in the to field is empty or
    invalid\n\n\n403\nBIL-103\nFeature [RingOut] is not available for current account\n\n\n403\nCMN-112\nFeature
    [RingOut] is not available for current extension type\n\n\n403\nCMN-113\nFeature
    [DomesticCalls] is not available for current extension\n\n\n403\nRNG-102\nCaller
    ID should be one of company direct numbers\n\n\n403\nTEL-101\nphoneNumber specified
    in the to field: [17176704078] is in blocked list\n\n\n403\nTEL-102\nphoneNumber
    specified in the from field: [17176704078] is in blocked list\n\n\n403\nTEL-107\nCaller
    ID: [+12094441763] is not allowed\n\n\n404\nCMN-102\nResource for parameter [forwardingNumberId]
    is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidringout-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Status of RingOut Call
  x-api-slug: restapiv1-0accountaccountidextensionextensionidringoutringoutid-get
  description: "Returns the status of a 2-leg RingOut call.\nApp Permission\nRingOut\nUsage
    Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
    Message\n   \n \n\n503\nCMN-201\nService Temporary Unavailable"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidringoutringoutid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Cancel RingOut Call
  x-api-slug: restapiv1-0accountaccountidextensionextensionidringoutringoutid-delete
  description: "Cancels a 2-leg RingOut call.\nApp Permission\nRingOut\nUsage Plan
    Group\nHeavy\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n
    \  \n \n\n404\nCMN-102\nResource for parameter [ringOutId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidringoutringoutid-delete-openapi.md
- name: RingCentral Connect Platform API Explorer - Make RingOut Call
  x-api-slug: restapiv1-0accountaccountidextensionextensionidringout-post
  description: "Makes a 2-leg RingOut call.\nApp Permission\nRingOut\nUsage Plan Group\nHeavy\nError
    Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
    [phoneNumber] value is invalid\n\n\n400\nTEL-107\nCaller ID: [+14152961727] is
    not allowed\n\n\n400\nTEL-108\nphoneNumber specified in the from field is empty
    or invalid\n\n\n400\nTEL-109\nphoneNumber specified in the to field is empty or
    invalid\n\n\n403\nBIL-103\nFeature [RingOut] is not available for current account\n\n\n403\nCMN-112\nFeature
    [RingOut] is not available for current extension type\n\n\n403\nCMN-113\nFeature
    [DomesticCalls] is not available for current extension\n\n\n403\nCMN-401\nIn order
    to call this API endpoint, application needs to have [RingOut] permission\n\n\n403\nRNG-102\nCaller
    ID should be one of company direct numbers\n\n\n403\nTEL-101\nphoneNumber specified
    in the to field: [17176704073] is in blocked list\n\n\n403\nTEL-102\nphoneNumber
    specified in the from field: [17172302150] is in blocked list\n\n\n403\nTEL-107\nCaller
    ID: [+12094441789] is not allowed\n\n\n404\nCMN-102\nResource for parameter [extensionId]
    is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidringout-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Status of RingOut Call
  x-api-slug: restapiv1-0accountaccountidextensionextensionidringoutringoutid-get
  description: "Returns status of a 2-leg RingOut call.\nApp Permission\nRingOut\nUsage
    Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
    Message\n   \n \n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-151\nAuthorization
    method not supported\n\n\n403\nCMN-401\nIn order to call this API endpoint, application
    needs to have [RingOut] permission\n\n\n404\nCMN-102\nResource for parameter [extensionId]
    is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidringoutringoutid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Cancel RingOut Call
  x-api-slug: restapiv1-0accountaccountidextensionextensionidringoutringoutid-delete
  description: "Cancels a 2-leg RingOut call.\nApp Permission\nRingOut\nUsage Plan
    Group\nHeavy\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n
    \  \n \n\n404\nCMN-102\nResource for parameter [extensionId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidringoutringoutid-delete-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Contacts
  x-api-slug: restapiv1-0accountaccountidextensionextensionidaddressbookcontact-get
  description: "Returns user personal contacts.\nApp Permission\nReadContacts\nUser
    Permission\nReadPersonalContacts\nUsage Plan Group\nHeavy\nError Codes\n\n \n
    \ \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
    [perPage] value is invalid\n\n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-151\nAuthorization
    method not supported\n\n\n403\nCMN-401\nIn order to call this API endpoint, application
    needs to have [ReadContacts] permission\n\n\n404\nCMN-102\nResource for parameter
    [accountId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidaddressbookcontact-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidaddressbookcontact-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Create Contact
  x-api-slug: restapiv1-0accountaccountidextensionextensionidaddressbookcontact-post
  description: "Creates personal user contact.\nApp Permission\nContacts\nUser Permission\nEditPersonalContacts\nUsage
    Plan Group\nHeavy\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
    Message\n   \n \n\n400\nCMN-101\nParameter [notes] value is invalid\n\n\n400\nPAB-102\nParameter
    [assistantPhone] is invalid. Failed to parse phone number.\n\n\n400\nPAB-103\nParameter
    [assistantPhone] is invalid. The phone number is too long.\n\n\n400\nPAB-104\nParameter
    [assistantPhone] is invalid. The phone numbers starting with the asterisk are
    not supported.\n\n\n400\nPAB-105\nParameter [assistantPhone] is invalid. The extensions
    longer than 10 digits are not supported.\n\n\n400\nPAB-106\nParameter [assistantPhone]
    is invalid. The DTMF sequences longer than 64 digits are not supported.\n\n\n403\nCMN-401\nIn
    order to call this API endpoint, application needs to have [Contacts] permission\n\n\n403\nCMN-408\nIn
    order to call this API endpoint, user needs to have [EditPersonalContacts] permission
    for requested resource.\n\n\n404\nCMN-102\nResource for parameter [accountId]
    is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidaddressbookcontact-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Contact(s) by ID
  x-api-slug: restapiv1-0accountaccountidextensionextensionidaddressbookcontactcontactid-get
  description: "Returns contact(s) by ID(s). Batch request is supported.\nApp Permission\nReadContacts\nUser
    Permission\nReadPersonalContacts\nUsage Plan Group\nHeavy\nError Codes\n\n \n
    \ \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n403\nCMN-401\nIn
    order to call this API endpoint, application needs to have [ReadContacts] permission\n\n\n404\nCMN-102\nResource
    for parameter [extensionId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidaddressbookcontactcontactid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Update Contact(s) by ID
  x-api-slug: restapiv1-0accountaccountidextensionextensionidaddressbookcontactcontactid-put
  description: "Updates personal contact information by contact ID(s). Batch request
    is supported\nApp Permission\nContacts\nUser Permission\nEditPersonalContacts\nUsage
    Plan Group\nHeavy\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
    Message\n   \n \n\n400\nCMN-101\nParameter [notes] value is invalid\n\n\n403\nCMN-401\nIn
    order to call this API endpoint, application needs to have [Contacts] permission\n\n\n403\nCMN-408\nIn
    order to call this API endpoint, user needs to have [EditPersonalContacts] permission
    for requested resource.\n\n\n404\nCMN-102\nResource for parameter [extensionId]
    is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidaddressbookcontactcontactid-put-openapi.md
- name: RingCentral Connect Platform API Explorer - Delete Contact(s) by ID
  x-api-slug: restapiv1-0accountaccountidextensionextensionidaddressbookcontactcontactid-delete
  description: "Deletes contact(s) by ID(s). Batch request is supported.\nApp Permission\nContacts\nUser
    Permission\nEditPersonalContacts\nUsage Plan Group\nHeavy\nError Codes\n\n \n
    \ \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n403\nCMN-401\nIn
    order to call this API endpoint, application needs to have [Contacts] permission\n\n\n403\nCMN-408\nIn
    order to call this API endpoint, user needs to have [EditPersonalContacts] permission
    for requested resource.\n\n\n404\nCMN-102\nResource for parameter [extensionId]
    is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidaddressbookcontactcontactid-delete-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Favorite Contacts
  x-api-slug: restapiv1-0accountaccountidextensionextensionidfavorite-get
  description: "Returns favorite contacts of the current extension. Favorite contacts
    include both company contacts (extensions) and personal contacts (address book
    records).\nApp Permission\nReadContacts\nUser Permission\nReadPersonalContacts\nUsage
    Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
    Message\n   \n \n\n403\nCMN-401\nIn order to call this API endpoint, application
    needs to have [ReadContacts] permission\n\n\n403\nCMN-408\nIn order to call this
    API endpoint, user needs to have [ReadPersonalContacts] permission for requested
    resource.\n\n\n404\nCMN-102\nResource for parameter [accountId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidfavorite-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidfavorite-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Update Favorite Contacts
  x-api-slug: restapiv1-0accountaccountidextensionextensionidfavorite-put
  description: "Updates favorite contacts of the current extension. Favorite contacts
    include both company contacts (extensions) and personal contacts (address book
    records).**Please note**: currently personal address book size is limited to 10
    000 contacts.\nApp Permission\nContacts\nUser Permission\nEditPersonalContacts\nUsage
    Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
    Message\n   \n \n\n400\nCMN-101\nParameter [records.extensionId] value is invalid\n\n\n400\nFAV-100\nContact
    not found\n\n\n400\nFAV-101\nMore than one contact with the same [records.extensionId]\n\n\n400\nFAV-102\n[records.extensionId]
    and [records.contactId] could not be specified for one contact simultaneously\n\n\n400\nFAV-103\nMore
    than one contact with the same [records.id]\n\n\n400\nFAV-104\nContact limit exceeded\n\n\n400\nFAV-105\nContact
    not found in federated directory\n\n\n403\nCMN-401\nIn order to call this API
    endpoint, application needs to have [Contacts] permission\n\n\n404\nCMN-102\nResource
    for parameter [accountId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidfavorite-put-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Corporate Directory Contacts
  x-api-slug: restapiv1-0accountaccountiddirectorycontacts-get
  description: |-
    Returns contact information on corporate users of federated accounts. Please note: 1. User, DigitalUser, VirtualUser and FaxUser types are returned as User type. 2.ApplicationExtension type is not returned. 3. Only extensions in Enabled, Disabled and NotActivated state are returned.
    App Permission
    ReadAccounts
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountiddirectorycontacts-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Corporate Directory Contact
  x-api-slug: restapiv1-0accountaccountiddirectorycontactscontactid-get
  description: |-
    Returns contact information on a particular corporate user of a federated account.
    App Permission
    ReadAccounts
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountiddirectorycontactscontactid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get User Status
  x-api-slug: restapiv1-0accountaccountidextensionextensionidpresence-get
  description: "Returns presence status of an extension or several extensions by their
    ID(s). Batch request is supported. The &#39;presenceStatus&#39; is returned as
    Offline (the parameters &#39;telephonyStatus&#39;, &#39;message&#39;, &#39;userStatus&#39;
    and &#39;dndStatus&#39; are not returned at all) for the following extension types:
    Department/Announcement Only/Take Messages Only (Voicemail)/Fax User/Paging Only
    Group/Shared Lines Group/IVR Menu/Application Extension/Park Location.If the user
    requests his/her own presence status, the response contains actual presence status
    even if the status publication is turned off. Batch request is supported. For
    batch requests the number of extensions in one request is limited to 30. If more
    extensions are included in the request, the error code 400 Bad Request is returned
    with the logical error code InvalidMultipartRequest and the corresponding message
    &#39;Extension Presence Info multipart request is limited to 30 extensions&#39;.\nApp
    Permission\nReadPresence\nUser Permission\nReadPresenceStatus\nUsage Plan Group\nLight\nError
    Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n403\nCMN-408\nIn
    order to call this API endpoint, user needs to have [ReadPresenceStatus] permission
    for requested resource.\n\n\n404\nCMN-102\nResource for parameter [extensionId]
    is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidpresence-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Update User Status
  x-api-slug: restapiv1-0accountaccountidextensionextensionidpresence-put
  description: "Updates user-defined extension presence status, status message and
    DnD status by extension ID. Supported for regular User extensions only. The extension
    types listed do not support presence status: Department, Announcement Only, Take
    Messages Only (Voicemail), Fax User, Paging Only Group, Shared Lines Group, IVR
    Menu, Application Extension.\nApp Permission\nEditPresence\nUsage Plan Group\nMedium\nError
    Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
    [allowSeeMyPresence] value is invalid\n\n\n403\nBIL-103\nFeature [DND] is not
    available for current account\n\n\n403\nCMN-408\nIn order to call this API endpoint,
    user needs to have [EditPresenceSettings] permission for requested resource.\n\n\n403\nPRS-105\nNot
    allowed update presence for extensions having Disabled state\n\n\n403\nPRS-106\nNot
    allowed update presence for extensions of Department type\n\n\n404\nCMN-102\nResource
    for parameter [accountId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidpresence-put-openapi.md
- name: RingCentral Connect Platform API Explorer - Get User Groups
  x-api-slug: restapiv1-0glipgroups-get
  description: |-
    Returns the list of groups associated with the user.
    App Permission
    Glip
    User Permission
    Glip
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0glipgroups-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Create Group
  x-api-slug: restapiv1-0glipgroups-post
  description: |-
    Creates a group.
    App Permission
    Glip
    User Permission
    Glip
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0glipgroups-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Group
  x-api-slug: restapiv1-0glipgroupsgroupid-get
  description: |-
    Returns a group or multiple groups by their ID(s). Batch request is supported.
    App Permission
    Glip
    User Permission
    Glip
    Usage Plan Group
    Light
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0glipgroupsgroupid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Edit Group Members
  x-api-slug: restapiv1-0glipgroupsgroupidbulkassign-post
  description: |-
    Updates group members. Please note: Only groups of &#39;Team&#39; type can be updated. Currently only one operation at a time (either adding or removal) is supported.
    App Permission
    Glip
    User Permission
    Glip
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0glipgroupsgroupidbulkassign-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Group Posts
  x-api-slug: restapiv1-0glipgroupsgroupidposts-get
  description: |-
    Returns posts which are available for the current user (by group ID). The maximum number of posts returned is 250.
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0glipgroupsgroupidposts-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Create Post in Group
  x-api-slug: restapiv1-0glipgroupsgroupidposts-post
  description: |-
    Creates a new post in a group specified.
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0glipgroupsgroupidposts-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Update Post
  x-api-slug: restapiv1-0glipgroupsgroupidpostspostidtext-put
  description: |-
    Modifies text of a post
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0glipgroupsgroupidpostspostidtext-put-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Posts
  x-api-slug: restapiv1-0glipposts-get
  description: |-
    Returns list of posts.
    App Permission
    Glip
    User Permission
    Glip
    Usage Plan Group
    Light
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0glipposts-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Create Post
  x-api-slug: restapiv1-0glipposts-post
  description: |-
    Creates a post.
    App Permission
    Glip
    User Permission
    Glip
    Usage Plan Group
    Light
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0glipposts-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Upload File
  x-api-slug: restapiv1-0glipfiles-post
  description: |-
    Posts a file.
    App Permission
    Glip
    User Permission
    Glip
    Usage Plan Group
    Heavy
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0glipfiles-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0glipfiles-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Person
  x-api-slug: restapiv1-0glippersonspersonid-get
  description: |-
    Returns a user or multiple users by their ID(s). Batch request is supported.
    App Permission
    Glip
    User Permission
    Glip
    Usage Plan Group
    Light
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0glippersonspersonid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0glippersonspersonid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Company Info
  x-api-slug: restapiv1-0glipcompaniescompanyid-get
  description: |-
    Returns a company by ID.
    App Permission
    Glip
    User Permission
    Glip
    Usage Plan Group
    Light
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0glipcompaniescompanyid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0glipcompaniescompanyid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Create Webhook in Group
  x-api-slug: restapiv1-0glipgroupsgroupidwebhooks-post
  description: |-
    Create new Webhook
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0glipgroupsgroupidwebhooks-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Webhooks in Group
  x-api-slug: restapiv1-0glipgroupsgroupidwebhooks-get
  description: |-
    Returns webhooks which are available for the current user (by group ID).
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0glipgroupsgroupidwebhooks-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Webhooks
  x-api-slug: restapiv1-0glipwebhooks-get
  description: |-
    Returns all webhooks.
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0glipwebhooks-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Webhook
  x-api-slug: restapiv1-0glipwebhookswebhookid-get
  description: |-
    Returns webhooks(s) with the specified id(s).
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0glipwebhookswebhookid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Delete Webhook
  x-api-slug: restapiv1-0glipwebhookswebhookid-delete
  description: |-
    Deletes the webhook by ID.
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0glipwebhookswebhookid-delete-openapi.md
- name: RingCentral Connect Platform API Explorer - Activate Webhook
  x-api-slug: restapiv1-0glipwebhookswebhookidactivate-post
  description: |-
    Activates webhooks by ID.
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0glipwebhookswebhookidactivate-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Suspend Webhook
  x-api-slug: restapiv1-0glipwebhookswebhookidsuspend-post
  description: |-
    Suspends webhooks by ID.
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0glipwebhookswebhookidsuspend-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0glipwebhookswebhookidsuspend-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Scheduled Meetings [Beta]
  x-api-slug: restapiv1-0accountaccountidextensionextensionidmeeting-get
  description: |-
    Returns a list of meetings for a particular extension. The list of meetings does not include meetings of &#39;Instant&#39; type.
    App Permission
    Meetings
    User Permission
    Meetings
    Usage Plan Group
    Light
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeeting-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeeting-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Create Meetings [Beta]
  x-api-slug: restapiv1-0accountaccountidextensionextensionidmeeting-post
  description: "Creates a new meeting.\nApp Permission\nMeetings\nUser Permission\nMeetings\nUsage
    Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
    Message\n   \n \n\n400\nCMN-101\nParameter [schedule] value is invalid\n\n\n404\nCMN-102\nResource
    for parameter [extensionId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeeting-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Meeting Info [Beta]
  x-api-slug: restapiv1-0accountaccountidextensionextensionidmeetingmeetingid-get
  description: "Returns a particular meetings details by ID.\nApp Permission\nMeetings\nUser
    Permission\nMeetings\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n
    \  Error Code\n   Error Message\n   \n \n\n404\nCMN-102\nResource for parameter
    [meetingId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeetingmeetingid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeetingmeetingid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Update Meeting
  x-api-slug: restapiv1-0accountaccountidextensionextensionidmeetingmeetingid-put
  description: "Modifies a particular meeting.\nApp Permission\nMeetings\nUser Permission\nMeetings\nUsage
    Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
    Message\n   \n \n\n400\nCMN-101\nParameter [password] value is invalid\n\n\n404\nCMN-102\nResource
    for parameter [extensionId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeetingmeetingid-put-openapi.md
- name: RingCentral Connect Platform API Explorer - Delete Meeting
  x-api-slug: restapiv1-0accountaccountidextensionextensionidmeetingmeetingid-delete
  description: |-
    Deletes a scheduled meeting.
    App Permission
    Meetings
    User Permission
    Meetings
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeetingmeetingid-delete-openapi.md
- name: RingCentral Connect Platform API Explorer - End Meeting
  x-api-slug: restapiv1-0accountaccountidextensionextensionidmeetingmeetingidend-post
  description: "Ends a meetings which is in progress.\nApp Permission\nMeetings\nUser
    Permission\nMeetings\nUsage Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP
    Code\n   Error Code\n   Error Message\n   \n \n\n404\nCMN-102\nResource for parameter
    [meetingId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeetingmeetingidend-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeetingmeetingidend-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Meeting Service Info
  x-api-slug: restapiv1-0accountaccountidextensionextensionidmeetingserviceinfo-get
  description: "Returns information on dial-in numbers for meetings, support and international
    dial-in numbers URIs and meeting account information.\nApp Permission\nMeetings\nUser
    Permission\nMeetings\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n
    \  Error Code\n   Error Message\n   \n \n\n403\nCMN-401\nIn order to call this
    API endpoint, application needs to have [Meetings] permission\n\n\n403\nCMN-408\nIn
    order to call this API endpoint, user needs to have [Meetings] permission for
    requested resource."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeetingserviceinfo-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidmeetingserviceinfo-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Subscriptions
  x-api-slug: restapiv1-0subscription-get
  description: |-
    Returns a list of subscriptions created by a particular user on a particular client app.
    Usage Plan Group
    Light
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0subscription-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Create Subscription
  x-api-slug: restapiv1-0subscription-post
  description: "Creates a new subscription.\nUsage Plan Group\nMedium\nError Codes\n\n
    \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
    [deliveryMode.verificationToken] value is invalid\n\n\n400\nSUB-515\nSubscription
    containing only reminder filter is not allowed\n\n\n400\nSUB-522\nWebHook responds
    with incorrect HTTP status. HTTP status is 500\n\n\n400\nSUB-525\nWebHook server
    response is invalid\n\n\n401\nAGW-401\nAuthorization header is not specified\n\n\n401\nAGW-402\nInvalid
    Authorization header\n\n\n401\nCMN-405\nLogin to extension required\n\n\n403\nSUB-406\nNot
    allowed subscribe for events to extensions of other account\n\n\n403\nSUB-408\nNot
    allowed subscribe for unknown user\n\n\n403\nSUB-505\nSubscriptions limit exceeded\n\n\n403\nSUB-518\nNot
    allowed subscribe for favorite contacts list changes of another extension\n\n\n403\nSUB-527\nNot
    allowed subscribe for missed calls of another extension\n\n\n403\nSUB-528\n[SubscriptionAPNS]
    application permission is required for [PubNub/APNS] transport\n\n\n403\nSUB-530\nNot
    allowed subscribe for incoming calls of another extension\n\n\n403\nSUB-531\nNot
    allowed subscribe for presence of presence-lines of another extension\n\n\n404\nCMN-102\nResource
    for parameter [dashboardId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0subscription-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Subscription
  x-api-slug: restapiv1-0subscriptionsubscriptionid-get
  description: "Returns the requested subscription.\nUsage Plan Group\nLight\nError
    Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n401\nCMN-405\nLogin
    to extension required\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n404\nCMN-102\nResource
    for parameter [subscriptionId] is not found\n\n\n404\nCMN-120\nInvalid URI"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0subscriptionsubscriptionid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Renew Subscription / Update Event
    Filters
  x-api-slug: restapiv1-0subscriptionsubscriptionid-put
  description: "Renews the existent subscription if the request body is empty. If
    event filters are specified, calling this method modifies the event filters for
    the existing subscription. The client application can extend or narrow the events
    for which it receives notifications in the frame of one subscription.\nUsage Plan
    Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n
    \  \n \n\n404\nCMN-102\nResource for parameter [subscriptionId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0subscriptionsubscriptionid-put-openapi.md
- name: RingCentral Connect Platform API Explorer - Cancel Subscription
  x-api-slug: restapiv1-0subscriptionsubscriptionid-delete
  description: "Cancels the existent subscription.\nUsage Plan Group\nMedium\nError
    Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n404\nCMN-102\nResource
    for parameter [subscriptionId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0subscriptionsubscriptionid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0subscriptionsubscriptionid-delete-openapi.md
- name: RingCentral Connect Platform API Explorer - Renew Subscription
  x-api-slug: restapiv1-0subscriptionsubscriptionidrenew-post
  description: |-
    Renews an existent subscription by ID by posting request with an empty body.
    Usage Plan Group
    Light
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0subscriptionsubscriptionidrenew-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Get User Permissions
  x-api-slug: restapiv1-0accountaccountidextensionextensionidauthzprofile-get
  description: "Returns a list of user permissions granted at authorization procedure.
    Please note: Some permissions may be restricted by extension type.\nUsage Plan
    Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n
    \  \n \n\n403\nCMN-404\nAttempt to access another extension\n\n\n404\nCMN-102\nResource
    for parameter [accountId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidauthzprofile-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Check User Permissions
  x-api-slug: restapiv1-0accountaccountidextensionextensionidauthzprofilecheck-get
  description: "Checks if a certain user permission is activated for a particular
    extension.\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error
    Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter [targetExtensionId]
    value is invalid\n\n\n403\nCMN-404\nAttempt to access another extension\n\n\n404\nCMN-102\nResource
    for parameter [accountId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidauthzprofilecheck-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidauthzprofilecheck-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get User Business Hours
  x-api-slug: restapiv1-0accountaccountidextensionextensionidbusinesshours-get
  description: "Returns the extension user hours when answering rules are to be applied.\nApp
    Permission\nReadAccounts\nUser Permission\nReadExtensions\nUsage Plan Group\nLight\nError
    Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n401\nCMN-405\nLogin
    to extension required\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n403\nCMN-401\nIn
    order to call this API endpoint, application needs to have [ReadAccounts] permission\n\n\n403\nCMN-408\nIn
    order to call this API endpoint, user needs to have [ReadUserAnsweringRules] permission
    for requested resource.\n\n\n404\nCMN-102\nResource for parameter [extensionId]
    is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidbusinesshours-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidbusinesshours-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Update User Business Hours
  x-api-slug: restapiv1-0accountaccountidextensionextensionidbusinesshours-put
  description: "Updates the extension user hours when answering rules are to be applied.\nApp
    Permission\nEditExtensions\nUser Permission\nEditUserAnsweringRules\nUsage Plan
    Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n
    \  \n \n\n400\nCMN-101\nParameter [ranges] value is invalid\n\n\n403\nCMN-401\nIn
    order to call this API endpoint, application needs to have [EditExtensions] permission\n\n\n404\nCMN-102\nResource
    for parameter [extensionId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidbusinesshours-put-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Company Business Hours
  x-api-slug: restapiv1-0accountaccountidbusinesshours-get
  description: |-
    Returns company hours when answering rules are to be applied.
    App Permission
    ReadAccounts
    User Permission
    ReadUserAnsweringRules
    Usage Plan Group
    Light
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidbusinesshours-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Update Company Business Hours
  x-api-slug: restapiv1-0accountaccountidbusinesshours-put
  description: "Updates company hours when answering rules are to be applied.\nApp
    Permission\nEditExtensions\nUser Permission\nEditUserAnsweringRules\nUsage Plan
    Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n
    \  \n \n\n400\nAWR-176\nAt least one time range for [monday] required\n\n\n400\nAWR-177\nTime
    ranges limit for [monday] exceeded\n\n\n400\nCMN-101\nParameter [schedule.weeklyRanges]
    value is invalid"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidbusinesshours-put-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Blocked Numbers
  x-api-slug: restapiv1-0accountaccountidextensionextensionidblockednumber-get
  description: "Returns the list of phone numbers which are specified by the user
    to block inbound calls and SMS messages.\nApp Permission\nReadAccounts\nUser Permission\nReadBlockedNumbers\nUsage
    Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
    Message\n   \n \n\n400\nCMN-101\nParameter [perPage] value is invalid\n\n\n401\nCMN-405\nLogin
    to extension required\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n403\nCMN-401\nIn
    order to call this API endpoint, application needs to have [ReadAccounts] permission\n\n\n403\nCMN-408\nIn
    order to call this API endpoint, user needs to have [ReadBlockedNumbers] permission
    for requested resource.\n\n\n404\nCMN-102\nResource for parameter [extensionId]
    is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidblockednumber-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidblockednumber-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Add Blocked Numbers
  x-api-slug: restapiv1-0accountaccountidextensionextensionidblockednumber-post
  description: "Adds a new phone number to the blocked number list.\nApp Permission\nEditExtensions\nUser
    Permission\nEditBlockedNumbers\nUsage Plan Group\nMedium\nError Codes\n\n \n  \n
    \  HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
    [phoneNumber] value is invalid\n\n\n403\nCMN-401\nIn order to call this API endpoint,
    application needs to have [EditExtensions] permission\n\n\n403\nCMN-408\nIn order
    to call this API endpoint, user needs to have [EditBlockedNumbers] permission
    for requested resource.\n\n\n404\nCMN-102\nResource for parameter [extensionId]
    is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidblockednumber-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Blocked Number
  x-api-slug: restapiv1-0accountaccountidextensionextensionidblockednumberblockednumberid-get
  description: "Returns specific information on blocked phone number(s) by their ID(s).
    Batch request is supported.\nApp Permission\nReadAccounts\nUser Permission\nReadBlockedNumbers\nUsage
    Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
    Message\n   \n \n\n403\nCMN-401\nIn order to call this API endpoint, application
    needs to have [ReadAccounts] permission\n\n\n403\nCMN-408\nIn order to call this
    API endpoint, user needs to have [ReadBlockedNumbers] permission for requested
    resource.\n\n\n404\nCMN-102\nResource for parameter [accountId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidblockednumberblockednumberid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Update Blocked Number
  x-api-slug: restapiv1-0accountaccountidextensionextensionidblockednumberblockednumberid-put
  description: "Updates blocked number(s) by their ID(s). Currently only the name
    can be updated. Batch request is supported.\nApp Permission\nEditExtensions\nUser
    Permission\nEditBlockedNumbers\nUsage Plan Group\nMedium\nError Codes\n\n \n  \n
    \  HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
    [] value is invalid\n\n\n403\nCMN-401\nIn order to call this API endpoint, application
    needs to have [EditExtensions] permission\n\n\n403\nCMN-408\nIn order to call
    this API endpoint, user needs to have [EditBlockedNumbers] permission for requested
    resource.\n\n\n404\nCMN-102\nResource for parameter [extensionId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidblockednumberblockednumberid-put-openapi.md
- name: RingCentral Connect Platform API Explorer - Delete Blocked Number
  x-api-slug: restapiv1-0accountaccountidextensionextensionidblockednumberblockednumberid-delete
  description: "Deletes a phone number from the blocked number list. Batch request
    is supported.\nApp Permission\nEditExtensions\nUser Permission\nEditBlockedNumbers\nUsage
    Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
    Message\n   \n \n\n403\nCMN-401\nIn order to call this API endpoint, application
    needs to have [EditExtensions] permission\n\n\n403\nCMN-408\nIn order to call
    this API endpoint, user needs to have [EditBlockedNumbers] permission for requested
    resource.\n\n\n404\nCMN-102\nResource for parameter [extensionId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidblockednumberblockednumberid-delete-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Caller Blocking Settings
  x-api-slug: restapiv1-0accountaccountidextensionextensionidcallerblocking-get
  description: |-
    Returns the current call blocking settings of a user.
    App Permission
    ReadAccounts
    User Permission
    ReadBlockedNumbers
    Usage Plan Group
    Light
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidcallerblocking-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Update Caller Blocking Settings
  x-api-slug: restapiv1-0accountaccountidextensionextensionidcallerblocking-put
  description: "Updates the current call blocking settings of a user.\nApp Permission\nEditExtensions\nUser
    Permission\nEditBlockedNumbers\nUsage Plan Group\nLight\nError Codes\n\n \n  \n
    \  HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
    [greetings] value is invalid"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidcallerblocking-put-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Blocked Numbers
  x-api-slug: restapiv1-0accountaccountidextensionextensionidcallerblockingphonenumbers-get
  description: "Returns the lists of blocked and allowed phone numbers.\nApp Permission\nReadAccounts\nUser
    Permission\nReadBlockedNumbers\nUsage Plan Group\nLight\nError Codes\n\n \n  \n
    \  HTTP Code\n   Error Code\n   Error Message\n   \n \n\n404\nCMN-102\nResource
    for parameter [accountId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidcallerblockingphonenumbers-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Add Blocked Number
  x-api-slug: restapiv1-0accountaccountidextensionextensionidcallerblockingphonenumbers-post
  description: |-
    Updates either blocked or allowed phone number list with a new phone number.
    App Permission
    EditExtensions
    User Permission
    EditBlockedNumbers
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidcallerblockingphonenumbers-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Blocked Number
  x-api-slug: restapiv1-0accountaccountidextensionextensionidcallerblockingphonenumbersblockednumberid-get
  description: "Returns blocked or allowed phone number(s) by their ID(s). Batch request
    is supported.\nApp Permission\nReadAccounts\nUser Permission\nReadBlockedNumbers\nUsage
    Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
    Message\n   \n \n\n404\nCMN-102\nResource for parameter [accountId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidcallerblockingphonenumbersblockednumberid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Delete Blocked Number
  x-api-slug: restapiv1-0accountaccountidextensionextensionidcallerblockingphonenumbersblockednumberid-delete
  description: |-
    Deletes blocked or allowed phone number(s) by their ID(s). Batch request is supported.
    App Permission
    EditExtensions
    User Permission
    EditBlockedNumbers
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidcallerblockingphonenumbersblockednumberid-delete-openapi.md
- name: RingCentral Connect Platform API Explorer - Update Blocked Number
  x-api-slug: restapiv1-0accountaccountidextensionextensionidcallerblockingphonenumbersblockednumberid-put
  description: |-
    Updates blocked or allowed phone number(s) by their ID(s). Batch request is supported.
    App Permission
    EditExtensions
    User Permission
    EditBlockedNumbers
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidcallerblockingphonenumbersblockednumberid-put-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Forwarding Numbers
  x-api-slug: restapiv1-0accountaccountidextensionextensionidforwardingnumber-get
  description: "Returns the list of extension phone numbers used for call forwarding
    and call flip. The returned list contains all the extension phone numbers used
    for call forwarding and call flip.\nApp Permission\nReadAccounts\nUser Permission\nReadUserForwardingFlipNumbers\nUsage
    Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
    Message\n   \n \n\n400\nCMN-101\nParameter [perPage] value is invalid\n\n\n401\nCMN-405\nLogin
    to extension required\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n403\nCMN-401\nIn
    order to call this API endpoint, application needs to have [ReadAccounts] permission\n\n\n403\nCMN-403\nThe
    feature is not available for this extension type\n\n\n403\nCMN-408\nIn order to
    call this API endpoint, user needs to have [ReadUserForwardingFlipNumbers] permission
    for requested resource.\n\n\n404\nCMN-102\nResource for parameter [accountId]
    is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidforwardingnumber-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Create Forwarding Numbers
  x-api-slug: restapiv1-0accountaccountidextensionextensionidforwardingnumber-post
  description: "Adds a new forwarding number to the forwarding number list.\nApp Permission\nEditExtensions\nUser
    Permission\nEditUserForwardingFlipNumbers\nUsage Plan Group\nMedium\nError Codes\n\n
    \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nAWR-180\nCall
    handling settings not available for Fax tiers\n\n\n400\nCMN-101\nParameter [phoneNumber]
    value is invalid\n\n\n400\nFPN-102\nLabel of number Work duplicates with existing
    forwarding number label\n\n\n400\nFPN-103\nLimit of available forwarding numbers
    (10) exceeded\n\n\n400\nFPN-104\nLimit of available custom labeled forwarding
    numbers (7) exceeded\n\n\n400\nFPN-105\nNumber +18442015485 duplicates with company/extension
    direct number\n\n\n400\nFPN-108\nInternational calling is currently disabled\n\n\n403\nCMN-401\nIn
    order to call this API endpoint, application needs to have [EditExtensions] permission\n\n\n403\nCMN-403\nThe
    feature is not available for this extension type\n\n\n404\nCMN-102\nResource for
    parameter [extensionId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidforwardingnumber-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Forwarding Number
  x-api-slug: restapiv1-0accountaccountidextensionextensionidforwardingnumberforwardingnumberid-get
  description: "Returns a specific forwarding number.\nApp Permission\nReadAccounts\nUser
    Permission\nReadUserForwardingFlipNumbers\nUsage Plan Group\nLight\nError Codes\n\n
    \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n403\nCMN-401\nIn
    order to call this API endpoint, application needs to have [ReadAccounts] permission\n\n\n403\nCMN-403\nThe
    feature is not available for this extension type\n\n\n403\nCMN-408\nIn order to
    call this API endpoint, user needs to have [ReadUserForwardingFlipNumbers] permission
    for requested resource.\n\n\n404\nCMN-102\nResource for parameter [accountId]
    is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidforwardingnumberforwardingnumberid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Update Forwarding Numbers
  x-api-slug: restapiv1-0accountaccountidextensionextensionidforwardingnumberforwardingnumberid-put
  description: "Updates the existing forwarding number from the forwarding number
    list.\nApp Permission\nEditExtensions\nUser Permission\nEditUserForwardingFlipNumbers\nUsage
    Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
    Message\n   \n \n\n400\nCMN-101\nParameter [flipNumber] value is invalid\n\n\n400\nFPN-102\nLabel
    of number Home duplicates with existing forwarding number label\n\n\n400\nFPN-105\nNumber
    +18552050457 duplicates with company/extension direct number\n\n\n400\nFPN-106\nFlip
    number 2 is already in use\n\n\n400\nFPN-108\nInternational calling is currently
    disabled\n\n\n403\nCMN-401\nIn order to call this API endpoint, application needs
    to have [EditExtensions] permission\n\n\n403\nCMN-408\nIn order to call this API
    endpoint, user needs to have [EditUserForwardingFlipNumbers] permission for requested
    resource.\n\n\n404\nCMN-102\nResource for parameter [forwardingNumberId] is not
    found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidforwardingnumberforwardingnumberid-put-openapi.md
- name: RingCentral Connect Platform API Explorer - Delete Forwarding Number
  x-api-slug: restapiv1-0accountaccountidextensionextensionidforwardingnumberforwardingnumberid-delete
  description: "Deletes a forwarding number from the forwarding number list by its
    ID.\nApp Permission\nEditExtensions\nUser Permission\nEditUserForwardingFlipNumbers\nUsage
    Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
    Message\n   \n \n\n403\nCMN-408\nIn order to call this API endpoint, user needs
    to have [EditUserForwardingFlipNumbers] permission for requested resource.\n\n\n403\nFPN-107\nDevice
    number cannot be deleted from the forwarding number list\n\n\n404\nCMN-102\nResource
    for parameter [forwardingNumberId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidforwardingnumberforwardingnumberid-delete-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Call Handling Rules
  x-api-slug: restapiv1-0accountaccountidextensionextensionidansweringrule-get
  description: "Returns the extension answering rules.\nApp Permission\nReadAccounts\nUser
    Permission\nReadUserAnsweringRules\nUsage Plan Group\nMedium\nError Codes\n\n
    \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
    [perPage] value is invalid\n\n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-151\nAuthorization
    method not supported\n\n\n403\nCMN-401\nIn order to call this API endpoint, application
    needs to have [ReadAccounts] permission\n\n\n403\nCMN-408\nIn order to call this
    API endpoint, user needs to have [ReadUserAnsweringRules] permission for requested
    resource.\n\n\n404\nCMN-102\nResource for parameter [accountId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidansweringrule-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Create Custom Call Handling Rules
  x-api-slug: restapiv1-0accountaccountidextensionextensionidansweringrule-post
  description: "Creates a custom answering rule for a particular caller ID.\nApp Permission\nEditExtensions\nUser
    Permission\nEditUserAnsweringRules\nUsage Plan Group\nMedium\nError Codes\n\n
    \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nAWR-100\nRule
    indexes should be sequential\n\n\n400\nAWR-101\nParameter [forwarding.rules[].forwardingNumbers[].id]
    are duplicated\n\n\n400\nAWR-106\nGreeting [Voicemail] is duplicated\n\n\n400\nAWR-107\nMore
    than one caller with the same [callerId]\n\n\n400\nAWR-108\nOnly custom rule can
    be created\n\n\n400\nAWR-111\nAt least one condition should be specified\n\n\n400\nAWR-113\nMore
    than one called number with the same [calledNumbers.phoneNumber]\n\n\n400\nAWR-121\nBusiness
    Hours not specified for current user\n\n\n400\nAWR-123\nPreset [131840] can not
    be used for greeting type [Voicemail]\n\n\n400\nAWR-124\npresetId specified for
    greeting type [Voicemail] is not found\n\n\n400\nAWR-125\nCustom greeting presetId
    specified for greeting type [Introductory]. Custom greeting uploading method should
    be used\n\n\n400\nAWR-126\nThe amount of schedule ranges exceeds 1000\n\n\n400\nAWR-136\nRing
    group with index 1 is not found\n\n\n400\nAWR-137\nRule index should be greater
    than 0\n\n\n400\nAWR-138\nContact center number cannot be used as called number\n\n\n400\nAWR-139\nHold
    audio interruption period not specified\n\n\n400\nAWR-140\nHold audio interruption
    period should be empty for interruption mode specified\n\n\n400\nAWR-144\nCall
    Queue agent with index 1 is not found\n\n\n400\nAWR-147\nPreset [65792] can not
    be used for extension type [Department]\n\n\n400\nAWR-148\nCall Queue agents should
    be the same as call queue members\n\n\n400\nAWR-149\nOnly user, voicemail or shared
    line group extension can be a voicemail recipient\n\n\n400\nAWR-150\nOnly user,
    voicemail, shared line group extension or current department can be a voicemail
    recipient\n\n\n400\nAWR-152\nVoicemail cannot be turned off for call queue extension\n\n\n400\nAWR-177\nTime
    ranges limit for [monday] exceeded\n\n\n400\nAWR-179\n[name] is too long: up to
    127 symbols supported\n\n\n400\nCMN-101\nParameter [name] value is invalid\n\n\n400\nFPN-105\nNumber
    +16196093249 duplicates with company/extension direct number\n\n\n400\nFPN-108\nInternational
    calling is currently disabled\n\n\n403\nCMN-401\nIn order to call this API endpoint,
    application needs to have [EditExtensions] permission\n\n\n403\nCMN-408\nIn order
    to call this API endpoint, user needs to have [EditUserAnsweringRules] permission
    for requested resource.\n\n\n404\nCMN-102\nResource for parameter [accountId]
    is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidansweringrule-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Call Handling Rule
  x-api-slug: restapiv1-0accountaccountidextensionextensionidansweringruleruleid-get
  description: "Returns an answering rule by ID.\nApp Permission\nReadAccounts\nUser
    Permission\nReadUserAnsweringRules\nUsage Plan Group\nLight\nError Codes\n\n \n
    \ \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
    [showInactiveNumbers] value is invalid\n\n\n403\nCMN-401\nIn order to call this
    API endpoint, application needs to have [ReadAccounts] permission\n\n\n404\nCMN-102\nResource
    for parameter [answering-rule] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidansweringruleruleid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Update Custom Call Handling Rule
  x-api-slug: restapiv1-0accountaccountidextensionextensionidansweringruleruleid-put
  description: "Updates a custom answering rule for a particular caller ID.\nApp Permission\nEditExtensions\nUser
    Permission\nEditUserAnsweringRules\nUsage Plan Group\nMedium\nError Codes\n\n
    \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nAWR-100\nRule
    indexes should be sequential\n\n\n400\nAWR-106\nGreeting [Voicemail] is duplicated\n\n\n400\nAWR-111\nAt
    least one condition should be specified\n\n\n400\nAWR-113\nMore than one called
    number with the same [calledNumbers.phoneNumber]\n\n\n400\nAWR-120\nBusiness Hours/After
    Hours schedule condition is allowed only with other answering rule conditions\n\n\n400\nAWR-123\nPreset
    [131840] can not be used for greeting type [Voicemail]\n\n\n400\nAWR-124\npresetId
    specified for greeting type [Voicemail] is not found\n\n\n400\nAWR-136\nRing group
    with index 1 is not found\n\n\n400\nAWR-137\nRule index should be greater than
    0\n\n\n400\nAWR-138\nContact center number cannot be used as called number\n\n\n400\nAWR-139\nHold
    audio interruption period not specified\n\n\n400\nAWR-140\nHold audio interruption
    period should be empty for interruption mode specified\n\n\n400\nAWR-144\nCall
    Queue agent with index 1 is not found\n\n\n400\nAWR-147\nPreset [65792] can not
    be used for extension type [Department]\n\n\n400\nAWR-148\nCall Queue agents should
    be the same as call queue members\n\n\n400\nAWR-179\n[name] is too long: up to
    127 symbols supported\n\n\n400\nCMN-101\nParameter [callHandlingAction] value
    is invalid\n\n\n400\nFPN-105\nNumber +18332051179 duplicates with company/extension
    direct number\n\n\n400\nFPN-108\nInternational calling is currently disabled\n\n\n403\nCMN-401\nIn
    order to call this API endpoint, application needs to have [EditExtensions] permission\n\n\n404\nCMN-102\nResource
    for parameter [accountId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidansweringruleruleid-put-openapi.md
- name: RingCentral Connect Platform API Explorer - Delete Call Handling Rule
  x-api-slug: restapiv1-0accountaccountidextensionextensionidansweringruleruleid-delete
  description: "Deletes a custom answering rule by a particular ID.\nApp Permission\nEditExtensions\nUser
    Permission\nEditUserAnsweringRules\nUsage Plan Group\nMedium\nError Codes\n\n
    \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n403\nAWR-110\nBusiness
    Hours/After Hours rule cannot be deleted\n\n\n403\nCMN-401\nIn order to call this
    API endpoint, application needs to have [EditExtensions] permission\n\n\n403\nCMN-408\nIn
    order to call this API endpoint, user needs to have [EditUserAnsweringRules] permission
    for requested resource.\n\n\n404\nCMN-102\nResource for parameter [answering-rule]
    is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidansweringruleruleid-delete-openapi.md
- name: RingCentral Connect Platform API Explorer - Create Company Call Handling Rule
  x-api-slug: restapiv1-0accountaccountidansweringrule-post
  description: "Creates a company answering rule for a particular caller ID.\nApp
    Permission\nEditAccounts\nUser Permission\nEditCompanyAnsweringRules\nUsage Plan
    Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n
    \  \n \n\n400\nAWR-106\nGreeting [Company] is duplicated\n\n\n400\nAWR-108\nOnly
    custom rule can be created\n\n\n400\nAWR-120\nBusiness Hours/After Hours schedule
    condition is allowed only with other answering rule conditions\n\n\n400\nAWR-121\nBusiness
    Hours not specified for current user\n\n\n400\nAWR-170\nInvalid greeting type:
    preset with [CompanyGreeting] must be used\n\n\n400\nAWR-172\n[extension] must
    be specified for [Bypass] call handling action\n\n\n400\nAWR-173\n[extension]
    can be specified for [Bypass] call handling action only\n\n\n400\nAWR-179\n[name]
    is too long: up to 127 symbols supported\n\n\n400\nAWR-182\nOnly bypass action
    is available in multi-level IVR mode\n\n\n400\nCMN-101\nParameter [callHandlingAction]
    value is invalid"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidansweringrule-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Company Call Handling Rules
  x-api-slug: restapiv1-0accountaccountidansweringrule-get
  description: |-
    Returns a list of company answering rules.
    App Permission
    ReadAccounts
    User Permission
    ReadCompanyAnsweringRules
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidansweringrule-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Company Call Handling Rule
  x-api-slug: restapiv1-0accountaccountidansweringruleruleid-get
  description: |-
    Returns a company answering rule by ID.
    App Permission
    ReadAccounts
    User Permission
    ReadCompanyAnsweringRules
    Usage Plan Group
    Light
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidansweringruleruleid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Update Company Call Handling Rule
  x-api-slug: restapiv1-0accountaccountidansweringruleruleid-put
  description: "Updates a company answering rule.\nApp Permission\nEditAccounts\nUser
    Permission\nEditCompanyAnsweringRules\nUsage Plan Group\nMedium\nError Codes\n\n
    \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nAWR-164\nRule
    type cannot be changed\n\n\n400\nAWR-170\nInvalid greeting type: preset with [CompanyGreeting]
    must be used\n\n\n400\nAWR-172\n[extension] must be specified for [Bypass] call
    handling action\n\n\n400\nAWR-173\n[extension] can be specified for [Bypass] call
    handling action only\n\n\n400\nAWR-179\n[name] is too long: up to 127 symbols
    supported\n\n\n400\nAWR-182\nOnly bypass action is available in multi-level IVR
    mode\n\n\n400\nCMN-101\nParameter [callHandlingAction] value is invalid"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidansweringruleruleid-put-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Standard Greetings
  x-api-slug: restapiv1-0dictionarygreeting-get
  description: "Returns a list of predefined standard greetings. Custom greetings
    recorded by user are not returned in response to this request. See Get Extension
    Custom Greetings.\nUsage Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n
    \  Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter [type] value
    is invalid"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0dictionarygreeting-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Greeting Info
  x-api-slug: restapiv1-0dictionarygreetinggreetingid-get
  description: "Returns a standard greeting by ID.\nUsage Plan Group\nMedium\nError
    Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n404\nCMN-102\nResource
    for parameter [greetingId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0dictionarygreetinggreetingid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0dictionarygreetinggreetingid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Create Custom Company Greeting
  x-api-slug: restapiv1-0accountaccountidgreeting-post
  description: "Creates a custom company greeting.\nApp Permission\nEditAccounts\nUser
    Permission\nReadUserInfo\nUsage Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP
    Code\n   Error Code\n   Error Message\n   \n \n\n400\nAWR-129\nInvalid attachment
    media type\n\n\n400\nAWR-178\nGreeting type [Voicemail] is not applicable to company
    rule\n\n\n400\nCMN-101\nParameter [type] value is invalid\n\n\n400\nCMN-102\nResource
    for parameter [answeringRule.id] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidgreeting-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Create User Custom Greeting
  x-api-slug: restapiv1-0accountaccountidextensionextensionidgreeting-post
  description: "Creates custom greeting for an extension user.\nApp Permission\nEditExtensions\nUser
    Permission\nEditUserAnsweringRules\nUsage Plan Group\nHeavy\nError Codes\n\n \n
    \ \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nAWR-128\nAttachment
    body is empty\n\n\n400\nAWR-129\nInvalid attachment media type\n\n\n400\nAWR-165\nHold
    music can be set for business hours rule only: the same value will be applied
    to all rules\n\n\n400\nCLR-103\nCompany level greeting cannot be created on user
    level.\n\n\n400\nCMN-101\nParameter [type] value is invalid\n\n\n400\nCMN-102\nResource
    for parameter [answeringRule.id] is not found\n\n\n400\nCMN-111\nBusiness operation
    is not supported"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidgreeting-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Custom Greeting Info
  x-api-slug: restapiv1-0accountaccountidextensionextensionidgreetinggreetingid-get
  description: "Returns a custom user greeting by ID.\nApp Permission\nReadAccounts\nUser
    Permission\nReadUserInfo\nUsage Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP
    Code\n   Error Code\n   Error Message\n   \n \n\n404\nCMN-102\nResource for parameter
    [greetingId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidgreetinggreetingid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidgreetinggreetingid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get IVR Prompts
  x-api-slug: restapiv1-0accountaccountidivrprompts-get
  description: "Returns a list of IVR prompts.\nApp Permission\nReadAccounts\nUser
    Permission\nReadCompanyGreetings\nUsage Plan Group\nMedium\nError Codes\n\n \n
    \ \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n403\nCMN-401\nIn
    order to call this API endpoint, application needs to have [ReadAccounts] permission\n\n\n403\nCMN-408\nIn
    order to call this API endpoint, user needs to have [ReadCompanyGreetings] permission
    for requested resource."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidivrprompts-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get IVR Prompt
  x-api-slug: restapiv1-0accountaccountidivrpromptspromptid-get
  description: "Returns an IVR prompt by ID.\nApp Permission\nReadAccounts\nUser Permission\nReadCompanyGreetings\nUsage
    Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
    Message\n   \n \n\n403\nCMN-401\nIn order to call this API endpoint, application
    needs to have [ReadAccounts] permission\n\n\n403\nCMN-408\nIn order to call this
    API endpoint, user needs to have [ReadCompanyGreetings] permission for requested
    resource.\n\n\n404\nCMN-102\nResource for parameter [promptId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidivrpromptspromptid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Delete IVR Prompt
  x-api-slug: restapiv1-0accountaccountidivrpromptspromptid-delete
  description: |-
    Deletes an IVR prompt by ID.
    App Permission
    EditAccounts
    User Permission
    EditCompanyGreetings
    Usage Plan Group
    Heavy
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidivrpromptspromptid-delete-openapi.md
- name: RingCentral Connect Platform API Explorer - Get IVR Prompt Content
  x-api-slug: restapiv1-0accountaccountidivrpromptspromptidcontent-get
  description: |-
    Returns media content of an IVR prompt by ID.
    App Permission
    ReadAccounts
    User Permission
    ReadCompanyGreetings
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidivrpromptspromptidcontent-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidivrpromptspromptidcontent-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get IVR Menu
  x-api-slug: restapiv1-0accountaccountidivrmenusivrmenuid-get
  description: |-
    Returns a company IVR menu by ID.
    App Permission
    ReadAccounts
    User Permission
    AutoReceptionist
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidivrmenusivrmenuid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Call Recording Settings
  x-api-slug: restapiv1-0accountaccountidcallrecording-get
  description: |-
    Returns call recording settings.
    App Permission
    ReadAccounts
    User Permission
    ReadCompanyInfo
    Usage Plan Group
    Light
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidcallrecording-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Call Recording Extension Settings
  x-api-slug: restapiv1-0accountaccountidcallrecordingextensions-get
  description: |-
    Returns the list of extensions to be recorded.
    App Permission
    ReadAccounts
    User Permission
    ReadCompanyInfo
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidcallrecordingextensions-get-openapi.md
- name: RingCentral Connect Platform API Explorer - [Beta] Get Call Recording Custom
    Greetings
  x-api-slug: restapiv1-0accountaccountidcallrecordingcustomgreetings-get
  description: |-
    Returns call recording custom greetings.
    App Permission
    ReadAccounts
    User Permission
    ReadCompanyInfo
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidcallrecordingcustomgreetings-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Register SIP Device
  x-api-slug: restapiv1-0clientinfosipprovision-post
  description: "Creates SIP registration of a device/application (WebPhone, Mobile,
    softphone)\nApp Permission\nVoipCalling\nUsage Plan Group\nHeavy\nError Codes\n\n
    \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
    [sipInfo.transport] value is invalid\n\n\n400\nSPR-114\nDevice id length [40]
    is greater than allowed [38]\n\n\n400\nSPR-118\nParameter [device.id]=@1qwbc)yppa!
    is not a number\n\n\n400\nSPR-129\nNot allowed to register with incompatible protocol
    list [WS, TCP]\n\n\n400\nSPR-130\ndevice is not allowed for WebRTC.\n\n\n403\nBIL-103\nFeature
    [WebPhone] is not available for current account\n\n\n403\nCMN-401\nIn order to
    call this API endpoint, application needs to have [VoipCalling] permission\n\n\n403\nCMN-402\nAdministrator
    permission required\n\n\n403\nSPR-112\nClient edition is not compatible with current
    Brand\n\n\n403\nSPR-122\nApplication version is not set in \"User-Agent\" header
    or not parseable"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0clientinfosipprovision-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Extension Phone Number List
  x-api-slug: restapiv1-0accountaccountidextensionextensionidphonenumber-get
  description: "Returns the list of phone numbers that are used by a particular extension,
    and can be filtered by the phone number type. The returned list contains all numbers
    which are directly mapped to a given extension plus the features and also company-level
    numbers which may be used when performing different operations on behalf of this
    extension.\nApp Permission\nReadAccounts\nUser Permission\nReadUserPhoneNumbers\nUsage
    Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
    Message\n   \n \n\n400\nCMN-101\nParameter [usageType] value is invalid\n\n\n401\nCMN-405\nLogin
    to extension required\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n403\nCMN-401\nIn
    order to call this API endpoint, application needs to have [ReadAccounts] permission\n\n\n404\nCMN-102\nResource
    for parameter [extensionId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidphonenumber-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Extension Info
  x-api-slug: restapiv1-0accountaccountidextensionextensionid-get
  description: "Returns basic information about a particular extension of an account.\nApp
    Permission\nReadAccounts\nUser Permission\nReadExtensions\nUsage Plan Group\nLight\nError
    Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n401\nCMN-405\nLogin
    to extension required\n\n\n401\nOAU-129\nAccess token corrupted\n\n\n401\nOAU-151\nAuthorization
    method not supported\n\n\n403\nCMN-401\nIn order to call this API endpoint, application
    needs to have [ReadAccounts] permission\n\n\n404\nCMN-102\nResource for parameter
    [extensionId] is not found\n\n\n429\nCMN-301\nRequest rate exceeded"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Extension Caller ID
  x-api-slug: restapiv1-0accountaccountidextensionextensionidcallerid-get
  description: |-
    Returns information on an outbound caller ID of an extension.
    App Permission
    ReadAccounts
    User Permission
    ReadCallerIDSettings
    Usage Plan Group
    Light
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidcallerid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Update Extension Caller ID
  x-api-slug: restapiv1-0accountaccountidextensionextensionidcallerid-put
  description: "Updates outbound caller ID information of an extension.\nApp Permission\nEditExtensions\nUser
    Permission\nEditCallerIDSettings\nUsage Plan Group\nMedium\nError Codes\n\n \n
    \ \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
    [byFeature.callerId.type] value is invalid\n\n\n400\nCMN-102\nResource for parameter
    [phoneInfo.id] is not found\n\n\n403\nCID-101\nFeature [CommonPhone] is not available
    for current account.\n\n\n403\nCID-102\nContact center phone number cannot be
    set as caller ID: Contact Center is not available for current account.\n\n\n403\nCID-103\nConferencing
    phone number cannot be set as caller ID."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidcallerid-put-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Extension Grants
  x-api-slug: restapiv1-0accountaccountidextensionextensionidgrant-get
  description: "Returns the list of extension grants.\nApp Permission\nReadAccounts\nUser
    Permission\nReadExtensions\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP
    Code\n   Error Code\n   Error Message\n   \n \n\n401\nCMN-405\nLogin to extension
    required\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n403\nCMN-408\nIn
    order to call this API endpoint, user needs to have [ReadExtensionGrant] permission
    for requested resource.\n\n\n404\nCMN-102\nResource for parameter [accountId]
    is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidgrant-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidgrant-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Notification Settings
  x-api-slug: restapiv1-0accountaccountidextensionextensionidnotificationsettings-get
  description: "Returns notification settings for the current extension.\nApp Permission\nReadAccounts\nUser
    Permission\nReadMessagesNotificationsSettings\nUsage Plan Group\nLight\nError
    Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n403\nCMN-401\nIn
    order to call this API endpoint, application needs to have [ReadAccounts] permission\n\n\n403\nCMN-408\nIn
    order to call this API endpoint, user needs to have [ReadMessagesNotificationsSettings]
    permission for requested resource."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidnotificationsettings-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Update Notification Settings
  x-api-slug: restapiv1-0accountaccountidextensionextensionidnotificationsettings-put
  description: "Updates notification settings for the current extension.\nApp Permission\nEditExtensions\nUser
    Permission\nEditMessagesNotificationsSettings\nUsage Plan Group\nMedium\nError
    Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n403\nCMN-109\nFeature
    VoicemailToText is unavailable\n\n\n403\nCMN-401\nIn order to call this API endpoint,
    application needs to have [EditExtensions] permission"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidnotificationsettings-put-openapi.md
- name: RingCentral Connect Platform API Explorer - Get User Profile Image
  x-api-slug: restapiv1-0accountaccountidextensionextensionidprofileimage-get
  description: "Returns a profile image of an extension.\nApp Permission\nReadAccounts\nUser
    Permission\nReadExtensions\nUsage Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP
    Code\n   Error Code\n   Error Message\n   \n \n\n401\nAGW-401\nAuthorization header
    is not specified\n\n\n401\nAGW-402\nInvalid Authorization header\n\n\n403\nCMN-109\nFeature
    Profile Image Streaming is unavailable\n\n\n403\nCMN-401\nIn order to call this
    API endpoint, application needs to have [ReadAccounts] permission\n\n\n404\nCMN-102\nResource
    for parameter [extensionId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidprofileimage-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Upload User Profile Image
  x-api-slug: restapiv1-0accountaccountidextensionextensionidprofileimage-post
  description: "Returns the extension profile image.\nApp Permission\nEditExtensions\nUser
    Permission\nEditUserInfo\nUsage Plan Group\nHeavy\nError Codes\n\n \n  \n   HTTP
    Code\n   Error Code\n   Error Message\n   \n \n\n403\nCMN-401\nIn order to call
    this API endpoint, application needs to have [EditExtensions] permission"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidprofileimage-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Update User Profile Image
  x-api-slug: restapiv1-0accountaccountidextensionextensionidprofileimage-put
  description: "Updates profile image of an extension.\nApp Permission\nEditExtensions\nUser
    Permission\nEditUserInfo\nUsage Plan Group\nHeavy\nError Codes\n\n \n  \n   HTTP
    Code\n   Error Code\n   Error Message\n   \n \n\n400\nACT-331\nProfile image not
    valid\n\n\n400\nACT-334\nProfile image file is more than 12 megapixel\n\n\n400\nCMN-101\nParameter
    [image] value is invalid\n\n\n403\nACT-332\nProfile image could not be set for
    an extension in unassigned status\n\n\n403\nCMN-401\nIn order to call this API
    endpoint, application needs to have [EditExtensions] permission\n\n\n403\nCMN-408\nIn
    order to call this API endpoint, user needs to have [EditUserInfo] permission
    for requested resource.\n\n\n404\nCMN-102\nResource for parameter [accountId]
    is not found\n\n\n415\nACT-330\nUnsupported image content type"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidprofileimage-put-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Extension Profile Image (Scaled)
  x-api-slug: restapiv1-0accountaccountidextensionextensionidprofileimagescalesize-get
  description: "Returns profile image of an extension.\nApp Permission\nReadAccounts\nUser
    Permission\nReadExtensions\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP
    Code\n   Error Code\n   Error Message\n   \n \n\n404\nACT-333\nProfile image is
    not found for scale size [92]"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidprofileimagescalesize-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get User Conferencing Settings
  x-api-slug: restapiv1-0accountaccountidextensionextensionidconferencing-get
  description: "Returns the information on the Free Conference Calling (FCC) feature
    for a given extension.\nApp Permission\nReadAccounts\nUser Permission\nOrganizeConference\nUsage
    Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
    Message\n   \n \n\n403\nCMN-112\nFeature [Conferencing] is not available for current
    extension type\n\n\n403\nCMN-408\nIn order to call this API endpoint, user needs
    to have [OrganizeConference] permission for requested resource.\n\n\n404\nCMN-102\nResource
    for parameter [accountId] is not found\n\n\n503\nFCC-103\nConference group is
    not set for current account"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidconferencing-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Update User Conferencing Settings
  x-api-slug: restapiv1-0accountaccountidextensionextensionidconferencing-put
  description: "Updates the default conferencing number for the current extension.
    The number can be selected from conferencing numbers of the current extension.
    Updates the setting, allowing participants join the conference before host.\nApp
    Permission\nEditExtensions\nUser Permission\nOrganizeConference\nUsage Plan Group\nMedium\nError
    Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
    [allowJoinBeforeHost, phoneNumbers] value is invalid\n\n\n403\nCMN-408\nIn order
    to call this API endpoint, user needs to have [OrganizeConference] permission
    for requested resource.\n\n\n404\nCMN-102\nResource for parameter [accountId]
    is not found\n\n\n503\nCMN-201\nService Temporary Unavailable"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextensionextensionidconferencing-put-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Company Info
  x-api-slug: restapiv1-0accountaccountid-get
  description: "Returns basic information about a particular RingCentral customer
    account.\nApp Permission\nReadAccounts\nUser Permission\nReadCompanyInfo\nUsage
    Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
    Message\n   \n \n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-151\nAuthorization
    method not supported\n\n\n401\nOAU-213\nToken not found\n\n\n403\nCMN-401\nIn
    order to call this API endpoint, application needs to have [ReadAccounts] permission\n\n\n404\nCMN-102\nResource
    for parameter [accountId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Company Business Address
  x-api-slug: restapiv1-0accountaccountidbusinessaddress-get
  description: "Returns business address of a company.\nApp Permission\nReadAccounts\nUser
    Permission\nReadCompanyInfo\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP
    Code\n   Error Code\n   Error Message\n   \n \n\n401\nCMN-405\nLogin to extension
    required\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n403\nCMN-401\nIn
    order to call this API endpoint, application needs to have [ReadAccounts] permission\n\n\n404\nCMN-102\nResource
    for parameter [accountId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidbusinessaddress-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Language List
  x-api-slug: restapiv1-0dictionarylanguage-get
  description: "Returns the information about supported languages.\nUsage Plan Group\nLight\nError
    Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
    [perPage] value is invalid"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0dictionarylanguage-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Language
  x-api-slug: restapiv1-0dictionarylanguagelanguageid-get
  description: "Returns language by ID.\nUsage Plan Group\nLight\nError Codes\n\n
    \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n404\nCMN-102\nResource
    for parameter [languageId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0dictionarylanguagelanguageid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Country List
  x-api-slug: restapiv1-0dictionarycountry-get
  description: "Returns all the countries available for calling.\nUsage Plan Group\nLight\nError
    Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
    [perPage] value is invalid\n\n\n401\nAGW-401\nAuthorization header is not specified\n\n\n401\nOAU-129\nAccess
    token corrupted"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0dictionarycountry-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0dictionarycountry-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Country
  x-api-slug: restapiv1-0dictionarycountrycountryid-get
  description: "Returns the information on a specific country.\nUsage Plan Group\nLight\nError
    Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-122\nMethod
    is brand specific\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n404\nCMN-102\nResource
    for parameter [countryId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0dictionarycountrycountryid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0dictionarycountrycountryid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Location List
  x-api-slug: restapiv1-0dictionarylocation-get
  description: "Returns all available locations for a certain state.\nUsage Plan Group\nLight\nError
    Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
    [orderBy] value is invalid\n\n\n404\nCMN-102\nResource for parameter [location]
    is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0dictionarylocation-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0dictionarylocation-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get State List
  x-api-slug: restapiv1-0dictionarystate-get
  description: "Returns all the states of a certain country\nUsage Plan Group\nLight\nError
    Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
    [perPage] value is invalid\n\n\n404\nCMN-102\nResource for parameter [stateId]
    is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0dictionarystate-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get State
  x-api-slug: restapiv1-0dictionarystatestateid-get
  description: "Returns the information on a specific state.\nUsage Plan Group\nLight\nError
    Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n404\nCMN-102\nResource
    for parameter [stateId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0dictionarystatestateid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Timezone List
  x-api-slug: restapiv1-0dictionarytimezone-get
  description: "Returns all available timezones.\nUsage Plan Group\nLight\nError Codes\n\n
    \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
    [perPage] value is invalid"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0dictionarytimezone-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0dictionarytimezone-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Timezone
  x-api-slug: restapiv1-0dictionarytimezonetimezoneid-get
  description: "Returns the information on a certain timezone.\nUsage Plan Group\nLight\nError
    Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n404\nCMN-102\nResource
    for parameter [timezoneId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0dictionarytimezonetimezoneid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0dictionarytimezonetimezoneid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get All Company Phone Numbers
  x-api-slug: restapiv1-0accountaccountidphonenumber-get
  description: "Returns the list of phone numbers assigned to RingCentral customer
    account. Both company-level and extension-level numbers are returned.\nApp Permission\nReadAccounts\nUser
    Permission\nReadCompanyPhoneNumbers\nUsage Plan Group\nHeavy\nError Codes\n\n
    \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
    [perPage] value is invalid\n\n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-151\nAuthorization
    method not supported\n\n\n403\nCMN-401\nIn order to call this API endpoint, application
    needs to have [ReadAccounts] permission\n\n\n404\nCMN-102\nResource for parameter
    [accountId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidphonenumber-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Phone Number
  x-api-slug: restapiv1-0accountaccountidphonenumberphonenumberid-get
  description: "Returns the phone number(s) belonging to a certain account or extension
    by phoneNumberId(s). Batch request is supported.\nApp Permission\nReadAccounts\nUser
    Permission\nReadCompanyPhoneNumbers\nUsage Plan Group\nLight\nError Codes\n\n
    \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n403\nCMN-401\nIn
    order to call this API endpoint, application needs to have [ReadAccounts] permission\n\n\n404\nCMN-102\nResource
    for parameter [accountId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidphonenumberphonenumberid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Extensions
  x-api-slug: restapiv1-0accountaccountidextension-get
  description: "Returns the list of extensions created for a particular account. All
    types of extensions are included in this list.\nApp Permission\nReadAccounts\nUser
    Permission\nReadExtensions\nUsage Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP
    Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter [status]
    value is invalid\n\n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-151\nAuthorization
    method not supported\n\n\n403\nCMN-401\nIn order to call this API endpoint, application
    needs to have [ReadAccounts] permission\n\n\n404\nCMN-102\nResource for parameter
    [accountId] is not found\n\n\n429\nCMN-301\nRequest rate exceeded"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidextension-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Department Member List
  x-api-slug: restapiv1-0accountaccountiddepartmentdepartmentidmembers-get
  description: "[Deprecated] Viewing user account info (including name, business name,
    address and phone number/account number)\nApp Permission\nReadAccounts\nUser Permission\nReadExtensions\nUsage
    Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
    Message\n   \n \n\n400\nCMN-101\nParameter [page] value is invalid\n\n\n401\nCMN-405\nLogin
    to extension required\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n403\nCMN-401\nIn
    order to call this API endpoint, application needs to have [ReadAccounts] permission\n\n\n404\nCMN-102\nResource
    for parameter [departmentId] is not found"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountiddepartmentdepartmentidmembers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountiddepartmentdepartmentidmembers-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Edit Call Queue Members
  x-api-slug: restapiv1-0accountaccountiddepartmentbulkassign-post
  description: "[Deprecated] Adds and/or removes multiple call queue members\nApp
    Permission\nEditAccounts\nUser Permission\nUserGroups\nUsage Plan Group\nHeavy\nError
    Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nEXT-401\nExtension
    ID should be present only in one section"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountiddepartmentbulkassign-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Paging Only Group Users
  x-api-slug: restapiv1-0accountaccountidpagingonlygroupspagingonlygroupidusers-get
  description: "Returns the list of users allowed to page this group.\nApp Permission\nReadAccounts\nUser
    Permission\nReadUserInfo\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP
    Code\n   Error Code\n   Error Message\n   \n \n\n403\nCMN-401\nIn order to call
    this API endpoint, application needs to have [ReadAccounts] permission"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidpagingonlygroupspagingonlygroupidusers-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Paging Only Group Devices
  x-api-slug: restapiv1-0accountaccountidpagingonlygroupspagingonlygroupiddevices-get
  description: "Returns the list of paging devices assigned to this group.\nApp Permission\nReadAccounts\nUser
    Permission\nReadCompanyDevices\nUsage Plan Group\nLight\nError Codes\n\n \n  \n
    \  HTTP Code\n   Error Code\n   Error Message\n   \n \n\n403\nCMN-401\nIn order
    to call this API endpoint, application needs to have [ReadAccounts] permission"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidpagingonlygroupspagingonlygroupiddevices-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Edit Paging Group Users and Devices
  x-api-slug: restapiv1-0accountaccountidpagingonlygroupspagingonlygroupidbulkassign-post
  description: "Adds and/or removes paging group users and devices.\nApp Permission\nEditAccounts\nUser
    Permission\nEditUserInfo\nUsage Plan Group\nHeavy\nError Codes\n\n \n  \n   HTTP
    Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter [addedDeviceIds]
    value is invalid\n\n\n403\nCMN-401\nIn order to call this API endpoint, application
    needs to have [EditAccounts] permission"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidpagingonlygroupspagingonlygroupidbulkassign-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Call Queues
  x-api-slug: restapiv1-0accountaccountidcallqueues-get
  description: |-
    Returns call queue group list
    App Permission
    ReadAccounts
    User Permission
    ReadExtensions
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidcallqueues-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Call Queue Members
  x-api-slug: restapiv1-0accountaccountidcallqueuesgroupidmembers-get
  description: |-
    Returns call queue group members.
    App Permission
    ReadAccounts
    User Permission
    ReadExtensions
    Usage Plan Group
    Light
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidcallqueuesgroupidmembers-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Edit Call Queue Group
  x-api-slug: restapiv1-0accountaccountidcallqueuesgroupidbulkassign-post
  description: "Updates call queue group.\nApp Permission\nEditExtensions\nUser Permission\nGroups\nUsage
    Plan Group\nHeavy\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
    Message\n   \n \n\n400\nEXT-405\nExtension of type [ParkLocation] could not be
    a member of [department}]"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidcallqueuesgroupidbulkassign-post-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Call Monitoring Groups
  x-api-slug: restapiv1-0accountaccountidcallmonitoringgroups-get
  description: |-
    Returns call monitoring groups that can be filtered by some extension.
    App Permission
    ReadAccounts
    User Permission
    ReadExtensions
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidcallmonitoringgroups-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Get Call Monitoring Group Members
  x-api-slug: restapiv1-0accountaccountidcallmonitoringgroupsgroupidmembers-get
  description: |-
    Returns call monitoring group members.
    App Permission
    ReadAccounts
    User Permission
    ReadExtensions
    Usage Plan Group
    Medium
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0accountaccountidcallmonitoringgroupsgroupidmembers-get-openapi.md
- name: RingCentral Connect Platform API Explorer - Parse Phone Number [Beta]
  x-api-slug: restapiv1-0numberparserparse-post
  description: "Returns one or more parsed and/or formatted phone numbers that are
    passed as a string.\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n
    \  Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter [nationalAsPriority]
    value is invalid"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/restapiv1-0numberparserparse-post-openapi.md
- name: RingCentral Connect Platform API Explorer - get service provider config
  x-api-slug: scimv2serviceproviderconfig-get
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/scimv2serviceproviderconfig-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/scimv2serviceproviderconfig-get-openapi.md
- name: RingCentral Connect Platform API Explorer - search or list users
  x-api-slug: scimv2users-get
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/scimv2users-get-openapi.md
- name: RingCentral Connect Platform API Explorer - create a user
  x-api-slug: scimv2users-post
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/scimv2users-post-openapi.md
- name: RingCentral Connect Platform API Explorer - search or list users
  x-api-slug: scimv2users-search-post
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/scimv2users-search-post-openapi.md
- name: RingCentral Connect Platform API Explorer - get a user by id
  x-api-slug: scimv2usersid-get
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/scimv2usersid-get-openapi.md
- name: RingCentral Connect Platform API Explorer - fully update/replace a user
  x-api-slug: scimv2usersid-put
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/scimv2usersid-put-openapi.md
- name: RingCentral Connect Platform API Explorer - delete a user
  x-api-slug: scimv2usersid-delete
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28867-developer-ringcentral-com.jpg
  humanURL: http://www.ringcentral.com
  baseURL: https://platform.ringcentral.com//
  tags: Telecommunications, ISP, Voice, Video Conferencing, Webinars, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/ringcentral/master/_listings/ringcentral/scimv2usersid-delete-openapi.md
x-common:
- type: x-blog
  url: https://medium.com/ringcentral-developers
- type: x-blog-rss
  url: https://medium.com/feed/ringcentral-developers
- type: x-github
  url: https://github.com/ringcentral
- type: x-openapi
  url: https://netstorage.ringcentral.com/dpw/api-explorer/swagger-ring_basic.yml?v=20180816
- type: x-website
  url: http://www.ringcentral.com
- type: x-api-gallery
  url: http://reverb.api.gallery.streamdata.io
- type: x-api-stack
  url: http://ringcentral.stack.network
- type: x-code
  url: https://developer.ringcentral.com/library/sdks.html
- type: x-crunchbase
  url: https://crunchbase.com/organization/ringcentral
- type: x-developer
  url: https://developer.ringcentral.com/
- type: x-documentation
  url: https://developer.ringcentral.com/api-explorer/latest/index.html?_ga=2.259782990.551967760.1534465156-1236351744.1533920460
- type: x-support
  url: https://developer.ringcentral.com/support.html
- type: x-twitter
  url: https://twitter.com/RingCentral
- type: x-website
  url: https://developer.ringcentral.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---