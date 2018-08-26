{
  "info": {
    "name": "RingCentral Get IVR Prompt Content",
    "_postman_id": "2cb72b06-b1a5-430a-9983-0de847f75994",
    "description": "Returns media content of an IVR prompt by ID.\nApp Permission\nReadAccounts\nUser Permission\nReadCompanyGreetings\nUsage Plan Group\nMedium",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "IVR",
      "item": [
        {
          "id": "ce973f57-2be6-4146-9470-b807ad81219c",
          "name": "getPromptContent",
          "request": {
            "url": {
              "protocol": "http",
              "host": "platform.ringcentral.com",
              "path": [
                "restapi/v1.0/account/:accountId/ivr-prompts/:promptId/content"
              ],
              "variable": [
                {
                  "id": "accountId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "promptId",
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
            "description": "Returns media content of an IVR prompt by ID.\nApp Permission\nReadAccounts\nUser Permission\nReadCompanyGreetings\nUsage Plan Group\nMedium"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0239afe7-cebc-468c-936b-1d20b168e4d0"
            }
          ]
        }
      ]
    }
  ]
}