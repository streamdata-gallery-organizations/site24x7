{
  "info": {
    "name": "Report API Performance Report by Monitor group",
    "_postman_id": "91f089be-e86d-4d81-935c-1e343795571f",
    "description": "Request Example",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Reports",
      "item": [
        {
          "id": "75e3503c-f180-446e-941c-43c3e0e6a35e",
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
              "id": "1e1dda9b-81e7-46b8-8404-07216d3d0475"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "8abb8d44-2210-4564-ba85-49e4b1bea845"
            }
          ]
        },
        {
          "id": "2aa7c1e1-3632-4219-b1ee-ee5f6967f820",
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
              "id": "cb53f5b6-a006-4a92-9326-bb5647501f20"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "44065fe0-42d5-4234-9977-a0cb284644c3"
            }
          ]
        },
        {
          "id": "68a23024-d6ef-48d5-b4ce-6cf760a1834d",
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
              "id": "b1f5909a-a54a-4b6c-993e-61d95f5ddebb"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "6e98e03a-ac6f-429e-8727-13e6f4065609"
            }
          ]
        },
        {
          "id": "a1c91d7d-0722-405f-ab71-3508c8619b5c",
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
              "id": "6d39f06a-b363-438a-8613-24a85a16ae7b"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "b8049d54-2d57-44a3-9c8c-7eefc4fc5fe1"
            }
          ]
        },
        {
          "id": "66d7b7e0-35f2-4772-8ce6-817aa05bb163",
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
              "id": "6912f611-9b3a-44c0-8762-bcfd9632c8f9"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "71d060c2-1052-4164-b7be-17f4c0321bf3"
            }
          ]
        },
        {
          "id": "0a2c88f4-32c4-4b3e-a882-33b95ca8e35a",
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
              "id": "06345894-741e-4f1f-875a-7aa2e43b48f1"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "93a2b841-5586-4cde-a6e7-9b54746b5837"
            }
          ]
        },
        {
          "id": "e970e15d-b6d7-4bcb-bb24-dc66df5772cf",
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
              "id": "f95327e7-e831-483f-9133-59eaf58590da"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "14800b18-4454-4ab2-ba35-05ad2b24ad61"
            }
          ]
        },
        {
          "id": "5ec55444-0349-40db-83af-9e411e153904",
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
              "id": "0b3e597c-10f0-4830-9230-e56b6a8c0811"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "b636a9e8-697a-49ec-8ce5-65768ad6cc19"
            }
          ]
        },
        {
          "id": "4f469bfb-aabe-4206-821b-8cb2ce71c253",
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
              "id": "671d0b5f-24ee-4a7b-a384-43c383af6520"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "760df3ae-e0a1-460e-be60-c179e5247067"
            }
          ]
        },
        {
          "id": "33ba98ac-f873-4325-897b-3e4da99744d9",
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
              "id": "5b566229-b07f-42e7-9cc3-f9f06821d74a"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "bf61eb0d-6a7b-4e20-a80d-5af90c4c07c5"
            }
          ]
        },
        {
          "id": "c1bba69a-5b69-43af-8235-38cee56f2bc5",
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
              "id": "4dbf975e-0ea2-418a-8a1d-dff6142d1202"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "561eb945-ca4c-4237-adaf-f99c07da0b31"
            }
          ]
        },
        {
          "id": "c70f577e-d078-42ce-a7af-0d7c7105e861",
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
              "id": "8476f6d4-ccbb-4cf9-8fc8-870a9cf42dd1"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "2e79a265-cd62-4f01-bf10-1ee850731453"
            }
          ]
        },
        {
          "id": "b194aa3b-8ca4-450c-ad1a-b5bec5ebce55",
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
              "id": "1d48bb5a-fe7b-49f0-bf06-2f59a4385a79"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "534b3feb-ba1b-4e0c-8840-264aed362e48"
            }
          ]
        },
        {
          "id": "44c5bc3a-56e9-40b8-8c80-3ef97134cbbe",
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
              "id": "60750c3a-f741-4609-9f8c-525584061e9b"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "1c19eb8e-cecb-4f99-9e1e-34cdde68515b"
            }
          ]
        },
        {
          "id": "7d0755e5-2cfb-4a47-96b5-f10fcc5821af",
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
              "id": "d9d73838-3355-4b2b-a980-b9fa2d5969b1"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "60971e2b-61e6-47b6-bb31-4070ae20b4b5"
            }
          ]
        },
        {
          "id": "95298a11-7da5-445e-95c4-e27b6c21df8d",
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
              "id": "71e8b50b-439f-4661-81b1-02988112a34f"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "e9400e8a-26fc-4a2c-b458-0046f9a3e766"
            }
          ]
        },
        {
          "id": "eed34f61-d858-447f-8bd9-16520d70bfa2",
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
              "id": "e506955d-67bb-4caa-99d7-c5d29a80e5ca"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "4ae7acb3-f61f-4a81-814f-677ba28c16ea"
            }
          ]
        }
      ]
    }
  ]
}