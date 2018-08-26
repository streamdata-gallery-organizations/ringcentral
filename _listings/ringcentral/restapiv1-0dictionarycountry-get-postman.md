{
  "info": {
    "name": "RingCentral Get Country List",
    "_postman_id": "0be35af3-7481-49df-98af-d5d23f05452e",
    "description": "Returns all the countries available for calling.\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter [perPage] value is invalid\n\n\n401\nAGW-401\nAuthorization header is not specified\n\n\n401\nOAU-129\nAccess token corrupted",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Country",
      "item": [
        {
          "id": "11dfa1c2-2d62-4c12-bf4d-9be3e5935611",
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
              "id": "678e9fe7-3c32-4775-a379-eb715bed58ae"
            }
          ]
        },
        {
          "id": "a7b47e5c-9f55-4163-ab3b-b5cdad99f776",
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
              "id": "4e6bd9da-0277-4c9b-b3a5-e5e574fdf41a"
            }
          ]
        }
      ]
    }
  ]
}