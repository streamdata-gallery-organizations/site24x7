---
swagger: "2.0"
x-collection-name: Site24x7
x-complete: 0
info:
  title: Status Dashboard API Update Status Dashboard
  description: Update the configuration of an existing Status Dashboard.
  version: 1.0.0
host: www.site24x7.com.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /status_dashboards:
    post:
      summary: Create Status Dashboard
      description: Create a new Status Dashboard
      operationId: create-status-dashboard
      x-api-path-slug: status-dashboards-post
      parameters:
      - in: path
        name: "display_name\n        \n        \n            required\n            Display
          name for the Status Dashboard.\n        \n    \n    \n        \n        description\n
          \       \n        \n            optional\n            Description for the
          Status Dashboard."
      responses:
        200:
          description: OK
      tags:
      - Status Dashboards
  /status_dashboards/{report_id}:
    put:
      summary: Update Status Dashboard
      description: Update the configuration of an existing Status Dashboard.
      operationId: update-status-dashboard
      x-api-path-slug: status-dashboardsreport-id-put
      parameters:
      - in: path
        name: "display_name\n        \n        \n            required\n            Display
          name for the Status Dashboard.\n        \n    \n    \n        \n        description\n
          \       \n        \n            optional\n            Description for the
          Status Dashboard."
      responses:
        200:
          description: OK
      tags:
      - Status Dashboards
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