{
  "info": {
    "name": "User Group API Create a new user group",
    "_postman_id": "2e6b51e9-8394-4358-952e-026c7674a86e",
    "description": "Create a new user group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "ca43dfc2-02c4-4826-b997-61fbcb63b486",
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
          "id": "60dab05d-ed14-4329-b238-e2cd368811b6"
        },
        {
          "status": "",
          "code": 500,
          "name": "Response_500",
          "id": "8d37df4f-6c30-4fdd-a434-bdd1a72de676"
        }
      ]
    }
  ]
}