{
  "info": {
    "name": "User API Retrieve an user info",
    "_postman_id": "c5056f67-a1ac-452b-826d-ccbcdf044a58",
    "description": "Retrieve information for an existing user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "073684f4-da9d-45ac-b027-4ff277f62325",
      "name": "retrieve-an-user-info",
      "request": {
        "url": {
          "protocol": "http",
          "host": "www.site24x7.com.",
          "path": [
            "users/:user_id"
          ],
          "variable": [
            {
              "id": "user_id",
              "value": "user_id",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "body": {
          "mode": "raw"
        },
        "description": "Retrieve information for an existing user."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "adb2f58d-14d4-4b3b-a3ca-764453f48dfa"
        },
        {
          "status": "",
          "code": 500,
          "name": "Response_500",
          "id": "773970e4-1eff-4d11-ad16-dd8afd5fd40c"
        }
      ]
    }
  ]
}