{
  "info": {
    "name": "Report API Busy Hours Report",
    "_postman_id": "72c1ea11-3aa1-421e-93e3-bf2203f6d326",
    "description": "Request Example",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Reports",
      "item": [
        {
          "id": "d92b4f1f-3683-4876-a553-cb0cc6abea15",
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
              "id": "62c65d1f-2f6e-4652-83e6-8bd9be2ce6dc"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "54884f66-f5a1-42cf-b5b6-9b8fbf1adbc0"
            }
          ]
        },
        {
          "id": "4da7a6a5-0209-46ee-adf3-8273835ebd9d",
          "name": "busy-hours-report",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.site24x7.com.",
              "path": [
                "reports/busy_hours/:monitor_id?period=:report_period_constants&segment_type=:segment_types"
              ],
              "variable": [
                {
                  "id": "monitor_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "report_period_constants",
                  "value": "report_period_constants",
                  "type": "string"
                },
                {
                  "id": "segment_types",
                  "value": "segment_types",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Request Example"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "c511b151-c17c-4764-9c45-6f07db4c3a14"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "d4c90f05-3d62-4958-b449-daa51723e48a"
            }
          ]
        }
      ]
    }
  ]
}