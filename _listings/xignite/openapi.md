---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 1
info:
  title: Xignite Futures
  description: provide-delayed-and-historical-commodity-quote-information-from-supported-exchanges-nymex
  version: 1.0.0
host: www.xignite.com
basePath: xFutures.json/XigniteFutures
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetFutureOptionsByStrikePrice:
    post:
      summary: Get Future Options By Strike Price
      description: Returns an option chain for a future contract matching a list of
        prices.
      operationId: postGetfutureoptionsbystrikeprice
      x-api-path-slug: getfutureoptionsbystrikeprice-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Future
      - Options
      - By
      - Strike
      - Price
---