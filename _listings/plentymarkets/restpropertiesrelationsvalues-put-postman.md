{
  "info": {
    "name": "Plentymarkets Update multiple property relation value",
    "_postman_id": "e6d6620f-a24a-4e3f-bef3-aba4f0491d99",
    "description": "Updates multiple property relation value",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Multiple",
      "item": [
        {
          "id": "8752acc8-faf5-4fe6-af69-95b4311ba286",
          "name": "deleteRestFeedbacksDeleteFeedbacksFeedbacks",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/feedbacks/delete_feedbacks/:feedbackIds"
              ],
              "variable": [
                {
                  "id": "feedbackIds",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
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
            "description": "Deletes multiple feedbacks. A list with IDs of feedbacks must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b4170350-5020-4dc9-bca2-571463147974"
            }
          ]
        },
        {
          "id": "bd1d5c0f-8215-4f74-b283-6f9538760307",
          "name": "postRestMarketsSettingsCorrelationsBulk",
          "request": {
            "url": "http://example.com/rest/markets/settings/correlations/bulk",
            "method": "POST",
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
            "description": "Creates multiple correlations. The type, market settings ID and the correlation ID for each param combination must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c74fd2cf-5b9c-434f-9033-94509fcd9406"
            }
          ]
        },
        {
          "id": "cd27d9f2-b95e-4eb9-b94d-62ff008b4150",
          "name": "deleteRestPluginSetsPluginsetLanguagesLanguagecode",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/plugin_sets/:pluginSetId/languages/:languageCode"
              ],
              "query": [
                {
                  "key": "$languageCode",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "$pluginSetId",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "languageCode",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "pluginSetId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
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
            "description": "Deletes multiple translation. The pluginSetId and languageCode must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "925b3194-1331-41eb-a4c1-06a2658da620"
            }
          ]
        },
        {
          "id": "a0cd03ce-c72a-4aeb-adc9-17fc54885617",
          "name": "putRestPropertiesRelationsValues",
          "request": {
            "url": "http://example.com/rest/properties/relations/values",
            "method": "PUT",
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
            "description": "Updates multiple property relation value"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c05a23a5-ebf8-44e4-ab88-aed8af73cecb"
            }
          ]
        }
      ]
    },
    {
      "name": "Visibility",
      "item": [
        {
          "id": "90bffa59-a541-4929-8857-59909ebc8a3d",
          "name": "putRestFeedbacksFeedbacksVisibility",
          "request": {
            "url": "http://example.com/rest/feedbacks/feedbacks_visibility?feedbackIds=%7B%7D&isVisible=%7B%7D",
            "method": "PUT",
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
            "description": "Updates the visibility of multiple feedbacks. A list with IDs of feedbacks must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "54461cd3-99f4-4e96-826f-0e2a7439a86f"
            }
          ]
        }
      ]
    }
  ]
}