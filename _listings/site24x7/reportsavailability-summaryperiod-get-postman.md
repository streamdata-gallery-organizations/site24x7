{
  "info": {
    "name": "Report API Availability Summary for all monitors",
    "_postman_id": "305db7f6-94bc-4717-bff6-93e7120cdba0",
    "description": "Request Example",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Reports",
      "item": [
        {
          "id": "f2762dd5-e5a5-42a0-b70a-2e54c066bfca",
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
              "id": "bdcce25c-0815-4880-ac80-3f7daa13de07"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "ce6d027d-f31a-4992-860a-3e74db80bfbd"
            }
          ]
        },
        {
          "id": "17ef1d65-ed1e-4084-ba72-0823eb6106e8",
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
              "id": "fe8fcf2d-a664-44af-b93f-038a8e20d57e"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "bbe721fa-4747-4961-a30c-ca36beec1d43"
            }
          ]
        },
        {
          "id": "ce434032-ad8f-4528-aa88-538c9e974ed5",
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
              "id": "2308590c-4467-4bdd-86ad-560376866298"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "ef2cf705-857b-4996-8a5b-58bb9b4da540"
            }
          ]
        },
        {
          "id": "533bdb59-6a61-4322-808a-281cb4155a28",
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
              "id": "7f6e683a-3f8a-4456-b843-e2621507ea3c"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "b1f3c162-d05e-4fa5-b68a-564da179f559"
            }
          ]
        },
        {
          "id": "185bc752-0842-4ab2-8664-9454c2529490",
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
              "id": "6f021206-ddb7-420c-a6cd-d0bb1d901e6b"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "f28254ab-9340-489a-a8fd-9662cb31836a"
            }
          ]
        },
        {
          "id": "c90cadd9-678f-434e-a734-87da8089ef20",
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
              "id": "c2e1013a-e51e-426a-b281-3aab30a12d45"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "55ec6f9f-f200-467c-8690-c5c9005b2dd6"
            }
          ]
        },
        {
          "id": "5d29e0a0-be6a-49c4-9496-fd7c07744bdf",
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
              "id": "39e486bd-3311-4745-9aa4-5e09bc7707ae"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "ca8cd36d-590b-464b-8720-f5b23b1ee6cf"
            }
          ]
        },
        {
          "id": "8e561e82-57ee-45c3-b7a7-ad1c0357edff",
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
              "id": "0b1134fa-0b7f-4ecd-ae6f-95a27084a4be"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "16e48f23-ec68-41c3-8a3e-bbbc99701951"
            }
          ]
        },
        {
          "id": "0d3e6357-a4c5-4bd9-a007-90caf1bf645c",
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
              "id": "0a212858-f100-4c48-bbb1-932ef98489a6"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "f2d8ecdb-8be4-4f3e-9b40-42d8f26297d7"
            }
          ]
        },
        {
          "id": "12f7dd09-7d6d-4868-96d9-8be15034fefe",
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
              "id": "de852a96-0795-43aa-adf6-4669687fdcac"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "0919c72c-f626-4d9b-b0ab-9f1ed7ad1773"
            }
          ]
        },
        {
          "id": "f22210d3-0a18-46df-bb04-e9ef26309d6a",
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
              "id": "91adf660-f8f4-42a2-ace3-ab7b260e8c9a"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "9e4e6c13-52d4-4505-b504-58fcd2b4ad92"
            }
          ]
        }
      ]
    }
  ]
}