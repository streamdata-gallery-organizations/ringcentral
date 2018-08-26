{
  "info": {
    "name": "RingCentral Get Country",
    "_postman_id": "6d4c3803-5177-4b92-b0b3-bf8cf9cd9544",
    "description": "Returns the information on a specific country.\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-122\nMethod is brand specific\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n404\nCMN-102\nResource for parameter [countryId] is not found",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Country",
      "item": [
        {
          "id": "8100ea4d-b8d1-4e67-872e-f6a6d61450a0",
          "name": "listCountries",
          "request": {
            "url": "http://platform.ringcentral.com/restapi/v1.0/dictionary/country?freeSoftphoneLine=%7B%7D&loginAllowed=%7B%7D&numberSelling=%7B%7D&page=%7B%7D&perPage=%7B%7D&signupAllowed=%7B%7D",
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
            "description": "Returns all the countries available for calling.\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter [perPage] value is invalid\n\n\n401\nAGW-401\nAuthorization header is not specified\n\n\n401\nOAU-129\nAccess token corrupted"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4c3eb4dd-11ca-4171-af91-33aaae01796f"
            }
          ]
        },
        {
          "id": "1338321c-6647-489e-b188-1f4277bc369a",
          "name": "loadCountry",
          "request": {
            "url": {
              "protocol": "http",
              "host": "platform.ringcentral.com",
              "path": [
                "restapi/v1.0/dictionary/country/:countryId"
              ],
              "variable": [
                {
                  "id": "countryId",
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
            "description": "Returns the information on a specific country.\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-122\nMethod is brand specific\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n404\nCMN-102\nResource for parameter [countryId] is not found"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e52ce855-c943-4171-b876-ae4a2a8403b9"
            }
          ]
        }
      ]
    }
  ]
}