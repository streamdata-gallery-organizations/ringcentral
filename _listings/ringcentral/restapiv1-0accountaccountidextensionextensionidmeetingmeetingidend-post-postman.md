{
  "info": {
    "name": "RingCentral End Meeting",
    "_postman_id": "b6b70be1-d23f-4257-a858-4a18b09602a2",
    "description": "Ends a meetings which is in progress.\nApp Permission\nMeetings\nUser Permission\nMeetings\nUsage Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n404\nCMN-102\nResource for parameter [meetingId] is not found",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "End",
      "item": [
        {
          "id": "77efdea7-f2ac-4e35-a308-bc5e3b8f09b1",
          "name": "endMeeting",
          "request": {
            "url": {
              "protocol": "http",
              "host": "platform.ringcentral.com",
              "path": [
                "restapi/v1.0/account/:accountId/extension/:extensionId/meeting/:meetingId/end"
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
                },
                {
                  "id": "meetingId",
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
            "description": "Ends a meetings which is in progress.\nApp Permission\nMeetings\nUser Permission\nMeetings\nUsage Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n404\nCMN-102\nResource for parameter [meetingId] is not found"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1298b074-cefa-425c-90e6-41681002c148"
            }
          ]
        }
      ]
    }
  ]
}