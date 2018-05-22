{
  "info": {
    "name": "Report API Update outage comments.",
    "_postman_id": "0a301126-92a7-401d-bebd-605652625d1b",
    "description": "Update the comment for a given monitor.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Reports",
      "item": [
        {
          "id": "23519495-7692-415d-84d3-2cbca63019f9",
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
              "id": "888a5917-03c3-4003-8130-9222c22c4607"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "cbfd007c-ed98-4791-8cc6-0a11e4ed4953"
            }
          ]
        },
        {
          "id": "1aff8e87-a535-4812-b61d-28cd2b822033",
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
              "id": "237e6aa3-f1bc-404f-84b0-5eee5e07511f"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "cc61bc73-3331-4b55-8451-8d6b97dcd7ef"
            }
          ]
        },
        {
          "id": "f4136499-81bf-438b-9aad-5db2e533ef69",
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
              "id": "3d3f2de3-c537-4eb1-98ee-b52ba514ded9"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "7cd8ce6e-d95e-4438-a07c-8a561aa9248a"
            }
          ]
        },
        {
          "id": "5df0e7ce-2151-428a-898e-adaea568cff3",
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
              "id": "a50bfde2-41bb-47e4-b80f-007da9aef309"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "05de0dd5-1b19-4a6d-b186-dcf13d12b88b"
            }
          ]
        },
        {
          "id": "1a3ccfe0-8802-485d-9976-77e29fae9ff9",
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
              "id": "83ae3b63-9c40-405c-8c3e-8174eb6d9d7a"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "76b258d5-dfe7-4652-99ac-fb2ea9409f28"
            }
          ]
        },
        {
          "id": "0085f5e9-c132-4af1-8614-a9a6d04226c0",
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
              "id": "01f47da0-252f-4d5a-b24a-98052d04d05e"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "5a6dda75-b49a-4380-a47e-f938e07cf137"
            }
          ]
        },
        {
          "id": "be4a0e39-ebdf-4e0f-bde5-e0a1683b2f97",
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
              "id": "3ca50614-0fd8-4424-bb9d-eac1f2f2a4c3"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "612b2013-1a33-4571-942d-6ca0b284145c"
            }
          ]
        },
        {
          "id": "a8560692-2089-48ee-a71a-237417789d25",
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
              "id": "7ddbb217-756f-4f11-9eec-a6d5348e217b"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "2bc5d692-8055-4fd9-977b-5ef051099c89"
            }
          ]
        }
      ]
    }
  ]
}