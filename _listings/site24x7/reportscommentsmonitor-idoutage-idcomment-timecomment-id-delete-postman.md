{
  "info": {
    "name": "Report API Delete comment",
    "_postman_id": "15c50b3e-1a2d-43d2-95a2-c255419eb623",
    "description": "Delete an outage comment.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Reports",
      "item": [
        {
          "id": "4a840322-9807-483d-b063-c99d72d03de4",
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
              "id": "f4e42dd5-c368-43d8-bf0e-74962fb1d960"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "a8c07f2e-bc2c-4fe9-b835-8b3667f451fd"
            }
          ]
        },
        {
          "id": "456f0813-95a9-4f29-8146-6b767a074127",
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
              "id": "e9e109f2-11c4-4696-9563-b24df3f878b2"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "c0a8cae9-7dce-475c-a4d6-08637e4944bf"
            }
          ]
        },
        {
          "id": "b8481ee7-ea04-401c-8fa1-8831ea991caf",
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
              "id": "a8d6c1d9-8090-4c75-9be5-2438eed9aba1"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "b59be49c-e83d-4ec9-bd14-9f76b42308e5"
            }
          ]
        },
        {
          "id": "316ec5b3-d5b5-446d-8412-6ac9ea038aa8",
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
              "id": "8460e9ad-4dfc-42e4-8a37-f8b6216436eb"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "9c27e853-da9e-468a-b120-c5e4f2d7a5e3"
            }
          ]
        },
        {
          "id": "efe7b817-123f-470f-b8fa-d2bd1b0bc6a8",
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
              "id": "c542c6ad-27be-4c51-a969-6d2e4d3f2788"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "4a8a0b4e-d79c-4c66-9338-6d8ad04ab628"
            }
          ]
        },
        {
          "id": "fa11f462-78ed-40ba-bf6e-dc27c73a7381",
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
              "id": "8b93f4d4-c52f-45e1-802f-18461c5a4de7"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "fb3f9f2c-ecd9-4e90-acd1-bf1a5cd12462"
            }
          ]
        },
        {
          "id": "bfcf4884-2232-4143-99bb-1be439540835",
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
              "id": "e90e4efc-acd2-4d67-a181-a36b68695d87"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "236972ff-fd43-45ec-ac79-15bbea1dd8c5"
            }
          ]
        },
        {
          "id": "07390379-e6c8-48a5-a2c9-09d7d8ff875d",
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
              "id": "9f6db43a-c8a4-4269-a8f6-f36cf3d3c53d"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "52545f0e-9dd9-48d8-b5e6-69eb7f04572c"
            }
          ]
        },
        {
          "id": "440ab635-b092-4be9-a2a7-6347d7e24e4f",
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
              "id": "226e900f-8e71-464b-9e69-ced0114f217b"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "c3daec7a-ec61-4a75-b3a8-dcc955fd0e40"
            }
          ]
        }
      ]
    }
  ]
}