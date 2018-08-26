{
  "info": {
    "name": "RingCentral Get Greeting Info",
    "_postman_id": "cb1f4a4a-b0a2-4676-8f36-a0b91096b73c",
    "description": "Returns a standard greeting by ID.\nUsage Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n404\nCMN-102\nResource for parameter [greetingId] is not found",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Version",
      "item": [
        {
          "id": "35e9beeb-ac59-4b43-ac21-60e7be10d1bf",
          "name": "getApiVersion",
          "request": {
            "url": {
              "protocol": "http",
              "host": "platform.ringcentral.com",
              "path": [
                "restapi/:apiVersion"
              ],
              "variable": [
                {
                  "id": "apiVersion",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns current API version info by apiVersion.\nUsage Plan Group\nNoThrottling"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "13ffde7b-82e6-4b46-a0d1-384e7ac745cc"
            }
          ]
        }
      ]
    },
    {
      "name": "Company",
      "item": [
        {
          "id": "e7ace743-5ffa-4d6d-8790-a2d0dac1a2fa",
          "name": "loadGlipCompany",
          "request": {
            "url": {
              "protocol": "http",
              "host": "platform.ringcentral.com",
              "path": [
                "restapi/v1.0/glip/companies/:companyId"
              ],
              "variable": [
                {
                  "id": "companyId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns a company by ID.\nApp Permission\nGlip\nUser Permission\nGlip\nUsage Plan Group\nLight"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cc539d72-6d25-4590-a5b8-d8d36d8ef111"
            }
          ]
        }
      ]
    },
    {
      "name": "Meeting",
      "item": [
        {
          "id": "fa3f0869-f65c-4ce9-a96e-8e5a44f37bd9",
          "name": "loadMeeting",
          "request": {
            "url": {
              "protocol": "http",
              "host": "platform.ringcentral.com",
              "path": [
                "restapi/v1.0/account/:accountId/extension/:extensionId/meeting/:meetingId"
              ],
              "variable": [
                {
                  "id": "accountId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "extensionId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "meetingId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns a particular meetings details by ID.\nApp Permission\nMeetings\nUser Permission\nMeetings\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n404\nCMN-102\nResource for parameter [meetingId] is not found"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "83aee6a6-ffb5-4aa1-a516-9c6078763c2a"
            }
          ]
        },
        {
          "id": "493f5669-7240-4d0b-810b-c128dffc5b0a",
          "name": "loadMeetingServiceInfo",
          "request": {
            "url": {
              "protocol": "http",
              "host": "platform.ringcentral.com",
              "path": [
                "restapi/v1.0/account/:accountId/extension/:extensionId/meeting/service-info"
              ],
              "variable": [
                {
                  "id": "accountId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "extensionId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns information on dial-in numbers for meetings, support and international dial-in numbers URIs and meeting account information.\nApp Permission\nMeetings\nUser Permission\nMeetings\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n403\nCMN-401\nIn order to call this API endpoint, application needs to have [Meetings] permission\n\n\n403\nCMN-408\nIn order to call this API endpoint, user needs to have [Meetings] permission for requested resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a09b9cd4-0257-46ba-a2fd-8a7fd5e10b68"
            }
          ]
        }
      ]
    },
    {
      "name": "Greeting",
      "item": [
        {
          "id": "6abc3ffe-9ee1-427c-914c-56f2fca49e86",
          "name": "getGreeting",
          "request": {
            "url": {
              "protocol": "http",
              "host": "platform.ringcentral.com",
              "path": [
                "restapi/v1.0/dictionary/greeting/:greetingId"
              ],
              "variable": [
                {
                  "id": "greetingId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns a standard greeting by ID.\nUsage Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n404\nCMN-102\nResource for parameter [greetingId] is not found"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "188b5512-bdc6-4c3a-a38d-c302bf4785d4"
            }
          ]
        }
      ]
    }
  ]
}