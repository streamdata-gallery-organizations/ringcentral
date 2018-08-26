{
  "info": {
    "name": "RingCentral Get Available Fax Cover Pages",
    "_postman_id": "755b02fb-40c5-4b16-8ade-5d63fdcde69a",
    "description": "Returns fax cover pages available for the current extension.\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter [page] value is invalid\n\n\n401\nCMN-405\nLogin to extension required",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Available",
      "item": [
        {
          "id": "3f345ff6-850f-4fe2-935a-ecdd9e4a5335",
          "name": "listFaxCoverPages",
          "request": {
            "url": "http://platform.ringcentral.com/restapi/v1.0/dictionary/fax-cover-page?page=%7B%7D&perPage=%7B%7D",
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
            "description": "Returns fax cover pages available for the current extension.\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter [page] value is invalid\n\n\n401\nCMN-405\nLogin to extension required"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4d89c106-5c04-40ca-83ec-edd1817b3cdb"
            }
          ]
        }
      ]
    }
  ]
}