{
  "info": {
    "name": "RingCentral Get Extension Grants",
    "_postman_id": "136b9ad6-d51c-4160-9623-a1d14ed2ff9f",
    "description": "Returns the list of extension grants.\nApp Permission\nReadAccounts\nUser Permission\nReadExtensions\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n403\nCMN-408\nIn order to call this API endpoint, user needs to have [ReadExtensionGrant] permission for requested resource.\n\n\n404\nCMN-102\nResource for parameter [accountId] is not found",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Extension",
      "item": [
        {
          "id": "186ad592-149e-4ac6-bf62-3eea13f2e0bd",
          "name": "listExtensionGrants",
          "request": {
            "url": {
              "protocol": "http",
              "host": "platform.ringcentral.com",
              "path": [
                "restapi/v1.0/account/:accountId/extension/:extensionId/grant"
              ],
              "query": [
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "perPage",
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
            "description": "Returns the list of extension grants.\nApp Permission\nReadAccounts\nUser Permission\nReadExtensions\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n403\nCMN-408\nIn order to call this API endpoint, user needs to have [ReadExtensionGrant] permission for requested resource.\n\n\n404\nCMN-102\nResource for parameter [accountId] is not found"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3232ad17-fb87-4122-a98a-a20d48c551be"
            }
          ]
        }
      ]
    }
  ]
}