---
swagger: "2.0"
x-collection-name: Site24x7
x-complete: 0
info:
  title: Report API Get Outage Details of Monitor Groups
  description: Obtain the actual down period and the total down duration of your chosen
    monitor group during a selected duration of time.
  version: 1.0.0
host: www.site24x7.com.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /customize_report:
    get:
      summary: Get Custom Report Settings
      description: Retrieve Custom Report Settings.
      operationId: get-custom-report-settings
      x-api-path-slug: customize-report-get
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
      - Reports
  /reports/busy_hours/{monitor_id}?period={report_period_constants}&segment_type={segment_types}:
    get:
      summary: Busy Hours Report
      description: Request Example
      operationId: busy-hours-report
      x-api-path-slug: reportsbusy-hoursmonitor-idperiodreport-period-constantssegment-typesegment-types-get
      parameters:
      - in: path
        name: monitor_id
        description: MandatoryUnique ID of the monitor
        type: <td>string</td>
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
      - Reports
  /reports/outage?period={report_period_constants}:
    get:
      summary: Get Outage Details
      description: Obtain the actual down period and the total down duration of your
        monitors for a specified duration of time.
      operationId: get-outage-details
      x-api-path-slug: reportsoutageperiodreport-period-constants-get
      parameters:
      - in: path
        name: period
        description: Mandatory Outage details report is generated within this predefined
          interval
        type: <td>int</td>
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
      - Reports
  /reports/outage/group/{monitor_group_id}?period={report_period_constants}:
    get:
      summary: Get Outage Details of Monitor Groups
      description: Obtain the actual down period and the total down duration of your
        chosen monitor group during a selected duration of time.
      operationId: get-outage-details-of-monitor-groups
      x-api-path-slug: reportsoutagegroupmonitor-group-idperiodreport-period-constants-get
      parameters:
      - in: path
        name: monitor_group_id
        description: MandatoryMonitor group ID
        type: <td>string</td>
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
      - Reports
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