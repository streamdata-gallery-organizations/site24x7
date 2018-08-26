{
  "info": {
    "name": "Report API Summary by monitor group",
    "_postman_id": "65a53de3-342a-40a2-a5d6-ee942f828b08",
    "description": "Request Example",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Reports",
      "item": [
        {
          "id": "60b52bd3-1b39-4750-bc21-f661500dc393",
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
              "id": "83964041-59e5-4190-9600-8de6b97278c9"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "b1cc030a-9e51-445f-925c-a08d42a25b59"
            }
          ]
        },
        {
          "id": "f5da623d-7192-4e29-80ab-5a5dcfcbfcb6",
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
              "id": "db6eb3e3-097d-42ff-887d-35e26294d3c0"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "4149aec6-c7e5-4b80-82a1-a37025f55b0b"
            }
          ]
        },
        {
          "id": "1e14b6c9-aa44-42fe-98fb-d32d1b454aa6",
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
              "id": "99b5e37b-b002-4274-93e3-359076b1b8d9"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "3b464982-ae2b-4488-a265-5eba7f40fc17"
            }
          ]
        },
        {
          "id": "1a7f76a7-4f93-4325-ae6a-f55da08c31c1",
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
              "id": "c86ddf94-4694-4df1-849d-4f527962c74d"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "0cb49d92-4be1-45e2-a8a2-189ff6ff6b42"
            }
          ]
        },
        {
          "id": "03553a79-ce38-4e31-b746-f8030082c775",
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
              "id": "ad81f824-804f-40ab-9e0d-755ab68fd662"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "b97e13dd-eca3-4566-9a5f-ca347beefbf6"
            }
          ]
        },
        {
          "id": "1a4347a7-ee31-47c4-aae8-e88365025792",
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
              "id": "51d5d068-39db-4e80-83c1-e0a0e6cc2589"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "952ccb69-40ba-4469-b481-6338f9b10bae"
            }
          ]
        },
        {
          "id": "14776802-3275-44f0-b549-9a103d9bd269",
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
              "id": "e1e301e2-3479-4a0d-939e-4752ae828363"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "cf97fdab-6151-44f7-b983-194a0ef4ca4f"
            }
          ]
        },
        {
          "id": "a284984a-2e00-428c-8019-74810b937b9a",
          "name": "update-outage-comments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.site24x7.com.",
              "path": [
                "reports/comments/:monitor_id/:outage_id"
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
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update the comment for a given monitor."
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "ac51c214-f7f0-42bd-8d48-1931663f64b3"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "cc4c1703-2a8e-4952-8d2e-ba372c9c1a59"
            }
          ]
        },
        {
          "id": "9d957367-9726-413a-8a0b-6ae5d8e681bf",
          "name": "delete-comment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.site24x7.com.",
              "path": [
                "reports/comments/:monitor_id/:outage_id?comment_time=:comment_id"
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
                },
                {
                  "id": "comment_id",
                  "value": "comment_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete an outage comment."
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "7a3c4327-573b-417e-b25f-90a9c47781e5"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "270e2970-0783-4afd-8776-5d755cefa2d0"
            }
          ]
        },
        {
          "id": "b99c2148-42bc-4be6-9532-be74b43bf1f2",
          "name": "availability-summary-by-monitor-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.site24x7.com.",
              "path": [
                "reports/availability_summary/group/:group_id?period="
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
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
              "id": "2bac48af-3f96-4b8f-a641-29835ac0fac2"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "31924038-8ffe-46f2-9fce-3aa46997ee38"
            }
          ]
        },
        {
          "id": "89624d22-565c-42b2-9266-5d0d082d9c4d",
          "name": "availability-summary-for-all-monitors",
          "request": {
            "url": "http://www.site24x7.com./reports/availability_summary?period=?period=%7B%7D",
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
              "id": "fa46ef6d-6dc4-4c80-8fb0-c367dd26309c"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "b08fc87a-5186-4da9-8c94-799f1b10dc0c"
            }
          ]
        },
        {
          "id": "db77c595-4f8d-4c09-819e-8a2c28848908",
          "name": "summary-by-monitor-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.site24x7.com.",
              "path": [
                "reports/summary/group/:group_id?period="
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
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
              "id": "434dbeb7-849c-449a-b33f-ce1e9498e3e3"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "c8e00b13-82e7-4de7-9cb7-cc45269a8c07"
            }
          ]
        }
      ]
    }
  ]
}