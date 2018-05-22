{
  "info": {
    "name": "Maintenance API Retrieve Maintenance",
    "_postman_id": "a9d30589-7080-4970-9aa6-2649b1cdaa15",
    "description": "Retrieve configuration of a Scheduled Maintenance.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Maintenance",
      "item": [
        {
          "id": "fc4f3338-4132-44e4-a501-e8a8ab8d7e09",
          "name": "retrieve-maintenance",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.site24x7.com.",
              "path": [
                "maintenance/:maintenance_id"
              ],
              "variable": [
                {
                  "id": "maintenance_id",
                  "value": "maintenance_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve configuration of a Scheduled Maintenance."
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "a2aad6b1-0326-44b4-926c-19db75d240af"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "4d65838e-8179-40bd-ac85-b9aec44b505c"
            }
          ]
        }
      ]
    }
  ]
}