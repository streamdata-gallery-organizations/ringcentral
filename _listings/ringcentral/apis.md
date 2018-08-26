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
created: "2018-08-26"
modified: "2018-08-26"
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