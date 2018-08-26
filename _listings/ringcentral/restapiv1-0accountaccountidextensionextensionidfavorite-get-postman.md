{
  "info": {
    "name": "RingCentral Get Favorite Contacts",
    "_postman_id": "7a41b277-d726-434e-a8b0-c91708412d1c",
    "description": "Returns favorite contacts of the current extension. Favorite contacts include both company contacts (extensions) and personal contacts (address book records).\nApp Permission\nReadContacts\nUser Permission\nReadPersonalContacts\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n403\nCMN-401\nIn order to call this API endpoint, application needs to have [ReadContacts] permission\n\n\n403\nCMN-408\nIn order to call this API endpoint, user needs to have [ReadPersonalContacts] permission for requested resource.\n\n\n404\nCMN-102\nResource for parameter [accountId] is not found",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Contacts",
      "item": [
        {
          "id": "b5a5ffee-43e5-44a9-a524-8cef35033ae3",
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
              "id": "611708a1-0c4a-41e9-bc81-6ebfd5f7a768"
            }
          ]
        }
      ]
    },
    {
      "name": "Favorite",
      "item": [
        {
          "id": "27a08edd-79ae-469a-9830-87d7ec1a1ab4",
          "name": "listFavoriteContacts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "platform.ringcentral.com",
              "path": [
                "restapi/v1.0/account/:accountId/extension/:extensionId/favorite"
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
            "description": "Returns favorite contacts of the current extension. Favorite contacts include both company contacts (extensions) and personal contacts (address book records).\nApp Permission\nReadContacts\nUser Permission\nReadPersonalContacts\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n403\nCMN-401\nIn order to call this API endpoint, application needs to have [ReadContacts] permission\n\n\n403\nCMN-408\nIn order to call this API endpoint, user needs to have [ReadPersonalContacts] permission for requested resource.\n\n\n404\nCMN-102\nResource for parameter [accountId] is not found"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "07e03b10-c0b6-4cd8-bccf-48c914af35bf"
            }
          ]
        }
      ]
    }
  ]
}