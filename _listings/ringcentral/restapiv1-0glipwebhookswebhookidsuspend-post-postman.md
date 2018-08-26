{
  "info": {
    "name": "RingCentral Suspend Webhook",
    "_postman_id": "81f55f99-6da7-4847-9271-7165b8a7cd4f",
    "description": "Suspends webhooks by ID.\nUsage Plan Group\nMedium",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Suspend",
      "item": [
        {
          "id": "1eeb5368-ae6c-430b-92aa-329818e343c9",
          "name": "suspendGlipWebhook",
          "request": {
            "url": {
              "protocol": "http",
              "host": "platform.ringcentral.com",
              "path": [
                "restapi/v1.0/glip/webhooks/:webhookId/suspend"
              ],
              "variable": [
                {
                  "id": "webhookId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
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
            "description": "Suspends webhooks by ID.\nUsage Plan Group\nMedium"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5d4aa737-d486-4b5d-8497-e5e284865663"
            }
          ]
        }
      ]
    }
  ]
}