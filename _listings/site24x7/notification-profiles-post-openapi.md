---
swagger: "2.0"
x-collection-name: Site24x7
x-complete: 0
info:
  title: Notification Profile API Create Notification Profile
  description: Create a new notification profile.
  version: 1.0.0
host: www.site24x7.com.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
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