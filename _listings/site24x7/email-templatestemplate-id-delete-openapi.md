---
swagger: "2.0"
x-collection-name: Site24x7
x-complete: 0
info:
  title: Email Template API Delete Email Template
  description: Delete an existing Email Template.
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