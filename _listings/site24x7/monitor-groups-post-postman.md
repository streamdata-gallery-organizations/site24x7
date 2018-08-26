{
  "info": {
    "name": "Monitor Group API Create a Monitor Group",
    "_postman_id": "801418ae-ab9c-4f57-bbae-61707a767c37",
    "description": "Create a new Monitor Group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Monitor Groups",
      "item": [
        {
          "id": "08756196-00ce-42f1-b3bf-1944a49a2e88",
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
              "id": "379a84ea-eb66-43bf-9a27-2395053ceb7a"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "63ad88e4-bb0c-4fab-8bb6-d9b6fbc14400"
            }
          ]
        }
      ]
    }
  ]
}