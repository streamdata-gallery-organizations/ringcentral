{
  "info": {
    "name": "RingCentral Get API Versions",
    "_postman_id": "4bfda5a9-bdee-4d7f-981f-872dc3814220",
    "description": "Returns current API version(s) and server info.\nUsage Plan Group\nNoThrottling",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Versions",
      "item": [
        {
          "id": "f4d1f7d1-cd95-4672-9e0c-bfc3a4ef2ed0",
          "name": "getAllVersions",
          "request": {
            "url": "http://platform.ringcentral.com/restapi/",
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
            "description": "Returns current API version(s) and server info.\nUsage Plan Group\nNoThrottling"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "12a808bb-3b3f-4e87-a871-c83f08bcc33d"
            }
          ]
        }
      ]
    }
  ]
}