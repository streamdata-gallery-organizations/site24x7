{
  "info": {
    "name": "Report API Health Trend Report by Monitor group",
    "_postman_id": "f5a9a415-1386-4785-953b-062c86d3de83",
    "description": "Request Example",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Reports",
      "item": [
        {
          "id": "96af692e-8c1c-41f5-ae3d-321d22168bea",
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
              "id": "365a1ee1-4c61-4c4a-bf8e-d6edc2d9f667"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "2588acd2-9d87-4b75-9796-55985b0433d5"
            }
          ]
        },
        {
          "id": "c8c9b71d-2c91-47d5-af4f-642194025237",
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
              "id": "914daa77-8ac9-4e3c-bbc1-02ae0f15983f"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "998ae815-f225-43f8-9fa6-3131c108dc32"
            }
          ]
        },
        {
          "id": "84f6f46c-475c-48f0-a78b-792099318cef",
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
              "id": "6757c3b7-64fb-4216-b033-5817181863e8"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "a01232a3-f714-4e10-955c-ba1455b751e7"
            }
          ]
        },
        {
          "id": "6ab256db-f74c-4f40-b90e-878a7d11521e",
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
              "id": "ba60110a-8826-4648-999f-d56be0a84609"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "f9bb42d3-62aa-463c-89ea-ac4e659eaee2"
            }
          ]
        },
        {
          "id": "da149512-ae1a-484b-91cb-f262d229ccd8",
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
              "id": "a8f9b47d-22a1-4dac-8ed3-cfc30247fc41"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "d61010b6-41dc-4dcd-b6be-fde07fc0cd0a"
            }
          ]
        },
        {
          "id": "11d72150-bf3c-4bb2-80f9-af366c3210ad",
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
              "id": "7cc729aa-38c3-4b80-8b84-680c052c80ca"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "30f6073e-5d07-4578-a0c8-4b4d47c59d2e"
            }
          ]
        },
        {
          "id": "ceb7d83e-4f9c-46b8-a924-0be3d2cb397a",
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
              "id": "a8990749-392b-4b39-b249-c3e34cc58885"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "d1f8ed44-4339-4b32-b2eb-110a02cf94b7"
            }
          ]
        },
        {
          "id": "44bcddcb-a014-4107-a0b4-e746d2f17e29",
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
              "id": "cede459f-1d0f-4642-943c-49b848a07bbc"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "971addbf-221e-499d-84a9-ce4aea1430af"
            }
          ]
        },
        {
          "id": "eb8e0176-138e-4fcc-8d95-7f22bdbce83a",
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
              "id": "5cefa11e-2078-4790-b1b8-e343bf6ce2f1"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "8199bc7b-8c78-415d-bbda-5e0ae5669b5b"
            }
          ]
        },
        {
          "id": "68b0e91e-97f0-4dd1-a7fa-5ae414f8a310",
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
              "id": "79786732-9961-4d02-ad3a-ecc1e9f5d322"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "6bebc836-199f-406a-a874-d2a855981726"
            }
          ]
        },
        {
          "id": "c7b52b71-e593-4a2e-989c-8e5a2b8ca14a",
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
              "id": "ce86c27f-ea2b-4dea-9deb-c15490ed687a"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "6f84f669-9822-4636-baed-f3d7344db5da"
            }
          ]
        },
        {
          "id": "de06d96f-3d87-4cb4-82a6-3570e0bea9fd",
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
              "id": "96d79281-f6db-45f3-a6c7-7b59b2077bab"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "f23e5090-9725-4ca2-a7b9-811302a96195"
            }
          ]
        },
        {
          "id": "0b9c650b-e13b-46e6-8770-9889a3b342de",
          "name": "summary-for-all-monitors",
          "request": {
            "url": "http://www.site24x7.com./reports/summary?period=?availability_percentage=%7B%7D",
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
              "id": "3fe7d79b-d96b-4cc8-9d80-644ec73ec76e"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "9c8f188a-df43-4272-8e6e-65b6ca2388d5"
            }
          ]
        },
        {
          "id": "ce9f0d1f-34af-443c-88a6-690f8c50c220",
          "name": "health-trend-report-by-monitor-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.site24x7.com.",
              "path": [
                "reports/trend/group/:group_id"
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
              "id": "f1023f4a-1d36-4cfa-909d-88762ba1affb"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "efbd6989-26a0-4472-9ca3-8d85b502cbba"
            }
          ]
        }
      ]
    }
  ]
}