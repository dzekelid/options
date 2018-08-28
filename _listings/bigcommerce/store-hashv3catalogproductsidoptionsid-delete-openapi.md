---
swagger: "2.0"
x-collection-name: BigCommerce
x-complete: 0
info:
  title: BigCommerce Delete a product option
  description: ""
  version: 1.0.0
host: api.bigcommerce.com
basePath: /stores
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{store_hash}/v3/catalog/products/{id}/options:
    get:
      summary: Retrieve an array of product options
      description: ""
      operationId: V3CatalogProductsOptionsByStoreHashAndIdGet
      x-api-path-slug: store-hashv3catalogproductsidoptions-get
      parameters:
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Retrieve
      - Array
      - Of
      - Product
      - Options
    post:
      summary: Create a product option
      description: ""
      operationId: V3CatalogProductsOptionsByStoreHashAndIdPost
      x-api-path-slug: store-hashv3catalogproductsidoptions-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Product
      - Option
  /{store_id}/v3/catalog/products/{id}/options/{id}:
    put:
      summary: Update a product option
      description: ""
      operationId: V3CatalogProductsOptionsIdByStoreIdAndIdPut
      x-api-path-slug: store-idv3catalogproductsidoptionsid-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: id
      - in: path
        name: store_id
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Product
      - Option
  /{store_hash}/v3/catalog/products/{id}/options/{id}:
    get:
      summary: Retrieve a product option
      description: Gets `Option` object by product id and option id.
      operationId: V3CatalogProductsOptionsIdByStoreHashAndIdGet
      x-api-path-slug: store-hashv3catalogproductsidoptionsid-get
      parameters:
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Retrieve
      - Product
      - Option
    delete:
      summary: Delete a product option
      description: ""
      operationId: V3CatalogProductsOptionsIdByStoreHashAndIdDelete
      x-api-path-slug: store-hashv3catalogproductsidoptionsid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Product
      - Option
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