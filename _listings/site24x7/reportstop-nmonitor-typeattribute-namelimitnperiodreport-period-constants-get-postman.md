{
  "info": {
    "name": "Report API Top N Report by monitor and attribute type",
    "_postman_id": "29b37ffc-6255-44c4-ade6-0cd7c77ae384",
    "description": "Request Example",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Reports",
      "item": [
        {
          "id": "e9f52e06-1478-45f4-9e5d-7310949cd6b9",
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
              "id": "855c8a8b-f2e6-4a1b-8728-9f14566f8c14"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "d40622f6-dc9c-45a4-8eb3-ff5ba611d0ec"
            }
          ]
        },
        {
          "id": "41398e52-c836-4eb1-9e7f-a6265c7020c4",
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
              "id": "3cb95d59-94da-4c0a-a469-0ce82933355c"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "564747c1-f521-47f9-b26d-33b923a83926"
            }
          ]
        },
        {
          "id": "eb974b18-abc8-42dd-a496-7c180f1725da",
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
              "id": "f6aae87a-3957-4665-99f1-ba4124c11aa9"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "c65d55b0-0653-48b0-b0b1-8958b63582ce"
            }
          ]
        },
        {
          "id": "26da6569-a092-4bf3-96c4-9ed3025a05d1",
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
              "id": "1ded3210-d98e-4c04-9547-05e2ea06e29d"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "2560323a-cf59-4f6b-8a8e-4eeeee38b79c"
            }
          ]
        },
        {
          "id": "84f8e026-fcbe-4d4b-9192-96e04a2d8cc0",
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
              "id": "66542923-f75d-49e9-bcaa-d25ccbc70c9b"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "493a0a9e-e012-4669-8601-f367289883cd"
            }
          ]
        },
        {
          "id": "69d8c438-555c-457e-8d97-a863d2cb9fc9",
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
              "id": "5f622f05-713f-4be8-bda3-e61003acaf6c"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "701daea4-8a3f-4efa-b8f4-5b7bd2fc6bcb"
            }
          ]
        },
        {
          "id": "b887e892-d203-411c-ae5a-cf30fd98b308",
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
              "id": "bcbef72a-e3cd-4ab9-8e12-d27ca623b3ca"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "0f6c559b-a386-40f9-8017-6082efc669fa"
            }
          ]
        },
        {
          "id": "a9a012a3-c200-4837-b6f3-5d270eed31ef",
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
              "id": "5af1b836-6d8d-4693-a4cb-a360eee16524"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "1563ec87-2cbc-4997-a895-4acb7ef067df"
            }
          ]
        },
        {
          "id": "d74948b4-c69e-471c-93c9-f2a08896814d",
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
              "id": "38155b1c-62ea-4789-8106-98aecdf9bb54"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "0fba3ea3-11d1-47b8-b943-450bc24255ff"
            }
          ]
        },
        {
          "id": "4a701506-8766-47ae-bf87-154a15880ee8",
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
              "id": "0184a369-583f-4071-b151-b4b3e9217c2b"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "f1c4e597-c72b-43a0-aaa2-f9b403370082"
            }
          ]
        },
        {
          "id": "1051bb46-a829-455d-a445-9c6db100c8a4",
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
              "id": "68920a60-f296-4229-a361-e7a48c5b8b7f"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "31f5c20c-e0ea-4d51-8756-8681055be703"
            }
          ]
        },
        {
          "id": "8a0b6ae9-d9af-440b-a7c0-f894da7fce7f",
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
              "id": "1872beac-e3b0-48e2-a9f9-cd1d7a81b8c3"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "c25284c0-160f-464d-982e-6fa9a7a17ad9"
            }
          ]
        },
        {
          "id": "3932a878-1a09-4a8c-aabc-3c09df572943",
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
              "id": "b5e73b97-a467-4a2e-be21-547ef0894a0f"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "8830255e-9908-4dcf-94a4-b3578e8c32ad"
            }
          ]
        },
        {
          "id": "523d5ad2-8bb5-4a08-b92f-ae9ac53de045",
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
              "id": "223e2a07-d6c8-422f-b74b-8523be300e53"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "6cf75fe5-9be8-4070-b805-94d074671fe0"
            }
          ]
        },
        {
          "id": "e91f077d-11d1-43a8-ab1b-5a2a86e3ba22",
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
              "id": "708434bb-2841-4b4a-8fa1-5b8450f2ecf3"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "d4072e20-0521-47a8-9ea3-f8c48ff42c02"
            }
          ]
        },
        {
          "id": "c74bf30a-7313-4021-824d-af3e0ea06b8f",
          "name": "top-n-report-by-monitor-and-attribute-type",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.site24x7.com.",
              "path": [
                "reports/top_n/:monitor_type/:attribute_name?limit=:N&period=:report_period_constants"
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
                  "id": "monitor_type",
                  "value": "monitor_type",
                  "type": "string"
                },
                {
                  "id": "attribute_name",
                  "value": "attribute_name",
                  "type": "string"
                },
                {
                  "id": "N",
                  "value": "N",
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
            "description": "Request Example"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "9f250140-61fe-49d5-90f7-48868e2fa7d3"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "ff968f8f-e3aa-4ea8-8801-922a110b312a"
            }
          ]
        }
      ]
    }
  ]
}