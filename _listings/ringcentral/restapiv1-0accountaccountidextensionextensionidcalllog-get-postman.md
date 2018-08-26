{
  "info": {
    "name": "RingCentral Get Call Log Records by Filter",
    "_postman_id": "91bbdb6d-dc19-44f5-832d-264c570d109d",
    "description": "Returns call log records filtered by parameters specified.\nApp Permission\nReadCallLog\nUser Permission\nReadCallLog\nUsage Plan Group\nHeavy\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCLG-110\nParameter [sessionId] is not allowed for usage along with parameter [extensionNumber]\n\n\n400\nCMN-101\nParameter [transport] value is invalid\n\n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-129\nAccess token corrupted\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n401\nOAU-213\nToken not found\n\n\n403\nCMN-401\nIn order to call this API endpoint, application needs to have [ReadCallLog] permission\n\n\n403\nCMN-408\nIn order to call this API endpoint, user needs to have [ReadCallLog] permission for requested resource.\n\n\n404\nCMN-102\nResource for parameter [extensionId] is not found\n\n\n429\nCMN-301\nRequest rate exceeded",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "User",
      "item": [
        {
          "id": "507986ad-023e-4872-9424-9b2285d2d7d2",
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
              "id": "678be997-84a3-4933-a244-2c68315bbfef"
            }
          ]
        }
      ]
    },
    {
      "name": "Call",
      "item": [
        {
          "id": "db7d24fc-8b1a-4ff2-b331-7717e4ea0405",
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
              "id": "bcd23523-8114-432a-a05f-7fe436440103"
            }
          ]
        }
      ]
    }
  ]
}