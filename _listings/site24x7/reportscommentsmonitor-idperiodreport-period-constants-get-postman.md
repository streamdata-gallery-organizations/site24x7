{
  "info": {
    "name": "Report API Get comments for a monitor",
    "_postman_id": "bceddaac-d8d5-4e5c-8b16-37665707a2da",
    "description": "Get all the comments for a monitor for the given duration.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Reports",
      "item": [
        {
          "id": "8e574336-8a1c-4125-8692-f27e2d10ac53",
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
              "id": "7139a177-1471-48ca-b14f-1bc48f4c6639"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "7f65be0c-f1d7-46c4-8490-903d1478c045"
            }
          ]
        },
        {
          "id": "e4e8a790-9f11-4eea-9beb-abef432c4049",
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
              "id": "d488e99a-f59a-4b21-92cc-c4450ab17f2b"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "e872eaa8-56c2-486d-ac80-43d43ba01abd"
            }
          ]
        },
        {
          "id": "8495b158-d5e0-4cd5-89c7-60fffe53cebc",
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
              "id": "c909f97d-7ece-419d-abbc-78f375456c55"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "6b3f5d8c-9385-4e8c-bf67-b38a653e63a8"
            }
          ]
        },
        {
          "id": "b0bfa506-b993-4bef-9573-29b633225770",
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
              "id": "5a71becf-c0f9-4c00-a40b-ae35c3391f2c"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "b1ff1b2b-d4f6-48bc-a5f6-53731cb50178"
            }
          ]
        },
        {
          "id": "c5c806d5-9c20-4716-83d1-cde8a3e4a98b",
          "name": "delete-outage",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.site24x7.com.",
              "path": [
                "reports/outage/:monitor_id/:outage_id"
              ],
              "variable": [
                {
                  "id": "monitor_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "outage_id",
                  "value": "outage_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete the faulty downtime alerts to reflect the actual available state of the monitor."
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "2762f32e-fc95-4c1e-b140-9b464d0920f9"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "235aa561-d852-4d52-9dce-17920bdac916"
            }
          ]
        },
        {
          "id": "ffc1acac-eb3c-4748-b6af-0be1b9e75e6b",
          "name": "get-alarms-of-monitor",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.site24x7.com.",
              "path": [
                "reports/alarm/:monitor_id?period=:report_period_constants"
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
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Obtain the actual down, trouble and maintenance status of your configured monitors. Alert types"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "1d5a097a-3739-4f05-afe1-2461dd601f01"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "c165e7ea-951d-495e-b77f-50deae1e8861"
            }
          ]
        },
        {
          "id": "d8553c1f-95f8-43f3-b895-1a1c3e5f6510",
          "name": "get-comments-for-a-monitor",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.site24x7.com.",
              "path": [
                "reports/comments/:monitor_id?period=:report_period_constants"
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
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get all the comments for a monitor for the given duration."
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "c4bd7f8f-ec05-4332-a9b8-152d624cbb54"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "f2447bd0-1bfc-426a-99ce-e53ff28a7168"
            }
          ]
        }
      ]
    }
  ]
}