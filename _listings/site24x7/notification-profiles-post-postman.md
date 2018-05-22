{
  "info": {
    "name": "Notification Profile API Create Notification Profile",
    "_postman_id": "bcf7299e-a7f6-4a44-b4aa-3a053bf0f036",
    "description": "Create a new notification profile.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Notification Profiles",
      "item": [
        {
          "id": "0222fe5d-d9a6-44ca-869b-fad1deb72f41",
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
              "id": "fd77e2cc-e122-4e68-bc5a-415a201b310b"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "06d02e57-d611-447f-9a16-f2cfaf93ab5f"
            }
          ]
        }
      ]
    }
  ]
}