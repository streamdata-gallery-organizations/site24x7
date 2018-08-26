{
  "info": {
    "name": "Scheduled Report API Schedule a Report",
    "_postman_id": "7852e0ce-512b-4d44-bd26-bc5bc7018ed4",
    "description": "Schedule a report to be received on a specific day and time.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Scheduled Reports",
      "item": [
        {
          "id": "f92e4e29-a806-4b05-82d9-fef16c45e2c7",
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
              "id": "0b92c5e7-b8da-4c3c-8c37-4a612cf2dec2"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "ec64bf13-df5b-4fb9-9897-1a365fdf3385"
            }
          ]
        }
      ]
    }
  ]
}