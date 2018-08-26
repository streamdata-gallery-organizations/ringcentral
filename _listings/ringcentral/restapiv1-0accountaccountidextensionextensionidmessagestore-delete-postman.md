{
  "info": {
    "name": "RingCentral Delete Conversations by ID's",
    "_postman_id": "b0026268-3381-42f2-b725-e5e64623d746",
    "description": "Deletes conversation(s) by conversation ID(s). Batch request is supported.\nApp Permission\nEditMessages\nUser Permission\nEditMessages\nUsage Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter [conversationId] value is invalid\n\n\n403\nCMN-401\nIn order to call this API endpoint, application needs to have [EditMessages] permission",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Conversations",
      "item": [
        {
          "id": "42cd0fd2-40aa-4c3b-b34f-5060203ae4b2",
          "name": "deleteMessagesByFilter",
          "request": {
            "url": {
              "protocol": "http",
              "host": "platform.ringcentral.com",
              "path": [
                "restapi/v1.0/account/:accountId/extension/:extensionId/message-store"
              ],
              "query": [
                {
                  "key": "conversationId",
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
            "method": "DELETE",
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
            "description": "Deletes conversation(s) by conversation ID(s). Batch request is supported.\nApp Permission\nEditMessages\nUser Permission\nEditMessages\nUsage Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter [conversationId] value is invalid\n\n\n403\nCMN-401\nIn order to call this API endpoint, application needs to have [EditMessages] permission"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dbdbd366-4f46-4332-a265-15f620696939"
            }
          ]
        }
      ]
    }
  ]
}