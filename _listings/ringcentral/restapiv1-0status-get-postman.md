{
  "info": {
    "name": "RingCentral Get Service status",
    "_postman_id": "8f6493e1-59d4-492d-aab8-6dd70142a6f4",
    "description": "Returns current PAS service status.\nUsage Plan Group\nNoThrottling",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Versions",
      "item": [
        {
          "id": "ecd29aef-fc85-4d7b-ba27-6fb00a237f83",
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
              "id": "649cf745-19bd-4744-8e32-cd3951a8d46b"
            }
          ]
        }
      ]
    },
    {
      "name": "Version",
      "item": [
        {
          "id": "8874359d-09e8-49a6-815b-d521026bf90d",
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
              "id": "765a84f6-68eb-45e9-94ea-9101b8457e15"
            }
          ]
        }
      ]
    },
    {
      "name": "Service",
      "item": [
        {
          "id": "7b08bab1-7724-4562-a00b-e25769d6e6af",
          "name": "loadAPIStatus",
          "request": {
            "url": "http://platform.ringcentral.com/restapi/v1.0/status",
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
            "description": "Returns current PAS service status.\nUsage Plan Group\nNoThrottling"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "70795faf-2866-4dfb-9499-f7aca279fb95"
            }
          ]
        }
      ]
    }
  ]
}