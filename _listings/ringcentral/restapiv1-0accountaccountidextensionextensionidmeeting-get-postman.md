{
  "info": {
    "name": "RingCentral Get Scheduled Meetings [Beta]",
    "_postman_id": "817aa69d-3017-4ea4-9863-2b472cd01dc7",
    "description": "Returns a list of meetings for a particular extension. The list of meetings does not include meetings of &#39;Instant&#39; type.\nApp Permission\nMeetings\nUser Permission\nMeetings\nUsage Plan Group\nLight",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Scheduled",
      "item": [
        {
          "id": "1998650c-26a3-4bab-893c-b97791972916",
          "name": "listMeetings",
          "request": {
            "url": {
              "protocol": "http",
              "host": "platform.ringcentral.com",
              "path": [
                "restapi/v1.0/account/:accountId/extension/:extensionId/meeting"
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
            "description": "Returns a list of meetings for a particular extension. The list of meetings does not include meetings of &#39;Instant&#39; type.\nApp Permission\nMeetings\nUser Permission\nMeetings\nUsage Plan Group\nLight"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "93c3fa84-66f9-4b74-bc6f-fbe6241064bf"
            }
          ]
        }
      ]
    }
  ]
}