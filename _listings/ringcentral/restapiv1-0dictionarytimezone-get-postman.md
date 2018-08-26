{
  "info": {
    "name": "RingCentral Get Timezone List",
    "_postman_id": "29472877-858f-4b0e-890a-4a93949d4a51",
    "description": "Returns all available timezones.\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter [perPage] value is invalid",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Timezone",
      "item": [
        {
          "id": "29361dd2-5f60-461e-bf40-69cf92fe1c49",
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
              "id": "8cb2a55b-17ad-4fb5-9471-fc1b2a5f2d08"
            }
          ]
        },
        {
          "id": "3548720b-4610-40d3-858d-7c57d044c448",
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
              "id": "5ee84417-25ca-4837-850d-149d99669a1a"
            }
          ]
        }
      ]
    }
  ]
}