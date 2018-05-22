{
  "info": {
    "name": "Location Profile API Retrieve Location Profile",
    "_postman_id": "d428b6c7-0934-4c66-8e91-cd183acc1178",
    "description": "Retrieve configuration of a location profile.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Location Profiles",
      "item": [
        {
          "id": "68d9ecd2-81ed-4df2-90ca-6ce62adaeca0",
          "name": "retrieve-location-profile",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.site24x7.com.",
              "path": [
                "location_profiles/:profile_id"
              ],
              "variable": [
                {
                  "id": "profile_id",
                  "value": "profile_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve configuration of a location profile."
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "6a6e24f3-91f1-4b88-9742-57a6e0c1b483"
            },
            {
              "status": "100 KiB",
              "code": 500,
              "name": "Response_500",
              "id": "5dc7c24c-7f38-4b9b-8908-e083e2be9943"
            }
          ]
        }
      ]
    }
  ]
}