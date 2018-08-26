{
  "info": {
    "name": "Report API Summary for all monitors",
    "_postman_id": "985dc7f4-bafa-4d1c-9b1b-e59fd5a04c4b",
    "description": "Request Example",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Reports",
      "item": [
        {
          "id": "e26ee977-1c47-4a73-b61f-0fa54b9d5f62",
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
              "id": "d6029f04-f2e4-495b-ac08-f99d0c213d2d"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "73c670c6-f4a6-404f-841d-3dbd7fe4f2a3"
            }
          ]
        },
        {
          "id": "361d8385-a932-4228-90c0-2afe9a02b51b",
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
              "id": "fae78284-d33a-4df4-8a64-3e6adf0f5e40"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "3048afd9-d195-4ac7-a6df-2ab3541a4643"
            }
          ]
        },
        {
          "id": "fbb8a08a-daad-41e7-9237-37b62c44d4b3",
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
              "id": "3dd31380-dbd1-4e34-a3d6-28388056ec93"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "a592314a-621e-460a-b593-66a8965a1553"
            }
          ]
        },
        {
          "id": "faacd2bb-b9bf-4219-8a95-a99974d1b23f",
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
              "id": "466fefc9-5da5-46c7-8d86-24b7a054e2bf"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "ebf21d9b-c327-48b1-a178-ffb113b5cc8a"
            }
          ]
        },
        {
          "id": "b9fb36d0-e316-4abe-b04e-be935be6c75f",
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
              "id": "da7377b6-b606-43d3-90e6-170778478d00"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "79a325ab-3a0e-40cb-8ce9-c24a9ecec019"
            }
          ]
        },
        {
          "id": "9c785b19-8316-4492-bd5d-2be33510865e",
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
              "id": "c3a89143-fa8c-45be-8e8f-091de0246ad6"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "a119aaf3-f32f-4de3-8819-b31a24454e5d"
            }
          ]
        },
        {
          "id": "7752481c-0331-4200-a7a4-e3eee591142d",
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
              "id": "f1b24061-37ae-4bcd-bb6b-56fb5b244007"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "713f02fa-d12a-41dd-8516-63cf02b90dc4"
            }
          ]
        },
        {
          "id": "506741c7-9f0f-451d-8c01-a43cd313fb2a",
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
              "id": "0f9de42d-04ac-4114-9453-503ae6a58271"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "d2684e75-1bb6-4f47-bbb1-7b559c52dd8d"
            }
          ]
        },
        {
          "id": "ce344f0d-a27c-4406-bb17-3393cdcc95d6",
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
              "id": "fc499507-ae3a-4d3e-aa64-271fa2052390"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "cc47a56b-c90d-4e8c-8c6a-176eaf7505df"
            }
          ]
        },
        {
          "id": "4d68e0df-1843-4e30-9532-aefe243019b0",
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
              "id": "b13d1b42-a1cd-4167-8672-153029753b99"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "ef68b28d-4440-46a2-ab85-9e71efba78df"
            }
          ]
        },
        {
          "id": "b52e8c20-b76c-42ea-8885-58db6525e59a",
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
              "id": "2d003f3b-8877-4170-9ebd-bdfd45c1f91c"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "9d96f1fd-c52c-4801-9dce-45426205fb58"
            }
          ]
        },
        {
          "id": "cdde2b5d-3246-45f9-9acc-5cf4e0ec00b8",
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
              "id": "a0778858-9e4a-4fd7-9817-d1cb4c0bf1e3"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "7b0dd2a6-11d4-4172-9a7f-a3b9b0eeb902"
            }
          ]
        },
        {
          "id": "664e88e5-eba8-4640-bafd-df395c2addec",
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
              "id": "70901a97-47cc-49b2-be30-084ab1c008b8"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "ea685def-78ef-4459-9af1-e9c8e09e0d82"
            }
          ]
        }
      ]
    }
  ]
}