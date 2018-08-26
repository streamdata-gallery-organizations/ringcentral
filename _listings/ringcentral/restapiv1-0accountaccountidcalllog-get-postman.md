{
  "info": {
    "name": "RingCentral Get Call Log Records by Filter",
    "_postman_id": "2741ed45-9991-452d-81f2-115e5d04a8b7",
    "description": "Returns call log records filtered by parameters specified.\nApp Permission\nReadCallLog\nUser Permission\nFullCompanyCallLog\nUsage Plan Group\nHeavy\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCLG-110\nParameter [sessionId] is not allowed for usage along with parameter [extensionNumber]\n\n\n400\nCMN-101\nParameter [dateFrom] value is invalid\n\n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n403\nCMN-401\nIn order to call this API endpoint, application needs to have [ReadCallLog] permission\n\n\n403\nCMN-408\nIn order to call this API endpoint, user needs to have [ReadCompanyCallLog] permission for requested resource.\n\n\n404\nCMN-102\nResource for parameter [accountId] is not found",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "User",
      "item": [
        {
          "id": "f9e63091-426f-4cc8-852e-584bfd451b08",
          "name": "listExtensionActiveCalls",
          "request": {
            "url": {
              "protocol": "http",
              "host": "platform.ringcentral.com",
              "path": [
                "restapi/v1.0/account/:accountId/extension/:extensionId/active-calls"
              ],
              "query": [
                {
                  "key": "direction",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "perPage",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "type",
                  "value": "%7B%7D",
                  "disabled": false
                }
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
            "description": "Returns records of all extension calls that are in progress, ordered by start time in descending order.\nApp Permission\nReadCallLog\nUser Permission\nReadCallLog\nUsage Plan Group\nHeavy\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter [direction] value is invalid\n\n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n403\nCMN-401\nIn order to call this API endpoint, application needs to have [ReadCallLog] permission\n\n\n403\nCMN-408\nIn order to call this API endpoint, user needs to have [ReadCallLog] permission for requested resource.\n\n\n404\nCMN-102\nResource for parameter [accountId] is not found"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "61f79d7c-669e-488e-a039-7cdd5ba7b3e9"
            }
          ]
        }
      ]
    },
    {
      "name": "Call",
      "item": [
        {
          "id": "2cf6eb55-22ad-4ed4-9309-b762736a0c05",
          "name": "loadExtensionCallLog",
          "request": {
            "url": {
              "protocol": "http",
              "host": "platform.ringcentral.com",
              "path": [
                "restapi/v1.0/account/:accountId/extension/:extensionId/call-log"
              ],
              "query": [
                {
                  "key": "dateFrom",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "dateTo",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "direction",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "extensionNumber",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "perPage",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "phoneNumber",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sessionId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "showBlocked",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "transport",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "view",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "withRecording",
                  "value": "%7B%7D",
                  "disabled": false
                }
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
            "description": "Returns call log records filtered by parameters specified.\nApp Permission\nReadCallLog\nUser Permission\nReadCallLog\nUsage Plan Group\nHeavy\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCLG-110\nParameter [sessionId] is not allowed for usage along with parameter [extensionNumber]\n\n\n400\nCMN-101\nParameter [transport] value is invalid\n\n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-129\nAccess token corrupted\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n401\nOAU-213\nToken not found\n\n\n403\nCMN-401\nIn order to call this API endpoint, application needs to have [ReadCallLog] permission\n\n\n403\nCMN-408\nIn order to call this API endpoint, user needs to have [ReadCallLog] permission for requested resource.\n\n\n404\nCMN-102\nResource for parameter [extensionId] is not found\n\n\n429\nCMN-301\nRequest rate exceeded"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "20bbd610-de7f-4e36-a46a-44c832729c37"
            }
          ]
        },
        {
          "id": "1f88cc1d-f12e-4e5b-9335-31483c0a517f",
          "name": "getCallRecords",
          "request": {
            "url": {
              "protocol": "http",
              "host": "platform.ringcentral.com",
              "path": [
                "restapi/v1.0/account/:accountId/extension/:extensionId/call-log/:callRecordId"
              ],
              "query": [
                {
                  "key": "view",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "accountId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "callRecordId",
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
            "description": "Returns filtered call log records.\nApp Permission\nReadCallLog\nUser Permission\nReadCallLog\nUsage Plan Group\nHeavy\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n403\nCMN-401\nIn order to call this API endpoint, application needs to have [ReadCallLog] permission\n\n\n403\nCMN-408\nIn order to call this API endpoint, user needs to have [ReadCallLog] permission for requested resource.\n\n\n404\nCMN-102\nResource for parameter [extensionId] is not found"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1d19cbe1-648a-4994-aeea-ca227beccbe1"
            }
          ]
        },
        {
          "id": "47ec7162-0000-45d5-9999-4c69ba7b4916",
          "name": "loadAccountCallLog",
          "request": {
            "url": {
              "protocol": "http",
              "host": "platform.ringcentral.com",
              "path": [
                "restapi/v1.0/account/:accountId/call-log"
              ],
              "query": [
                {
                  "key": "dateFrom",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "dateTo",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "direction",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "extensionNumber",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "perPage",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "phoneNumber",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sessionId",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "view",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "withRecording",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "accountId",
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
            "description": "Returns call log records filtered by parameters specified.\nApp Permission\nReadCallLog\nUser Permission\nFullCompanyCallLog\nUsage Plan Group\nHeavy\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCLG-110\nParameter [sessionId] is not allowed for usage along with parameter [extensionNumber]\n\n\n400\nCMN-101\nParameter [dateFrom] value is invalid\n\n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n403\nCMN-401\nIn order to call this API endpoint, application needs to have [ReadCallLog] permission\n\n\n403\nCMN-408\nIn order to call this API endpoint, user needs to have [ReadCompanyCallLog] permission for requested resource.\n\n\n404\nCMN-102\nResource for parameter [accountId] is not found"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "200d83cd-cb71-4a44-851d-a38bd8de83eb"
            }
          ]
        }
      ]
    }
  ]
}