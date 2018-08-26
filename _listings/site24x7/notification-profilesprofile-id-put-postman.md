{
  "info": {
    "name": "Notification Profile API Update Notification Profile",
    "_postman_id": "1403f5a9-636d-488e-9e23-d3a1623c0956",
    "description": "Update an existing notification profile",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Notification Profiles",
      "item": [
        {
          "id": "ea10cde2-6675-4136-a4d0-46bf61df63df",
          "name": "create-notification-profile",
          "request": {
            "url": "http://www.site24x7.com./notification_profiles?profile_name\n        \n        \n            required\n            Display name for the location profile.\n        \n    \n    \n        \n        downtime_notification_delay\n        \n        \n            optional\n            Configuration for delayed notifi=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a new notification profile."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "60ef2e40-b05c-4981-a7e9-03d654ec4ccf"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "9072c953-b740-4d64-8c6e-7138e6adffdf"
            }
          ]
        },
        {
          "id": "af9e20f2-26ff-4a88-8f65-f3119b98392c",
          "name": "update-notification-profile",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.site24x7.com.",
              "path": [
                "notification_profiles/:profile_id"
              ],
              "query": [
                {
                  "key": "profile_name\n        \n        \n            required\n            Display name for the location profile.\n        \n    \n    \n        \n        downtime_notification_delay\n        \n        \n            optional\n            Configuration for delayed notifi",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "profile_id",
                  "value": "profile_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update an existing notification profile"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8740d1bb-d086-4d88-837a-44f8414e1646"
            }
          ]
        }
      ]
    }
  ]
}