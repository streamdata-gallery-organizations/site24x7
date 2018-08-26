{
  "info": {
    "name": "Monitor Group API Update a Monitor Group",
    "_postman_id": "a386caf0-0558-409b-8c08-a6f46f6fce64",
    "description": "Update an existing Monitor Group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Monitor Groups",
      "item": [
        {
          "id": "54fb8a47-4cf0-4395-8e7d-3b94cb59bae6",
          "name": "create-a-monitor-group",
          "request": {
            "url": "http://www.site24x7.com./monitor_groups?display_name\n        \n        \n            required\n            Display Name for the Monitor Group.\n        \n    \n    \n        \n        description\n        \n        \n            optional\n            Description for the Monitor Group.=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a new Monitor Group."
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "832715ca-3091-4d4a-9255-209eecd3c5c9"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "7799e2a5-a898-4efb-a1d4-310f50dda1fc"
            }
          ]
        },
        {
          "id": "2ad379f1-ab1c-4e2f-bec5-7d03b06c2176",
          "name": "update-a-monitor-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.site24x7.com.",
              "path": [
                "monitor_groups/:monitor_group_id"
              ],
              "query": [
                {
                  "key": "display_name\n        \n        \n            required\n            Display Name for the Monitor Group.\n        \n    \n    \n        \n        description\n        \n        \n            optional\n            Description for the Monitor Group.",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "monitor_group_id",
                  "value": "monitor_group_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update an existing Monitor Group."
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "cefe78a1-e637-47ad-8d75-372d649962f0"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "f2df6767-cd6a-421d-a40b-2059c7606687"
            }
          ]
        }
      ]
    }
  ]
}