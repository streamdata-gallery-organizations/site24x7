{
  "info": {
    "name": "Email Template API Retrieve Email Template",
    "_postman_id": "52afe264-9ca3-463d-bed6-386d0229da81",
    "description": "Retrieve configuration of a Email Template.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Email Templates",
      "item": [
        {
          "id": "1d65f9c9-8088-44b5-b2e9-a781d3a30294",
          "name": "retrieve-email-template",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.site24x7.com.",
              "path": [
                "email_templates/:template_id"
              ],
              "variable": [
                {
                  "id": "template_id",
                  "value": "template_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve configuration of a Email Template."
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "cf15d191-7c66-4a81-ae67-a80f02e4fe74"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "d208fed0-fc71-424d-a213-de15fecc5a9c"
            }
          ]
        }
      ]
    }
  ]
}