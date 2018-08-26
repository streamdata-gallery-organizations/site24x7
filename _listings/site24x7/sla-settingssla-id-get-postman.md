{
  "info": {
    "name": "SLA Setting API Get SLA Report",
    "_postman_id": "dbe514ec-885c-481f-99b8-89a8f85de916",
    "description": "Retrieve the configuration of a SLA Report.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "SLA Settings",
      "item": [
        {
          "id": "390a6df0-dc83-4647-8967-9a5a40a74301",
          "name": "get-sla-report",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.site24x7.com.",
              "path": [
                "sla_settings/:sla_id"
              ],
              "variable": [
                {
                  "id": "sla_id",
                  "value": "sla_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve the configuration of a SLA Report."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5aea46ae-6877-4dba-b40f-32ecad10e5eb"
            }
          ]
        }
      ]
    }
  ]
}