---
swagger: "2.0"
x-collection-name: Site24x7
x-complete: 0
info:
  title: SLA Setting API Delete SLA Report
  description: Delete the existing SLA Report.
  version: 1.0.0
host: www.site24x7.com.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /sla_settings/{sla_id}:
    get:
      summary: Get SLA Report
      description: Retrieve the configuration of a SLA Report.
      operationId: get-sla-report
      x-api-path-slug: sla-settingssla-id-get
      responses:
        200:
          description: OK
      tags:
      - SLA Settings
    delete:
      summary: Delete SLA Report
      description: Delete the existing SLA Report.
      operationId: delete-sla-report
      x-api-path-slug: sla-settingssla-id-delete
      responses:
        200:
          description: OK
      tags:
      - SLA Settings
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