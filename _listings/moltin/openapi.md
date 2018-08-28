swagger: "2.0"
x-collection-name: moltin
x-complete: 1
info:
  title: Moltin
  description: -welcomethis-is-a-place-to-put-general-notes-and-extra-information-for-internal-use-to-get-started-designingdocumenting-this-api-select-a-version-on-the-left-
  version: 1.0.0
host: api.moltin.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/variations/{variationID}/options/{optionID}:
    put:
      summary: Update a Product Variation Option
      description: Update a product variation option.
      operationId: V2VariationsOptionsByVariationIDAndOptionIDPut
      x-api-path-slug: v2variationsvariationidoptionsoptionid-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: optionID
      - in: path
        name: variationID
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Variation
      - Option
    delete:
      summary: Delete a Product Variation Option
      description: Delete a product variation option.
      operationId: V2VariationsOptionsByVariationIDAndOptionIDDelete
      x-api-path-slug: v2variationsvariationidoptionsoptionid-delete
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: optionID
      - in: path
        name: variationID
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Variation
      - Option
  /v2/variations/{variationID}/options:
    post:
      summary: Create a Product Variation Option
      description: Create a product variation option.
      operationId: V2VariationsOptionsByVariationIDPost
      x-api-path-slug: v2variationsvariationidoptions-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: variationID
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Variation
      - Option