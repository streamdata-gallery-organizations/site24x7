{
  "info": {
    "name": "Threshold Profile API Retrieve Threshold Profile",
    "_postman_id": "f4400094-dfdc-4c20-bc01-fb7db751b6b3",
    "description": "Retrieve the configuration of a Threshold profile.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Threshold Profiles",
      "item": [
        {
          "id": "da39ca1a-0ccd-4567-bcb6-87d19b1ac966",
          "name": "retrieve-threshold-profile",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.site24x7.com.",
              "path": [
                "threshold_profiles/:profile_id"
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
            "description": "Retrieve the configuration of a Threshold profile."
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "d505f047-2550-4a0e-bbd4-566f2f051427"
            },
            {
              "status": "",
              "code": 500,
              "name": "Response_500",
              "id": "66dfdddd-cf32-4ece-9c05-e7c81fd0d4f6"
            }
          ]
        }
      ]
    }
  ]
}