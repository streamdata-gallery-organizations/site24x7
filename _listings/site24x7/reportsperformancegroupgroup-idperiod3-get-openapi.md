---
swagger: "2.0"
x-collection-name: Site24x7
x-complete: 0
info:
  title: Report API Performance Report by Monitor group
  description: Request Example
  version: 1.0.0
host: www.site24x7.com.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /business_hours:
    post:
      summary: Create Business Hour
      description: Create a new Business Hour.
      operationId: create-business-hour
      x-api-path-slug: business-hours-post
      parameters:
      - in: path
        name: "display_name\n        \n        \n            required\n            Display
          name for the Business Hour.\n        \n    \n    \n        \n        description\n
          \       \n        \n            optional\n            Description for the
          Business Hour"
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
      - Business Hours
    get:
      summary: List Business Hours
      description: List of all Business Hours.
      operationId: list-business-hours
      x-api-path-slug: business-hours-get
      parameters:
      - in: path
        name: "background_color\n        \n        \n            string\n            Back
          ground color for your reports.\n        \n                \n    \n        \n
          \       foreground_color\n        \n        \n            string\n            Foreground
          ground color for your r"
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
      - Business Hours
  /business_hours/{business_hours_id}:
    put:
      summary: Update Business Hour
      description: Update an existing Business Hour.
      operationId: update-business-hour
      x-api-path-slug: business-hoursbusiness-hours-id-put
      parameters:
      - in: path
        name: "display_name\n        \n        \n            required\n            Display
          name for the Business Hour.\n        \n    \n    \n        \n        description\n
          \       \n        \n            optional\n            Description for the
          Business Hour"
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
      - Business Hours
  /current_status/{monitor_id}:
    get:
      summary: Current Status of Monitor
      description: Request Example
      operationId: current-status-of-monitor
      x-api-path-slug: current-statusmonitor-id-get
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
      - Current Status
  /current_status/type/{monitor_type}:
    get:
      summary: Current Status by Monitor Type
      description: Request Example
      operationId: current-status-by-monitor-type
      x-api-path-slug: current-statustypemonitor-type-get
      parameters:
      - in: path
        name: monitor_type
        description: MandatoryType of the monitor
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
      - Current Status
  /email_templates/{template_id}:
    get:
      summary: Retrieve Email Template
      description: Retrieve configuration of a Email Template.
      operationId: retrieve-email-template
      x-api-path-slug: email-templatestemplate-id-get
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
      - Email Templates
    delete:
      summary: Delete Email Template
      description: Delete an existing Email Template.
      operationId: delete-email-template
      x-api-path-slug: email-templatestemplate-id-delete
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
      - Email Templates
  /location_profiles/{profile_id}:
    get:
      summary: Retrieve Location Profile
      description: Retrieve configuration of a location profile.
      operationId: retrieve-location-profile
      x-api-path-slug: location-profilesprofile-id-get
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
      - Location Profiles
    delete:
      summary: Delete Location Profile
      description: Delete an existing location profile.
      operationId: delete-location-profile
      x-api-path-slug: location-profilesprofile-id-delete
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
      - Location Profiles
  /maintenance/{maintenance_id}:
    get:
      summary: Retrieve Maintenance
      description: Retrieve configuration of a Scheduled Maintenance.
      operationId: retrieve-maintenance
      x-api-path-slug: maintenancemaintenance-id-get
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
      - Maintenance
    delete:
      summary: Delete Maintenance
      description: Delete an existing Scheduled Maintenance.
      operationId: delete-maintenance
      x-api-path-slug: maintenancemaintenance-id-delete
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
      - Maintenance
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
    get:
      summary: List of all Monitor Groups
      description: List of all Monitor Groups.
      operationId: list-of-all-monitor-groups
      x-api-path-slug: monitor-groups-get
      parameters:
      - in: path
        name: "user_id\n        \n        \n            string\n            Unique
          ID generated by the server. This can be used as an identifier.\n        \n
          \               \n    \n        \n        display_name\n        \n        \n
          \           string\n            Name of the U"
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
  /notification_profiles:
    post:
      summary: Create Notification Profile
      description: Create a new notification profile.
      operationId: create-notification-profile
      x-api-path-slug: notification-profiles-post
      parameters:
      - in: path
        name: "profile_name\n        \n        \n            required\n            Display
          name for the location profile.\n        \n    \n    \n        \n        downtime_notification_delay\n
          \       \n        \n            optional\n            Configuration for
          delayed notifi"
      responses:
        Maximum record size:
          description: 100 KiB
        Maximum number of records per datastore:
          description: "100,000"
        Maximum datastore size:
          description: 10 MiB
        Maximum size of a delta:
          description: 2 MiB
        200:
          description: OK
      tags:
      - Notification Profiles
    get:
      summary: List Notification Profiles
      description: List of all notification profiles.
      operationId: list-notification-profiles
      x-api-path-slug: notification-profiles-get
      parameters:
      - in: path
        name: "template_id\n        \n        \n            string\n            Unique
          ID generated by the server. This can be used as an identifier.\n        \n
          \               \n    \n        \n        display_name\n        \n        \n
          \           string\n            Display n"
      responses:
        200:
          description: OK
      tags:
      - Notification Profiles
  /notification_profiles/{profile_id}:
    put:
      summary: Update Notification Profile
      description: Update an existing notification profile
      operationId: update-notification-profile
      x-api-path-slug: notification-profilesprofile-id-put
      parameters:
      - in: path
        name: "profile_name\n        \n        \n            required\n            Display
          name for the location profile.\n        \n    \n    \n        \n        downtime_notification_delay\n
          \       \n        \n            optional\n            Configuration for
          delayed notifi"
      responses:
        200:
          description: OK
      tags:
      - Notification Profiles
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
    get:
      summary: List Operations Dashboards
      description: List of all Operations Dashboards.
      operationId: list-operations-dashboards
      x-api-path-slug: operations-dashboards-get
      responses:
        200:
          description: OK
      tags:
      - Operation Dashboards
  /operations_dashboards/{dashboard_id}:
    put:
      summary: Update Operations Dashboard
      description: Update the configuration of an existing Operations Dashboard.
      operationId: update-operations-dashboard
      x-api-path-slug: operations-dashboardsdashboard-id-put
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
  /reports/outage/{monitor_id}/{outage_id}:
    delete:
      summary: Delete Outage
      description: Delete the faulty downtime alerts to reflect the actual available
        state of the monitor.
      operationId: delete-outage
      x-api-path-slug: reportsoutagemonitor-idoutage-id-delete
      parameters:
      - in: path
        name: monitor_id
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
  /reports/alarm/{monitor_id}?period={report_period_constants}:
    get:
      summary: Get Alarms of Monitor
      description: Obtain the actual down, trouble and maintenance status of your
        configured monitors. Alert types
      operationId: get-alarms-of-monitor
      x-api-path-slug: reportsalarmmonitor-idperiodreport-period-constants-get
      parameters:
      - in: path
        name: monitor_id
        description: MandatoryMonitor ID
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
  /reports/comments/{monitor_id}?period={report_period_constants}:
    get:
      summary: Get comments for a monitor
      description: Get all the comments for a monitor for the given duration.
      operationId: get-comments-for-a-monitor
      x-api-path-slug: reportscommentsmonitor-idperiodreport-period-constants-get
      parameters:
      - in: path
        name: monitor_id
        description: MandatoryMonitor ID
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
  /reports/comments/{monitor_id}/{outage_id}:
    put:
      summary: Update outage comments.
      description: Update the comment for a given monitor.
      operationId: update-outage-comments
      x-api-path-slug: reportscommentsmonitor-idoutage-id-put
      parameters:
      - in: path
        name: monitor_id
        description: MandatoryMonitor ID
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
  /reports/comments/{monitor_id}/{outage_id}?comment_time={comment_id}:
    delete:
      summary: Delete comment
      description: Delete an outage comment.
      operationId: delete-comment
      x-api-path-slug: reportscommentsmonitor-idoutage-idcomment-timecomment-id-delete
      parameters:
      - in: path
        name: monitor_id
        description: MandatoryMonitor ID
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
  /reports/availability_summary/group/{group_id}?period=:
    get:
      summary: Availability Summary by monitor group
      description: Request Example
      operationId: availability-summary-by-monitor-group
      x-api-path-slug: reportsavailability-summarygroupgroup-idperiod-get
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
  /reports/availability_summary?period=:
    get:
      summary: Availability Summary for all monitors
      description: Request Example
      operationId: availability-summary-for-all-monitors
      x-api-path-slug: reportsavailability-summaryperiod-get
      parameters:
      - in: path
        name: period
        description: Availability and performance details are generated within this
          predefined interval
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
  /reports/summary/group/{group_id}?period=:
    get:
      summary: Summary by monitor group
      description: Request Example
      operationId: summary-by-monitor-group
      x-api-path-slug: reportssummarygroupgroup-idperiod-get
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
  /reports/summary?period=:
    get:
      summary: Summary for all monitors
      description: Request Example
      operationId: summary-for-all-monitors
      x-api-path-slug: reportssummaryperiod-get
      parameters:
      - in: path
        name: availability_percentage
        description: Gives the total availability percentage of the monitor for the
          month
        type: <td>float</td>
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
  /reports/trend/group/{group_id}:
    get:
      summary: Health Trend Report by Monitor group
      description: Request Example
      operationId: health-trend-report-by-monitor-group
      x-api-path-slug: reportstrendgroupgroup-id-get
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
  /reports/trend:
    get:
      summary: Health trend Report for all monitors
      description: Request Example
      operationId: health-trend-report-for-all-monitors
      x-api-path-slug: reportstrend-get
      parameters:
      - in: path
        name: period
        description: Top N report is generated within this predefined interval
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
  /reports/top_n/{monitor_type}/{attribute_name}?limit={N}&period={report_period_constants}:
    get:
      summary: Top N Report by monitor and attribute type
      description: Request Example
      operationId: top-n-report-by-monitor-and-attribute-type
      x-api-path-slug: reportstop-nmonitor-typeattribute-namelimitnperiodreport-period-constants-get
      parameters:
      - in: path
        name: period
        description: Performance details report is generated within this predefined
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
  /reports/performance/group/{group_id}?period=3:
    get:
      summary: Performance Report by Monitor group
      description: Request Example
      operationId: performance-report-by-monitor-group
      x-api-path-slug: reportsperformancegroupgroup-idperiod3-get
      parameters:
      - in: path
        name: name
        description: It contains the name of all the monitors in the group
        type: <td>string array</td>
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