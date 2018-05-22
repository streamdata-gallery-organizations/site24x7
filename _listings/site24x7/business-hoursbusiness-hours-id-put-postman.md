{
  "info": {
    "name": "Business Hours API Update Business Hour",
    "_postman_id": "989a8a63-c94d-44a4-a5f0-1df3392b596d",
    "description": "Update an existing Business Hour.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Business Hours",
      "item": [
        {
          "id": "4e1875a3-1fff-4dc6-b27a-ab991942baa6",
          "name": "create-business-hour",
          "request": {
            "url": "http://www.site24x7.com./business_hours?display_name\n        \n        \n            required\n            Display name for the Business Hour.\n        \n    \n    \n        \n        description\n        \n        \n            optional\n            Description for the Business Hour=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a new Business Hour."
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "61096649-41c8-4d5a-9fa3-97cf5a01b0f1"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "286c1ac8-221c-4d6a-8b63-4b84cf0c6fb1"
            }
          ]
        },
        {
          "id": "a892e22a-e570-49cf-a92c-d6b2f38fbb5f",
          "name": "update-business-hour",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.site24x7.com.",
              "path": [
                "business_hours/:business_hours_id"
              ],
              "query": [
                {
                  "key": "display_name\n        \n        \n            required\n            Display name for the Business Hour.\n        \n    \n    \n        \n        description\n        \n        \n            optional\n            Description for the Business Hour",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "business_hours_id",
                  "value": "business_hours_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update an existing Business Hour."
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "18fb65ec-c01c-43e5-9b73-96daf8833704"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "288f4c83-3a29-4b54-82ea-a55ff7fd1165"
            }
          ]
        }
      ]
    }
  ]
}