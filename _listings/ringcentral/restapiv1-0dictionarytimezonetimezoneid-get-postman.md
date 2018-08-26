{
  "info": {
    "name": "RingCentral Get Timezone",
    "_postman_id": "555cfe63-7683-4e79-8448-67b70e33650f",
    "description": "Returns the information on a certain timezone.\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n404\nCMN-102\nResource for parameter [timezoneId] is not found",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Timezone",
      "item": [
        {
          "id": "eec44938-f588-4261-86c8-e4d0927e0b6a",
          "name": "listTimezones",
          "request": {
            "url": "http://platform.ringcentral.com/restapi/v1.0/dictionary/timezone?page=%7B%7D&perPage=%7B%7D",
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
            "description": "Returns all available timezones.\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter [perPage] value is invalid"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "762f2300-e2d9-484c-a448-6204c0ec961e"
            }
          ]
        },
        {
          "id": "2daef9e7-438d-42ec-8f3a-6098bdb5ad1c",
          "name": "loadTimezone",
          "request": {
            "url": {
              "protocol": "http",
              "host": "platform.ringcentral.com",
              "path": [
                "restapi/v1.0/dictionary/timezone/:timezoneId"
              ],
              "query": [
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "perPage",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "timezoneId",
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
            "description": "Returns the information on a certain timezone.\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n404\nCMN-102\nResource for parameter [timezoneId] is not found"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "94bfac71-62eb-4089-9a3e-393675dbe298"
            }
          ]
        }
      ]
    }
  ]
}