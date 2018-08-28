{
  "info": {
    "name": "Jumpseller Get Products Options Count",
    "_postman_id": "5189504d-27d3-49ed-a457-95b84479afbd",
    "description": "",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Countries",
      "item": [
        {
          "id": "2c45140c-f271-40d9-ba9f-6d132d1da9ad",
          "name": "getCountries.json",
          "request": {
            "url": "http://api.jumpseller.com/v1/countries.json?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve all countries.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d41208de-7aaa-4022-b908-7a4ff19274a9"
            }
          ]
        },
        {
          "id": "5e92fff2-dbdd-4f2e-b8b0-054d9f2300d5",
          "name": "getCountriesCountryCode.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.jumpseller.com",
              "path": [
                "v1",
                "countries/:country_code.json"
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
                  "id": "country_code",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve a single country information.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1ab93fe5-810a-49d4-b3ec-e62c623f8cbe"
            }
          ]
        },
        {
          "id": "416f3cf5-22a4-4c04-a84c-96dfea204e20",
          "name": "getCountriesCountryCodeRegions.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.jumpseller.com",
              "path": [
                "v1",
                "countries/:country_code/regions.json"
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
                  "id": "country_code",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve all regions from a single country.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e4b33b80-84ea-42a2-847c-0ee67f3c4bec"
            }
          ]
        },
        {
          "id": "b324262a-fdeb-42a9-ba1d-c808cda24fc6",
          "name": "getCountriesCountryCodeRegionsRegionCode.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.jumpseller.com",
              "path": [
                "v1",
                "countries/:country_code/regions/:region_code.json"
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
                  "id": "country_code",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "region_code",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve a single region information object.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e1280516-3d12-4273-a403-d4124f2dbc8d"
            }
          ]
        }
      ]
    },
    {
      "name": "Products",
      "item": [
        {
          "id": "941b5b3f-03a8-4df6-99bd-8da07b492fdf",
          "name": "getProductsCategoryCategoryCount.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.jumpseller.com",
              "path": [
                "v1",
                "products/category/:category_id/count.json"
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
                  "id": "category_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Products Category Category Count"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "38fdb8a3-c181-4e16-92eb-c0ed8e0a3cd6"
            }
          ]
        },
        {
          "id": "51b197df-f689-460d-861d-4ce076c7cc9d",
          "name": "getProductsCount.json",
          "request": {
            "url": "http://api.jumpseller.com/v1/products/count.json?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Products Count"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ae041339-b9e7-4db3-bb11-e9830bcda572"
            }
          ]
        },
        {
          "id": "a300649a-7fd5-4593-918f-5387b76b6865",
          "name": "getProductsStatusStatusCount.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.jumpseller.com",
              "path": [
                "v1",
                "products/status/:status/count.json"
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
                  "id": "status",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Products Status Status Count"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "09ee44ba-4eb5-4c22-a118-6c99683fb9ac"
            }
          ]
        },
        {
          "id": "c234f34e-a953-4423-9fa2-afe8691a9b30",
          "name": "getProductsFieldsCount.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.jumpseller.com",
              "path": [
                "v1",
                "products/:id/fields/count.json"
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
            "description": "Get Products Fields Count"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f1115807-e379-4ab3-93ec-2f2a3d7e4817"
            }
          ]
        },
        {
          "id": "55bb8d6a-c882-4300-b808-20136f924a48",
          "name": "getProductsImagesCount.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.jumpseller.com",
              "path": [
                "v1",
                "products/:id/images/count.json"
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
            "description": "Get Products Images Count"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c46673bc-d73d-4515-8edd-39133636b947"
            }
          ]
        },
        {
          "id": "de1ed48d-dc40-45db-beb9-633bfb9e525c",
          "name": "getProductsOptionsCount.json",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.jumpseller.com",
              "path": [
                "v1",
                "products/:id/options/count.json"
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
            "description": "Get Products Options Count"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6b4e5045-0cee-41bb-a66d-32dcea74ed15"
            }
          ]
        }
      ]
    }
  ]
}