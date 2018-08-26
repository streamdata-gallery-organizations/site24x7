{
  "info": {
    "name": "Report API Get Custom Report Settings",
    "_postman_id": "11c417e5-15d8-49dc-bb43-a967c07c99d5",
    "description": "Retrieve Custom Report Settings.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Reports",
      "item": [
        {
          "id": "4be784b1-b77f-4f73-9b0e-5b64bd4d7770",
          "name": "get-custom-report-settings",
          "request": {
            "url": "http://www.site24x7.com./customize_report",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve Custom Report Settings."
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "d210f404-2891-41c7-9050-b142b1bfd254"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "836c7060-7ec2-40be-970c-3fe1eb2bc68f"
            }
          ]
        }
      ]
    }
  ]
}