{
  "info": {
    "name": "RingCentral Upload File",
    "_postman_id": "eacd8314-d811-41e9-881a-bb573f1907d4",
    "description": "Posts a file.\nApp Permission\nGlip\nUser Permission\nGlip\nUsage Plan Group\nHeavy",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Upload",
      "item": [
        {
          "id": "2c765df0-c496-43b4-a85d-3a50b78cd9b3",
          "name": "createGlipFile",
          "request": {
            "url": "http://platform.ringcentral.com/restapi/v1.0/glip/files?groupId=%7B%7D",
            "method": "POST",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "body",
                  "value": "{}",
                  "disabled": false,
                  "description": "The file to upload"
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "Name of a file attached"
                }
              ]
            },
            "description": "Posts a file.\nApp Permission\nGlip\nUser Permission\nGlip\nUsage Plan Group\nHeavy"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1ea4c55f-1544-4287-aae9-07431dfc1417"
            }
          ]
        }
      ]
    }
  ]
}