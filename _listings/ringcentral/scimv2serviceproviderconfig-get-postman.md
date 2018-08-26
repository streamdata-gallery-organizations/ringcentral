{
  "info": {
    "name": "RingCentral get service provider config",
    "_postman_id": "571f8c60-d589-4101-a09b-eca747673f4f",
    "description": "",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Get",
      "item": [
        {
          "id": "9b0de064-047a-4ece-b743-d93ed710f732",
          "name": "getServiceProviderConfig",
          "request": {
            "url": "http://platform.ringcentral.com/scim/v2/ServiceProviderConfig",
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
            "description": "get service provider config"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8e6a3907-fbae-461c-abcb-b6b27e854f74"
            }
          ]
        }
      ]
    }
  ]
}