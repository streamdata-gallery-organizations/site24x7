---
swagger: "2.0"
x-collection-name: Site24x7
x-complete: 0
info:
  title: Update Button API Get Uptime Button
  description: Retrieve the configuration of the Uptime Button.
  version: 1.0.0
host: www.site24x7.com.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /uptime_buttons/{monitor_id}:
    get:
      summary: Get Uptime Button
      description: Retrieve the configuration of the Uptime Button.
      operationId: get-uptime-button
      x-api-path-slug: uptime-buttonsmonitor-id-get
      responses:
        '400: for badly-formed requests, e.g. missing or invalid parameters':
          description: ""
        '403: for authentication issues':
          description: ""
        '409: for issues where the request is well-formed but cannot be completed':
          description: ""
      tags:
      - Uptime Buttons
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