{
  "info": {
    "name": "Business Hours API Create Business Hour",
    "_postman_id": "95a3fe75-6029-442b-82bd-78e1c28f0d6d",
    "description": "Create a new Business Hour.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Business Hours",
      "item": [
        {
          "id": "e0b85de6-8607-4979-a9d1-638af84f5c5a",
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
              "id": "65a637ff-1bac-406b-b229-e91739690fe0"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "178bfde9-c157-440a-9e36-773abdb33d07"
            }
          ]
        }
      ]
    }
  ]
}