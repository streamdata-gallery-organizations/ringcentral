{
  "info": {
    "name": "RingCentral Get Location List",
    "_postman_id": "59f0fd72-fc5d-4150-b87c-90840378d168",
    "description": "Returns all available locations for a certain state.\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter [orderBy] value is invalid\n\n\n404\nCMN-102\nResource for parameter [location] is not found",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Location",
      "item": [
        {
          "id": "621afe1f-5910-4f70-a831-446fb02fac34",
          "name": "listLocations",
          "request": {
            "url": "http://platform.ringcentral.com/restapi/v1.0/dictionary/location?orderBy=%7B%7D&page=%7B%7D&perPage=%7B%7D&stateId=%7B%7D&withNxx=%7B%7D",
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
            "description": "Returns all available locations for a certain state.\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter [orderBy] value is invalid\n\n\n404\nCMN-102\nResource for parameter [location] is not found"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "441288bd-6d09-4036-9d38-2aa5552829b0"
            }
          ]
        }
      ]
    }
  ]
}