---
swagger: "2.0"
x-collection-name: Site24x7
x-complete: 0
info:
  title: Operation Dashboard API Update Operations Dashboard
  description: Update the configuration of an existing Operations Dashboard.
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