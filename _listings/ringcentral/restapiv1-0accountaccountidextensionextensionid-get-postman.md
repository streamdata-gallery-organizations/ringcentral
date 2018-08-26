{
  "info": {
    "name": "RingCentral Get Extension Info",
    "_postman_id": "99299da5-6e01-4bd4-b28e-0b753f113308",
    "description": "Returns basic information about a particular extension of an account.\nApp Permission\nReadAccounts\nUser Permission\nReadExtensions\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-129\nAccess token corrupted\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n403\nCMN-401\nIn order to call this API endpoint, application needs to have [ReadAccounts] permission\n\n\n404\nCMN-102\nResource for parameter [extensionId] is not found\n\n\n429\nCMN-301\nRequest rate exceeded",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Version",
      "item": [
        {
          "id": "b267cb61-c3dd-4136-a94b-c9060b9a97bf",
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
              "id": "db48e400-df3e-418e-be5a-80c8060b3517"
            }
          ]
        }
      ]
    },
    {
      "name": "Company",
      "item": [
        {
          "id": "af7d2f3a-5837-448d-b44b-2c88d1b61e92",
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
              "id": "d4ff4f07-8e1b-40d5-b985-3d4e77010765"
            }
          ]
        }
      ]
    },
    {
      "name": "Meeting",
      "item": [
        {
          "id": "a9ea811c-68e4-426d-a8e9-d5add6c9fd0c",
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
              "id": "f10377c5-7ca4-4ea6-8510-cb6569a96d3b"
            }
          ]
        },
        {
          "id": "6ce8500a-fb33-41c6-a7e9-fc503ee3bbff",
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
              "id": "0c51fedf-3279-48cd-988c-a6b5bc044bf6"
            }
          ]
        }
      ]
    },
    {
      "name": "Greeting",
      "item": [
        {
          "id": "254dede6-6af8-4f49-9fbd-9a85c70eac87",
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
              "id": "9c394daf-3dfe-4626-9357-0aa0bbfe1e14"
            }
          ]
        }
      ]
    },
    {
      "name": "Custom",
      "item": [
        {
          "id": "8502cd63-dbd7-4d19-98c6-949af792ad97",
          "name": "getGreetingByID",
          "request": {
            "url": {
              "protocol": "http",
              "host": "platform.ringcentral.com",
              "path": [
                "restapi/v1.0/account/:accountId/extension/:extensionId/greeting/:greetingId"
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
            "description": "Returns a custom user greeting by ID.\nApp Permission\nReadAccounts\nUser Permission\nReadUserInfo\nUsage Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n404\nCMN-102\nResource for parameter [greetingId] is not found"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1c9bcc73-0b1d-4b6c-a423-f91af962325a"
            }
          ]
        }
      ]
    },
    {
      "name": "Extension",
      "item": [
        {
          "id": "11327106-77ca-4131-9f72-2b61909d31e7",
          "name": "loadExtensionInfo",
          "request": {
            "url": {
              "protocol": "http",
              "host": "platform.ringcentral.com",
              "path": [
                "restapi/v1.0/account/:accountId/extension/:extensionId"
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
            "description": "Returns basic information about a particular extension of an account.\nApp Permission\nReadAccounts\nUser Permission\nReadExtensions\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-129\nAccess token corrupted\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n403\nCMN-401\nIn order to call this API endpoint, application needs to have [ReadAccounts] permission\n\n\n404\nCMN-102\nResource for parameter [extensionId] is not found\n\n\n429\nCMN-301\nRequest rate exceeded"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b1950fc7-291c-41fb-8e9b-7ea5c4b98c20"
            }
          ]
        }
      ]
    }
  ]
}