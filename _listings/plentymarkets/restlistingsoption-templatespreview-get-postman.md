{
  "info": {
    "name": "Plentymarkets Get a preview list of option templates",
    "_postman_id": "344d2e7c-f8d4-4efe-9f28-951e02c820de",
    "description": "Gets a preview list of all available listing option templates.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Preview",
      "item": [
        {
          "id": "9aab829d-31b4-4923-9380-fd70b2553a74",
          "name": "getRestListingsOptionTemplatesPreview",
          "request": {
            "url": "http://example.com/rest/listings/option_templates/preview",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets a preview list of all available listing option templates."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7532827e-7fc7-4965-95e6-2c1a65438bf4"
            }
          ]
        }
      ]
    }
  ]
}