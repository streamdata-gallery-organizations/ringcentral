{
  "info": {
    "name": "RingCentral Get Version Info",
    "_postman_id": "9d598eb8-9435-433f-9b43-eb5c6d4b1e5d",
    "description": "Returns current API version info by apiVersion.\nUsage Plan Group\nNoThrottling",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Version",
      "item": [
        {
          "id": "968ecb9f-fffa-4db2-a5ee-f1c455424dff",
          "name": "getApiVersion",
          "request": {
            "url": {
              "protocol": "http",
              "host": "platform.ringcentral.com",
              "path": [
                "restapi/:apiVersion"
              ],
              "variable": [
                {
                  "id": "apiVersion",
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
            "description": "Returns current API version info by apiVersion.\nUsage Plan Group\nNoThrottling"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "43a7c292-4649-44b8-a609-271f526aefcd"
            }
          ]
        }
      ]
    }
  ]
}