{
  "info": {
    "name": "RingCentral Get Blocked Numbers",
    "_postman_id": "a9dbc8be-bc08-4c81-a45f-06e8e4684e0e",
    "description": "Returns the list of phone numbers which are specified by the user to block inbound calls and SMS messages.\nApp Permission\nReadAccounts\nUser Permission\nReadBlockedNumbers\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter [perPage] value is invalid\n\n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n403\nCMN-401\nIn order to call this API endpoint, application needs to have [ReadAccounts] permission\n\n\n403\nCMN-408\nIn order to call this API endpoint, user needs to have [ReadBlockedNumbers] permission for requested resource.\n\n\n404\nCMN-102\nResource for parameter [extensionId] is not found",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blocked",
      "item": [
        {
          "id": "f02444ed-deea-4cd6-a753-a40f25ce3aa2",
          "name": "listBlockedNumbers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "platform.ringcentral.com",
              "path": [
                "restapi/v1.0/account/:accountId/extension/:extensionId/blocked-number"
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
            "description": "Returns the list of phone numbers which are specified by the user to block inbound calls and SMS messages.\nApp Permission\nReadAccounts\nUser Permission\nReadBlockedNumbers\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter [perPage] value is invalid\n\n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n403\nCMN-401\nIn order to call this API endpoint, application needs to have [ReadAccounts] permission\n\n\n403\nCMN-408\nIn order to call this API endpoint, user needs to have [ReadBlockedNumbers] permission for requested resource.\n\n\n404\nCMN-102\nResource for parameter [extensionId] is not found"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b0c6a3b5-01ec-42a3-bc54-bca862f416be"
            }
          ]
        }
      ]
    }
  ]
}