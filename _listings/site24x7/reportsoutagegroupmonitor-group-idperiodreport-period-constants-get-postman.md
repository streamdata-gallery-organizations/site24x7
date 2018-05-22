{
  "info": {
    "name": "Report API Get Outage Details of Monitor Groups",
    "_postman_id": "14b9f23f-9609-4083-8bdf-be1b06c2f7dd",
    "description": "Obtain the actual down period and the total down duration of your chosen monitor group during a selected duration of time.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Reports",
      "item": [
        {
          "id": "33e62146-0243-46e2-ad23-a6479290caab",
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
              "id": "4725f614-8a59-4ea6-a0f9-f3bc769f25e4"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "ca8c0401-9037-4534-9b76-ab08055d79de"
            }
          ]
        },
        {
          "id": "5e3e207d-6426-4797-a7ee-1ea91b489aa8",
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
              "id": "3d644f51-5738-4267-9531-70c7957a1f57"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "7f1e3f4d-16bc-4421-aa89-57edb957345c"
            }
          ]
        },
        {
          "id": "c1402b04-b78a-4743-85b8-e1f97a74b978",
          "name": "get-outage-details",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.site24x7.com.",
              "path": [
                "reports/outage?period=:report_period_constants"
              ],
              "query": [
                {
                  "key": "period",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "report_period_constants",
                  "value": "report_period_constants",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Obtain the actual down period and the total down duration of your monitors for a specified duration of time."
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "fd362096-89f2-4a8b-a46b-de6a68220598"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "0622e19d-0fed-4c55-b44f-fd4861f0eff0"
            }
          ]
        },
        {
          "id": "d61f31b9-ba5b-49eb-bbfb-7fd7b9e95055",
          "name": "get-outage-details-of-monitor-groups",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.site24x7.com.",
              "path": [
                "reports/outage/group/:monitor_group_id?period=:report_period_constants"
              ],
              "variable": [
                {
                  "id": "monitor_group_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "report_period_constants",
                  "value": "report_period_constants",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Obtain the actual down period and the total down duration of your chosen monitor group during a selected duration of time."
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "0f968b94-c7bb-4f8d-b883-dbc952864e24"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "a166d1b4-e6f1-4a0a-b562-294fc4397e66"
            }
          ]
        }
      ]
    }
  ]
}