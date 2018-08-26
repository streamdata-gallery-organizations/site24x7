---
swagger: "2.0"
x-collection-name: Site24x7
x-complete: 0
info:
  title: Business Hours API Update Business Hour
  description: Update an existing Business Hour.
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