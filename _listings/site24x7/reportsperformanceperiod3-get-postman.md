{
  "info": {
    "name": "Report API Performance Report of all monitors",
    "_postman_id": "71c983c4-3d69-4bc2-b5b0-88b2f6190f1d",
    "description": "Request Example",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Reports",
      "item": [
        {
          "id": "6d11817d-d60f-447c-9721-231d65a36bdd",
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
              "id": "21d0acf9-19f6-4abc-ac19-f21fa3b1b40a"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "643e71a1-c703-4240-b119-289c05a3fe7d"
            }
          ]
        },
        {
          "id": "4896e9f7-94e3-4232-8da7-e3b12bc25276",
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
              "id": "b7f1d205-72ff-45c6-acc9-aec6dae5e263"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "1a86af7a-1492-4ad9-a1d7-03e455843b49"
            }
          ]
        },
        {
          "id": "da149ca8-44eb-4c4d-819b-fb3792a323ba",
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
              "id": "acdf438e-2972-411d-9efb-314ba3304e8f"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "de0efee9-4fc8-46c8-aa26-6f1d3f066222"
            }
          ]
        },
        {
          "id": "a9694ddb-ba18-45e4-8f6d-79b0e3462384",
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
              "id": "2c4d8359-978f-4be3-acde-77ace5570e98"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "0263eae5-b038-479b-82c1-73fe0b0474eb"
            }
          ]
        },
        {
          "id": "537a8ef6-caa9-4f56-ad0b-c4fb398a2871",
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
              "id": "e8d3f6ee-c97c-46fe-9162-7bf18c9f538b"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "ee3cb654-9ae0-4b20-a4f9-8c119a61cd16"
            }
          ]
        },
        {
          "id": "4d447bef-1021-4140-971e-e252dfe83271",
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
              "id": "55512894-8e53-4f09-a7dd-4197faad8c4b"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "5d471648-fa5c-43d1-afe4-5e98058c2c36"
            }
          ]
        },
        {
          "id": "26a6c9c4-2206-4b1c-8034-e0a76064066f",
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
              "id": "6424985a-3108-4915-97a6-77e5b3e3c777"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "47ee8aa7-4c78-43ed-8d72-06e18c355814"
            }
          ]
        },
        {
          "id": "e2127eae-490e-4377-b4c8-ec258fabf98b",
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
              "id": "b9d3a7d8-ac14-46da-b21e-4edad6f24b99"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "6c8d4dca-1d5e-4311-84ab-495df57733ff"
            }
          ]
        },
        {
          "id": "90cd09ee-22fc-4479-974a-47ebe1fd2aaf",
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
              "id": "04188b85-fb79-4631-9c66-16cbc05aced2"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "ab54f8fc-2ba4-4f36-b3b9-d098316a3dc3"
            }
          ]
        },
        {
          "id": "b4e94240-7e54-4226-9c9e-b74b2d638dff",
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
              "id": "4f461615-3a67-46e4-a22b-54b1c2634e8a"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "99969a86-14e2-43b2-8a42-9fbdb6403e02"
            }
          ]
        },
        {
          "id": "af10d867-2bd7-4d84-8c5e-92c005012f22",
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
              "id": "279e1b79-e9b7-4a06-91b1-f77b2ec2ea6c"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "172da3a0-213c-42a0-80ae-3e121194b3b2"
            }
          ]
        },
        {
          "id": "5ca63749-7443-4811-8fe8-79ebf51f67b8",
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
              "id": "b1d26e8a-981c-4c79-9392-57c0b986aa1b"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "48740ad1-c4b2-4fc4-b426-c50eaa62b274"
            }
          ]
        },
        {
          "id": "8f9bc855-13ca-4eea-bc50-ac74212f92a0",
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
              "id": "cadd18cf-e0b7-448f-b7a0-282b05ca9068"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "e4827d08-9b36-44f4-ad96-363f3fbc497d"
            }
          ]
        },
        {
          "id": "4e10701f-d9e2-4143-bc59-9c446225111a",
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
              "id": "3239c629-47be-44f3-9387-1cd10cf69c9c"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "dad63861-fbc9-49ea-ab2f-229971a66eaf"
            }
          ]
        },
        {
          "id": "b8856c11-f78c-483e-8e07-8ad7a0731246",
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
              "id": "21ab29a0-1ca8-4b1c-b20e-2337a46f1741"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "1701d5c7-10e6-4268-82da-4470659fb659"
            }
          ]
        },
        {
          "id": "b0dfea64-8b1c-47af-83d6-d6bc848596d2",
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
              "id": "f3b03ebe-bce2-409e-a9fd-b221f17b4f04"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "9bc64392-f7cb-4101-ad12-1edec1a25271"
            }
          ]
        },
        {
          "id": "639c143a-6d42-49a7-8d20-52216f6b3763",
          "name": "performance-report-by-monitor-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.site24x7.com.",
              "path": [
                "reports/performance/group/:group_id?period=3"
              ],
              "query": [
                {
                  "key": "name",
                  "value": "%7B%7D",
                  "disabled": false
                }
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
              "id": "84730fe3-1c59-43a5-a064-f213f3138fa4"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "47849c13-aadd-4345-8ba1-19688660b862"
            }
          ]
        },
        {
          "id": "9a7ad2ac-a132-4762-9d69-5a4743d65552",
          "name": "performance-report-of-all-monitors",
          "request": {
            "url": "http://www.site24x7.com./reports/performance?period=3?period=%7B%7D",
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
              "id": "23d20a6c-d62d-45d7-82d3-eb4868c5f18f"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "dd677850-68df-46c6-8f12-e6211c578f11"
            }
          ]
        }
      ]
    }
  ]
}