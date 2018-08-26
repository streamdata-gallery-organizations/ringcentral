{
  "info": {
    "name": "RingCentral Get Message Attachment",
    "_postman_id": "7813eaf1-d00a-4a40-ae39-d717f6132a1f",
    "description": "Returns a specific message attachment data as a media stream.\nApp Permission\nReadMessages\nUser Permission\nReadMessageContent\nUsage Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n401\nAGW-402\nInvalid Authorization header\n\n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-149\nUnparsable access token\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n403\nCMN-401\nIn order to call this API endpoint, application needs to have [ReadMessages] permission\n\n\n403\nCMN-408\nIn order to call this API endpoint, user needs to have [ReadMessageContent] permission for requested resource.\n\n\n404\nCMN-102\nResource for parameter [extensionId] is not found\n\n\n416\nCMN-107\nRequested range not satisfiable",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Message",
      "item": [
        {
          "id": "dd3a8289-e01e-46c3-a012-0637b799ae24",
          "name": "preturns-a-specific-message-attachment-data-as-a-media-streamph4app-permissionh4preadmessagesph4user",
          "request": {
            "url": {
              "protocol": "http",
              "host": "platform.ringcentral.com",
              "path": [
                "restapi/v1.0/account/:accountId/extension/:extensionId/message-store/:messageId/content/:attachmentId"
              ],
              "variable": [
                {
                  "id": "accountId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "attachmentId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "extensionId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "messageId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Range",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns a specific message attachment data as a media stream.\nApp Permission\nReadMessages\nUser Permission\nReadMessageContent\nUsage Plan Group\nMedium\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n401\nAGW-402\nInvalid Authorization header\n\n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-149\nUnparsable access token\n\n\n401\nOAU-151\nAuthorization method not supported\n\n\n403\nCMN-401\nIn order to call this API endpoint, application needs to have [ReadMessages] permission\n\n\n403\nCMN-408\nIn order to call this API endpoint, user needs to have [ReadMessageContent] permission for requested resource.\n\n\n404\nCMN-102\nResource for parameter [extensionId] is not found\n\n\n416\nCMN-107\nRequested range not satisfiable"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "86546e0c-a6fb-4534-9ceb-2529b7f0b0dd"
            }
          ]
        }
      ]
    }
  ]
}