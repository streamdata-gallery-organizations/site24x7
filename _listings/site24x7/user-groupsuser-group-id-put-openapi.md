---
swagger: "2.0"
x-collection-name: Site24x7
x-complete: 0
info:
  title: User Group API Update an user group details
  description: Update an existing User Group Information.
  version: 1.0.0
host: www.site24x7.com.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user_groups:
    post:
      summary: Create a new user group
      description: Create a new user group.
      operationId: create-a-new-user-group
      x-api-path-slug: user-groups-post
      parameters:
      - in: path
        name: "display_name\n        \n        \n            required\n            Display
          name for the user group.\n        \n    \n    \n        \n        users\n
          \       \n        \n            required\n            Users to be associated
          for the group."
      responses:
        '400: for badly-formed requests, e.g. missing or invalid parameters':
          description: ""
        '403: for authentication issues':
          description: ""
        '409: for issues where the request is well-formed but cannot be completed':
          description: ""
      tags:
      - ""
  /user_groups/{user_group_id}:
    put:
      summary: Update an user group details
      description: Update an existing User Group Information.
      operationId: update-an-user-group-details
      x-api-path-slug: user-groupsuser-group-id-put
      parameters:
      - in: path
        name: "display_name\n        \n        \n            required\n            Display
          name for the user group.\n        \n    \n    \n        \n        users\n
          \       \n        \n            required\n            Users to be associated
          for the group."
      responses:
        '400: for badly-formed requests, e.g. missing or invalid parameters':
          description: ""
        '403: for authentication issues':
          description: ""
        '409: for issues where the request is well-formed but cannot be completed':
          description: ""
      tags:
      - ""
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