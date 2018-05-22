---
swagger: "2.0"
x-collection-name: Site24x7
x-complete: 0
info:
  title: Operation Dashboard API Create Operations Dashboard
  description: Create a new Operations Dashboard
  version: 1.0.0
host: www.site24x7.com.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /operations_dashboards:
    post:
      summary: Create Operations Dashboard
      description: Create a new Operations Dashboard
      operationId: create-operations-dashboard
      x-api-path-slug: operations-dashboards-post
      parameters:
      - in: path
        name: "display_name\n        \n        \n            required\n            Display
          name for the Operations Dashboard.\n        \n    \n    \n        \n        layout_type\n
          \       \n        \n            required\n            Layout to be used
          for the Operations Dashboa"
      responses:
        200:
          description: OK
      tags:
      - Operation Dashboards
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