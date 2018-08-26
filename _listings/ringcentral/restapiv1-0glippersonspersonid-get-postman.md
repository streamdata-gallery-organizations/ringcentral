{
  "info": {
    "name": "RingCentral Get Person",
    "_postman_id": "4911656d-e7ba-45a6-a127-686dfd9f922a",
    "description": "Returns a user or multiple users by their ID(s). Batch request is supported.\nApp Permission\nGlip\nUser Permission\nGlip\nUsage Plan Group\nLight",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Person",
      "item": [
        {
          "id": "967f9222-fc3d-41e8-b83c-d937be77ed02",
          "name": "loadGlipPerson",
          "request": {
            "url": {
              "protocol": "http",
              "host": "platform.ringcentral.com",
              "path": [
                "restapi/v1.0/glip/persons/:personId"
              ],
              "variable": [
                {
                  "id": "personId",
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
            "description": "Returns a user or multiple users by their ID(s). Batch request is supported.\nApp Permission\nGlip\nUser Permission\nGlip\nUsage Plan Group\nLight"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6a1d0389-2cfd-443b-9b85-a4c933c31fd5"
            }
          ]
        }
      ]
    }
  ]
}