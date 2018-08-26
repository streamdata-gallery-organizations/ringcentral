{
  "info": {
    "name": "RingCentral Get Contacts",
    "_postman_id": "83dc6d81-1d4f-462f-bc16-9f9eb3b3cd43",
    "description": "Returns user personal contacts.\nApp Permission\nReadContacts\nUser Permission\nReadPersonalContacts\nUsage Plan Group\nHeavy\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter [perPage] value is invalid\n\n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n403\nCMN-401\nIn order to call this API endpoint, application needs to have [ReadContacts] permission\n\n\n404\nCMN-102\nResource for parameter [accountId] is not found",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Contacts",
      "item": [
        {
          "id": "235ec65a-22ed-4b13-8a81-6b791e0d4751",
          "name": "listContacts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "platform.ringcentral.com",
              "path": [
                "restapi/v1.0/account/:accountId/extension/:extensionId/address-book/contact"
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
                },
                {
                  "key": "phoneNumber",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sortBy",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "startsWith",
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
            "description": "Returns user personal contacts.\nApp Permission\nReadContacts\nUser Permission\nReadPersonalContacts\nUsage Plan Group\nHeavy\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter [perPage] value is invalid\n\n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n403\nCMN-401\nIn order to call this API endpoint, application needs to have [ReadContacts] permission\n\n\n404\nCMN-102\nResource for parameter [accountId] is not found"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b818bd95-ecb6-4287-9024-391e290e30ed"
            }
          ]
        }
      ]
    }
  ]
}