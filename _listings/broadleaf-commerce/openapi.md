swagger: "2.0"
x-collection-name: Broadleaf Commerce
x-complete: 1
info:
  title: Broadleaf Commerce API
  description: the-default-broadleaf-commerce-apis
  version: 1.0.0
host: demo.broadleafcommerce.org
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /docsreload:
    options:
      summary: Options Docsreload
      description: Options docsreload.
      operationId: optionsDocsreload
      x-api-path-slug: docsreload-options
      responses:
        200:
          description: OK
      tags:
      - Options
      - Docsreload
  /error:
    options:
      summary: Options Error
      description: Options error.
      operationId: optionsError
      x-api-path-slug: error-options
      responses:
        200:
          description: OK
      tags:
      - Options
      - Error
  /preview/**:
    options:
      summary: Options Preview **
      description: Options preview **.
      operationId: optionsPreview**
      x-api-path-slug: preview-options
      responses:
        200:
          description: OK
      tags:
      - Options
      - Preview
      - '**'
  /ratings/{itemId}:
    options:
      summary: Options Ratings
      description: Options ratings.
      operationId: optionsRatingsItem
      x-api-path-slug: ratingsitemid-options
      parameters:
      - in: path
        name: itemId
        description: itemId
      - in: query
        name: ratingType
        description: ratingType
      responses:
        200:
          description: OK
      tags:
      - Options
      - Ratings
  /shipping/options:
    get:
      summary: Get Shipping Options
      description: Get shipping options.
      operationId: getShippingOptions
      x-api-path-slug: shippingoptions-get
      parameters:
      - in: query
        name: fulfillmentType
        description: fulfillmentType
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Options
  /shipping/{cartId}/estimate:
    options:
      summary: Options Shipping Estimate
      description: Options shipping estimate.
      operationId: optionsShippingCartEstimate
      x-api-path-slug: shippingcartidestimate-options
      parameters:
      - in: path
        name: cartId
        description: cartId
      responses:
        200:
          description: OK
      tags:
      - Options
      - Shipping
      - Estimate
  /shipping/{cartId}/group/{fulfillmentGroupId}/option/{fulfillmentOptionId}:
    put:
      summary: Put Shipping Group Fulfillmentgroupid Option Fulfillmentoptionid
      description: Put shipping group fulfillmentgroupid option fulfillmentoptionid.
      operationId: putShippingCartGroupFulfillmentgroupOptionFulfillmentoption
      x-api-path-slug: shippingcartidgroupfulfillmentgroupidoptionfulfillmentoptionid-put
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: path
        name: fulfillmentGroupId
        description: fulfillmentGroupId
      - in: path
        name: fulfillmentOptionId
        description: fulfillmentOptionId
      - in: query
        name: priceOrder
        description: priceOrder
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Group
      - Fulfillmentgroupid
      - Option
      - Fulfillmentoptionid