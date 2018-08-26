---
swagger: "2.0"
x-collection-name: Site24x7
x-complete: 0
info:
  title: Threshold Profile API Delete Threshold Profile
  description: Delete an existing Threshold profile.
  version: 1.0.0
host: www.site24x7.com.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /threshold_profiles/{profile_id}:
    get:
      summary: Retrieve Threshold Profile
      description: Retrieve the configuration of a Threshold profile.
      operationId: retrieve-threshold-profile
      x-api-path-slug: threshold-profilesprofile-id-get
      responses:
        '400: for badly-formed requests, e.g. missing or invalid parameters':
          description: ""
        '403: for authentication issues':
          description: ""
        '409: for issues where the request is well-formed but cannot be completed':
          description: ""
      tags:
      - Threshold Profiles
    delete:
      summary: Delete Threshold Profile
      description: Delete an existing Threshold profile.
      operationId: delete-threshold-profile
      x-api-path-slug: threshold-profilesprofile-id-delete
      responses:
        '400: for badly-formed requests, e.g. missing or invalid parameters':
          description: ""
        '403: for authentication issues':
          description: ""
        '409: for issues where the request is well-formed but cannot be completed':
          description: ""
      tags:
      - Threshold Profiles
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