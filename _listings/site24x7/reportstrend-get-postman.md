{
  "info": {
    "name": "Report API Health trend Report for all monitors",
    "_postman_id": "83acf06c-6abb-4c7b-882a-22c4844d2ff9",
    "description": "Request Example",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Reports",
      "item": [
        {
          "id": "55284995-00ec-4018-8ad2-b8e5ce134532",
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
              "id": "a4c28793-dd00-4866-8310-3f8430078d1e"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "b5751781-fdbb-4db0-aec4-760d852cef00"
            }
          ]
        },
        {
          "id": "ef91b06e-2ab0-450a-9579-fbbfef20c726",
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
              "id": "1f797fdd-3437-4660-9f07-279238430a52"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "c354d4e0-519a-4370-9ce2-3198587daa1b"
            }
          ]
        },
        {
          "id": "b1bff4f3-4eac-4624-8c34-6077023687e6",
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
              "id": "60d6e01e-ca94-452d-be01-2110c32a36a8"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "15b9648c-7e0b-45ae-a992-a6d51684f275"
            }
          ]
        },
        {
          "id": "419db92d-4582-44ba-94df-75aadeb7ecd8",
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
              "id": "b8b9ed29-5e06-464a-bc5e-8722ba363706"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "bcb0b2d2-08af-435d-80f5-a38041efb062"
            }
          ]
        },
        {
          "id": "20219cce-78ad-43d8-8394-2e5e0bd2eb7c",
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
              "id": "dfdbe301-7dc8-411b-92db-e9637f14254a"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "1c31d740-069e-431e-aa70-926c53326cb4"
            }
          ]
        },
        {
          "id": "753326b8-39bf-4369-845d-37e18afbb63d",
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
              "id": "92d24fbb-813c-412a-997a-115f091e0692"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "154d7842-c701-4bd2-aff7-5d66e2785ca8"
            }
          ]
        },
        {
          "id": "4c0d7583-f8b5-4274-b53e-06846799b4c7",
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
              "id": "f3fe494f-7341-4501-bd47-9b662ec0b012"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "bc0a5dd9-9163-45ed-884c-118e9d3257d9"
            }
          ]
        },
        {
          "id": "ebd9c744-9796-4069-b0a1-9f97c7e4e619",
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
              "id": "178e126c-8f0d-49fe-8531-45ed98982c2f"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "1bc6fb2c-d946-4982-ad34-6861c0478c46"
            }
          ]
        },
        {
          "id": "b71b8bee-ffd8-4d4a-976d-048e898ace8a",
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
              "id": "ff95d26c-54e0-48c9-b81f-7235c439fea0"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "2c710a1a-3b8f-4d3d-bb22-2f6004978752"
            }
          ]
        },
        {
          "id": "853a8852-d43e-42d2-9a85-234513381274",
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
              "id": "1b5d24d1-0a6d-4eae-98b6-255e18e8994f"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "f694ec51-4468-4265-8875-5593a1b21afe"
            }
          ]
        },
        {
          "id": "c5a6176a-a0a9-432b-ba41-2bb5b09af21c",
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
              "id": "cdd4a27e-ef60-456e-b625-5e5e697935d0"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "f3b0fbc2-20ba-4f95-8c57-73b968f9539a"
            }
          ]
        },
        {
          "id": "595ee34f-068f-4b06-a5ad-4b099a5a4fb5",
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
              "id": "9952c881-2b7b-4fff-a84e-30ce751a04df"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "1ea4af95-0d48-438f-8fbb-6e1515e86fe8"
            }
          ]
        },
        {
          "id": "09fd7633-c2fb-4def-abd5-4ea1cb8bfc9e",
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
              "id": "13b61867-51c3-479e-9016-6e94e5e235b0"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "d3643408-3926-4310-92c1-14b9eae10909"
            }
          ]
        },
        {
          "id": "a2d7f2d0-3898-45c4-8f7a-38e7ec7055e6",
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
              "id": "2b39a4a6-36dd-4c31-87ee-ee46c664ef2f"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "58a73177-7292-4b0f-af99-b59b2d0aa815"
            }
          ]
        },
        {
          "id": "cf34f086-0edf-4461-9b30-86d7fe836f51",
          "name": "health-trend-report-for-all-monitors",
          "request": {
            "url": "http://www.site24x7.com./reports/trend?period=%7B%7D",
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
              "id": "844bebb0-b585-4487-9ed8-88f648cd8f94"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "5c86415e-e828-497c-9003-0d8428af05f7"
            }
          ]
        }
      ]
    }
  ]
}