{
  "info": {
    "name": "RingCentral Get Department Member List",
    "_postman_id": "bda9292c-3a33-4b95-bbfb-824c24419329",
    "description": "[Deprecated] Viewing user account info (including name, business name, address and phone number/account number)\nApp Permission\nReadAccounts\nUser Permission\nReadExtensions\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter [page] value is invalid\n\n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n403\nCMN-401\nIn order to call this API endpoint, application needs to have [ReadAccounts] permission\n\n\n404\nCMN-102\nResource for parameter [departmentId] is not found",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Department",
      "item": [
        {
          "id": "41741f6a-186e-4438-a643-1c67ee57b591",
          "name": "listDepartmentMembers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "platform.ringcentral.com",
              "path": [
                "restapi/v1.0/account/:accountId/department/:departmentId/members"
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
                  "id": "accountId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "departmentId",
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
            "description": "[Deprecated] Viewing user account info (including name, business name, address and phone number/account number)\nApp Permission\nReadAccounts\nUser Permission\nReadExtensions\nUsage Plan Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter [page] value is invalid\n\n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n403\nCMN-401\nIn order to call this API endpoint, application needs to have [ReadAccounts] permission\n\n\n404\nCMN-102\nResource for parameter [departmentId] is not found"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "14c3218c-eda7-4ccc-a9c2-c815219d39de"
            }
          ]
        }
      ]
    }
  ]
}