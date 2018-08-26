{
  "info": {
    "name": "Update Button API Get Uptime Button",
    "_postman_id": "e6f51aed-dbd1-4c90-8d72-376dbd283f8d",
    "description": "Retrieve the configuration of the Uptime Button.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Uptime Buttons",
      "item": [
        {
          "id": "197b1028-38a4-4b00-96a0-3c907a5798ca",
          "name": "get-uptime-button",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.site24x7.com.",
              "path": [
                "uptime_buttons/:monitor_id"
              ],
              "variable": [
                {
                  "id": "monitor_id",
                  "value": "monitor_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve the configuration of the Uptime Button."
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "736ff457-3e08-4a8e-ae91-1a93d72e52eb"
            },
            {
              "status": "",
              "code": 500,
              "name": "Response_500",
              "id": "db56e89c-881f-4395-81a2-7e2c1f0e1c2d"
            }
          ]
        }
      ]
    }
  ]
}