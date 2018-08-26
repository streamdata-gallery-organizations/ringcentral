{
  "info": {
    "name": "RingCentral Get Meeting Service Info",
    "_postman_id": "153a7240-f514-46c1-be28-a1324f1aeb10",
    "description": "Returns information on dial-in numbers for meetings, support and international dial-in numbers URIs and meeting account information.\nApp Permission\nMeetings\nUser Permission\nMeetings\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n403\nCMN-401\nIn order to call this API endpoint, application needs to have [Meetings] permission\n\n\n403\nCMN-408\nIn order to call this API endpoint, user needs to have [Meetings] permission for requested resource.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Version",
      "item": [
        {
          "id": "5c96b664-9b9a-4735-8080-7c65cdf42873",
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
              "id": "55d8ac10-edfa-495a-92e8-a8d431e09474"
            }
          ]
        }
      ]
    },
    {
      "name": "Company",
      "item": [
        {
          "id": "bb8a9228-e2f5-49ab-bf1e-39f3085bb272",
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
              "id": "81904032-584a-4f00-b7e5-e3ac90361dc1"
            }
          ]
        }
      ]
    },
    {
      "name": "Meeting",
      "item": [
        {
          "id": "74e69254-0737-49e2-b48a-b66ac4aac5f6",
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
              "id": "acf2d0ed-843a-4e98-a14d-a25fbe41dbf3"
            }
          ]
        },
        {
          "id": "6461bf66-c877-4842-8d93-15b4c543fc2c",
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
              "id": "91c1a66b-ba2b-46fa-8214-23127e54c104"
            }
          ]
        }
      ]
    }
  ]
}