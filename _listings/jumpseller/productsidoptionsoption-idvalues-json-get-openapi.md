---
swagger: "2.0"
x-collection-name: Jumpseller
x-complete: 0
info:
  title: Jumpseller Get Products Options Option Values
  description: ""
  version: "1"
host: api.jumpseller.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /products/{id}/options.json:
    get:
      summary: Get Products Options
      description: ""
      operationId: getProductsOptions.json
      x-api-path-slug: productsidoptions-json-get
      parameters:
      - in: path
        name: id
        description: ID of the Product
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Products
      - Id
      - Options
      - Json
    post:
      summary: Post Products Options
      description: ""
      operationId: postProductsOptions.json
      x-api-path-slug: productsidoptions-json-post
      parameters:
      - in: body
        name: body
        description: Product Option parameters
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Products
      - Id
      - Options
      - Json
  /products/{id}/options/count.json:
    get:
      summary: Get Products Options Count
      description: ""
      operationId: getProductsOptionsCount.json
      x-api-path-slug: productsidoptionscount-json-get
      parameters:
      - in: path
        name: id
        description: ID of the Product
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Products
      - Id
      - Options
      - Count
      - Json
  /products/{id}/options/{option_id}.json:
    delete:
      summary: Delete Products Options Option
      description: ""
      operationId: deleteProductsOptionsOption.json
      x-api-path-slug: productsidoptionsoption-id-json-delete
      parameters:
      - in: query
        name: No Name
      - in: path
        name: option_id
        description: Id of the Product Option
      responses:
        200:
          description: OK
      tags:
      - Products
      - Id
      - Options
      - Option
      - Id
      - Json
    get:
      summary: Get Products Options Option
      description: ""
      operationId: getProductsOptionsOption.json
      x-api-path-slug: productsidoptionsoption-id-json-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: option_id
        description: Id of the Product Option
      responses:
        200:
          description: OK
      tags:
      - Products
      - Id
      - Options
      - Option
      - Id
      - Json
    put:
      summary: Put Products Options Option
      description: ""
      operationId: putProductsOptionsOption.json
      x-api-path-slug: productsidoptionsoption-id-json-put
      parameters:
      - in: body
        name: body
        description: Product option parameters to change
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      - in: path
        name: option_id
        description: Id of the Product Option
      responses:
        200:
          description: OK
      tags:
      - Products
      - Id
      - Options
      - Option
      - Id
      - Json
  /products/{id}/options/{option_id}/values.json:
    get:
      summary: Get Products Options Option Values
      description: ""
      operationId: getProductsOptionsOptionValues.json
      x-api-path-slug: productsidoptionsoption-idvalues-json-get
      parameters:
      - in: path
        name: id
        description: ID of the Product
      - in: query
        name: No Name
      - in: path
        name: option_id
        description: ID of the Product Option
      responses:
        200:
          description: OK
      tags:
      - Products
      - Id
      - Options
      - Option
      - Id
      - Values
      - Json
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---