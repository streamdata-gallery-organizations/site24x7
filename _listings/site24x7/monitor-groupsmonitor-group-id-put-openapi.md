---
swagger: "2.0"
x-collection-name: Site24x7
x-complete: 0
info:
  title: Monitor Group API Update a Monitor Group
  description: Update an existing Monitor Group.
  version: 1.0.0
host: www.site24x7.com.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /monitor_groups:
    post:
      summary: Create a Monitor Group
      description: Create a new Monitor Group.
      operationId: create-a-monitor-group
      x-api-path-slug: monitor-groups-post
      parameters:
      - in: path
        name: "display_name\n        \n        \n            required\n            Display
          Name for the Monitor Group.\n        \n    \n    \n        \n        description\n
          \       \n        \n            optional\n            Description for the
          Monitor Group."
      responses:
        Maximum record size:
          description: 100 KiB
        Maximum number of records per datastore:
          description: "100,000"
        Maximum datastore size:
          description: 10 MiB
        Maximum size of a delta:
          description: 2 MiB
      tags:
      - Monitor Groups
  /monitor_groups/{monitor_group_id}:
    put:
      summary: Update a Monitor Group
      description: Update an existing Monitor Group.
      operationId: update-a-monitor-group
      x-api-path-slug: monitor-groupsmonitor-group-id-put
      parameters:
      - in: path
        name: "display_name\n        \n        \n            required\n            Display
          Name for the Monitor Group.\n        \n    \n    \n        \n        description\n
          \       \n        \n            optional\n            Description for the
          Monitor Group."
      responses:
        Maximum record size:
          description: 100 KiB
        Maximum number of records per datastore:
          description: "100,000"
        Maximum datastore size:
          description: 10 MiB
        Maximum size of a delta:
          description: 2 MiB
      tags:
      - Monitor Groups
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---