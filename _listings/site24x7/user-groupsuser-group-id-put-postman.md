{
  "info": {
    "name": "User Group API Update an user group details",
    "_postman_id": "c5447bec-dd32-41c1-9a79-bd2f014024c0",
    "description": "Update an existing User Group Information.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "beacbba0-1ecd-488c-bb6e-a0d51bafe81e",
      "name": "create-a-new-user-group",
      "request": {
        "url": "http://www.site24x7.com./user_groups?display_name\n        \n        \n            required\n            Display name for the user group.\n        \n    \n    \n        \n        users\n        \n        \n            required\n            Users to be associated for the group.=%7B%7D",
        "method": "POST",
        "body": {
          "mode": "raw"
        },
        "description": "Create a new user group."
      },
      "response": [
        {
          "code": 200,
          "name": "Response_200",
          "id": "0bfc5a95-5ac3-4a69-a621-f9ddb3c0c7fb"
        },
        {
          "status": "",
          "code": 500,
          "name": "Response_500",
          "id": "66825d52-67fc-4d2a-8951-de9a628bbc08"
        }
      ]
    },
    {
      "id": "43d51e3b-1c90-45b3-839f-62aee648d2aa",
      "name": "update-an-user-group-details",
      "request": {
        "url": {
          "protocol": "http",
          "host": "www.site24x7.com.",
          "path": [
            "user_groups/:user_group_id"
          ],
          "query": [
            {
              "key": "display_name\n        \n        \n            required\n            Display name for the user group.\n        \n    \n    \n        \n        users\n        \n        \n            required\n            Users to be associated for the group.",
              "value": "%7B%7D",
              "disabled": false
            }
          ],
          "variable": [
            {
              "id": "user_group_id",
              "value": "user_group_id",
              "type": "string"
            }
          ]
        },
        "method": "PUT",
        "body": {
          "mode": "raw"
        },
        "description": "Update an existing User Group Information."
      },
      "response": [
        {
          "code": 200,
          "name": "Response_200",
          "id": "21869027-4280-4196-ac3d-503ca37e7a64"
        },
        {
          "status": "",
          "code": 500,
          "name": "Response_500",
          "id": "c299686e-e979-4bcc-b508-fd32ae3bda9f"
        }
      ]
    }
  ]
}