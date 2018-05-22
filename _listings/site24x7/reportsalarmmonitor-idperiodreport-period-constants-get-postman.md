{
  "info": {
    "name": "Report API Get Alarms of Monitor",
    "_postman_id": "cc4c26bd-5da6-4f6f-a832-3c162aa92c65",
    "description": "Obtain the actual down, trouble and maintenance status of your configured monitors. Alert types",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Reports",
      "item": [
        {
          "id": "cb3c529b-5c23-43d9-9262-8de676092fcd",
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
              "id": "aaba0f78-177d-4c17-9a71-098f325d3915"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "417e130a-eb9e-4827-b403-93e599b4bad4"
            }
          ]
        },
        {
          "id": "17041ac5-7edd-483c-bbe9-52fdc0f799ad",
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
              "id": "e76527c2-cc99-4f98-b162-99e3a48b3be5"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "e0f50642-04b1-4e03-8916-c7f3c6a77947"
            }
          ]
        },
        {
          "id": "6cac56f8-fc01-494b-b411-204a1bdb2a50",
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
              "id": "0add5e46-4509-48f7-9d05-edebdd874d12"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "1948b77c-1a86-4ab5-8dff-455e68339b95"
            }
          ]
        },
        {
          "id": "b348af43-058f-4b88-902f-0445386662bc",
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
              "id": "5b1d30a6-77a1-4849-95ee-f55160cd03dc"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "584898e4-9118-4582-b34b-09616b6f56df"
            }
          ]
        },
        {
          "id": "aa615040-7d3e-4d51-91f1-6c8556199a17",
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
              "id": "4bee4f90-d82b-402f-af67-dfa072fd663f"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "e27e00ca-1840-4bad-9f16-fd264f63ea1c"
            }
          ]
        },
        {
          "id": "5d39a3ee-9ef1-4bb6-b436-0a16a5c81bd6",
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
              "id": "cce18806-69e8-4188-b1c3-590d8970b812"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "dbf63c67-796f-40e9-8aab-e7ce89660962"
            }
          ]
        }
      ]
    }
  ]
}