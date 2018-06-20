{
  "info": {
    "name": "Jumpseller Get Products Options",
    "_postman_id": "21a047c6-ef15-4772-937d-b45cd669dc93",
    "description": "",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Products",
      "item": [
        {
          "id": "30dcff8a-3d48-4e34-a0d4-f5302b5a0377",
          "name": "getProductsOptions.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.jumpseller.com",
              "path": [
                "v1",
                "products/:id/options.json"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Products Options"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aba3c3b7-a9c1-4d6f-a483-bb48e34cef37"
            }
          ]
        }
      ]
    }
  ]
}