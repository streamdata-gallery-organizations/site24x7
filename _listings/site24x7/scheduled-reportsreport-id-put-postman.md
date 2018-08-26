{
  "info": {
    "name": "Scheduled Report API Update Scheduled Report",
    "_postman_id": "46f60ef2-7373-493e-8b4d-2a814f7b896c",
    "description": "Update the configuration of an existing Scheduled Report.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Scheduled Reports",
      "item": [
        {
          "id": "d20e5d31-ef09-4d25-92e6-93d10a50cb2b",
          "name": "schedule-a-report",
          "request": {
            "url": "http://www.site24x7.com./scheduled_reports?display_name\n        \n        \n            required\n            Display name for the Report.\n        \n    \n    \n        \n        report_type\n        \n        \n            required\n            Type of report to be Scheduled.Report Constants=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Schedule a report to be received on a specific day and time."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3cd5979d-4559-4710-9d85-c53718511af5"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "83a3b0de-7b0b-4836-8b00-bc383bcd565b"
            }
          ]
        },
        {
          "id": "7de3f7fc-3efd-4563-8680-76d41aa6d7bb",
          "name": "update-scheduled-report",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.site24x7.com.",
              "path": [
                "scheduled_reports/:report_id"
              ],
              "query": [
                {
                  "key": "display_name\n        \n        \n            required\n            Display name for the Report.\n        \n    \n    \n        \n        report_type\n        \n        \n            required\n            Type of report to be Scheduled.Report Constants",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "report_id",
                  "value": "report_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update the configuration of an existing Scheduled Report."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b159279f-a647-4314-9a88-c66734faabad"
            }
          ]
        }
      ]
    }
  ]
}