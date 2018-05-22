{
  "info": {
    "name": "Report API Delete Outage",
    "_postman_id": "0fc2a491-dbd7-4430-b5b0-03bb4cff8d55",
    "description": "Delete the faulty downtime alerts to reflect the actual available state of the monitor.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Reports",
      "item": [
        {
          "id": "15ce5673-10d7-4508-909d-5f8fc5a1a97a",
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
              "id": "c4b1b514-e6b2-4ebe-9795-a47f1c2ca185"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "8886d680-7f8a-4849-a822-b0bdd0aae766"
            }
          ]
        },
        {
          "id": "882988c5-02d0-4a5c-b9ce-3f036e62a003",
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
              "id": "7f677138-959c-4cd4-ac97-4115a84e3604"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "93e5d8cb-e0ea-47d2-9824-01d3f64413f0"
            }
          ]
        },
        {
          "id": "cdd7cca5-7073-40c4-b911-619b37c7815a",
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
              "id": "e472ffc7-6a07-45fe-a2b7-4c76cf620c83"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "8c3b484b-9dc7-4935-b38c-9f8e079314f3"
            }
          ]
        },
        {
          "id": "1004b7e7-737f-44ae-a989-944bf45384c2",
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
              "id": "b9586f97-5b1b-48c9-afa5-270e519b5b41"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "3525506a-0662-4701-bc19-78f107192e3f"
            }
          ]
        },
        {
          "id": "4e52a0a0-38a5-40a9-997e-7216b596bfe3",
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
              "id": "2f0b9833-f7f0-4a46-91b3-d01c0d6bccaa"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "d0dd8ac2-c1bd-4e37-8d67-944814179484"
            }
          ]
        }
      ]
    }
  ]
}