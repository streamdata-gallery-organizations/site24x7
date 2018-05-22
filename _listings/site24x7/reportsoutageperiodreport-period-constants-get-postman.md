{
  "info": {
    "name": "Report API Get Outage Details",
    "_postman_id": "13d37fc1-4e67-49f1-97be-9a3eb24ec2b0",
    "description": "Obtain the actual down period and the total down duration of your monitors for a specified duration of time.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Reports",
      "item": [
        {
          "id": "b5bd9c3c-4e76-4cbf-b123-82d704495085",
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
              "id": "f3421930-3fc1-41ea-be89-7f1aeb71302f"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "65870151-46bf-4066-8d1d-3fab7e3efa98"
            }
          ]
        },
        {
          "id": "77397fd9-f7a4-4b23-9bd2-d0019e64286c",
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
              "id": "f8f63881-0dac-47b6-a1cd-c7dd056f37f5"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "bc33614d-a4a0-4dcf-ac15-37d97b3f7094"
            }
          ]
        },
        {
          "id": "1d8deeb0-7986-4949-b7a5-ddf0b2ce2729",
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
              "id": "d564f4d1-1a0f-4984-9efd-c806510d2125"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "289ecb31-34f5-4600-ab8f-07f7912e2070"
            }
          ]
        }
      ]
    }
  ]
}