{
  "info": {
    "name": "Report API Availability Summary by monitor group",
    "_postman_id": "2f29c560-ec3e-4dc9-a245-a0f4a1197190",
    "description": "Request Example",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Reports",
      "item": [
        {
          "id": "4d3d44f4-883d-40be-9c2c-648faf2a7d37",
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
              "id": "92014ab4-144a-4da3-b923-d18713988a95"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "c4e80e0f-49e5-40f9-90c0-d351217af5e0"
            }
          ]
        },
        {
          "id": "f09db12c-d407-436a-bf52-1d220fcf8f4c",
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
              "id": "4ca8d892-be84-47a8-b268-7d25ae005511"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "ca18a49e-2626-4bdf-a9b9-e26422f04dcf"
            }
          ]
        },
        {
          "id": "2484f40b-e89f-4daa-abcc-9c5d041d9994",
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
              "id": "c24685a8-237a-4feb-9644-39e43273fecc"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "758212b6-be5c-488f-88ca-d96c1f5017f9"
            }
          ]
        },
        {
          "id": "76dec95f-2159-4864-b450-5a1c823b7752",
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
              "id": "53e1d458-28a6-4360-82b1-c8ee8f99f95d"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "2093047a-0836-4392-917b-ee21cc3328c0"
            }
          ]
        },
        {
          "id": "9e27507f-b97c-47d5-a345-cbe7058673dd",
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
              "id": "89eb3b9c-fff4-40f9-9379-4c2b24287c6d"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "5fb354ff-9bdf-4d56-88c7-9e9d219e297b"
            }
          ]
        },
        {
          "id": "37667dd3-b3ec-4cb1-8915-166d0229cc3b",
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
              "id": "67b89bdb-2ff3-4145-a74b-3c443fd81aa6"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "f77a4b11-473d-4c40-9889-7966853e7f47"
            }
          ]
        },
        {
          "id": "55db6574-33ab-4b44-a7ee-3261d2450de0",
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
              "id": "d5a675a1-1010-42ef-866b-455215d39490"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "004c310a-f1c4-4062-af19-af797078d728"
            }
          ]
        },
        {
          "id": "620e018f-96e2-4da6-bb8b-46af197a6ab2",
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
              "id": "a86e643d-a437-4d19-b355-7e32bc903ed5"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "52b465b3-9676-4e9c-95a0-53f9dc4230a3"
            }
          ]
        },
        {
          "id": "5bd67328-3a9f-46a1-acd1-0d715a175692",
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
              "id": "66dc5c7c-643c-47e8-8a0a-3565eeef5c7c"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "0c8008dd-f513-4002-a2d6-2d4d532abf75"
            }
          ]
        },
        {
          "id": "001836cd-dff1-47be-9103-490d50cba833",
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
              "id": "ae9c3cd4-b188-4d69-975c-b023e4105e37"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "96e33e85-f259-467f-8bca-02df7fe4a0b1"
            }
          ]
        }
      ]
    }
  ]
}