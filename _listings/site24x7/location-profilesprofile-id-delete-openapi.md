---
swagger: "2.0"
x-collection-name: Site24x7
x-complete: 0
info:
  title: Location Profile API Delete Location Profile
  description: Delete an existing location profile.
  version: 1.0.0
host: www.site24x7.com.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
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