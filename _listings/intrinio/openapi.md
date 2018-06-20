---
swagger: "2.0"
x-collection-name: Intrinio
x-complete: 1
info:
  title: Intrinio
  description: through-our-intrinio-data-marketplace-we-offer-a-wide-selection-of-financial-data-feeds-sourced-by-our-own-proprietary-processes-as-well-as-from-many-data-vendors--the-primary-application-of-the-intrinio-api-is-for-use-in-thirdparty-applications-and-integrations-or-for-endusers-utilizing-the-excel-addin-and-google-sheets-addon--the-intrinio-api-uses-https-verbs-and-a-restful-endpoint-structure-which-makes-it-easy-to-request-data-from-intrinio--basic-authentication-is-administered-over-https--responses-are-delivered-in-json-format-
  version: 1.0.0
host: api.intrinio.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /options/expirations:
    get:
      summary: Option Expirations
      description: Returns all option contract expiration dates for a given ticker.
      operationId: option-expirations
      x-api-path-slug: optionsexpirations-get
      parameters:
      - in: query
        name: ticker
        description: the option ticker symbol, corresponding to the underlying security
        type: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Options
  /options/historical:
    get:
      summary: Historical Prices
      description: Returns the historical prices for the given option contract.
      operationId: historical-prices
      x-api-path-slug: optionshistorical-get
      parameters:
      - in: query
        name: expiration
        description: the contract expiration date, in the format YYYY
        type: string
      - in: query
        name: identifier
        description: 'the contract identifier (example: AAPL190118C00195000)'
        type: string
      - in: query
        name: page_number
        description: an integer greater than or equal to 1 for specifying the page
          number for the return values
        type: string
      - in: query
        name: page_size
        description: an integer greater than 1 for specifying the number of results
          on each page
        type: string
      - in: query
        name: strike
        description: the contract strike price
        type: string
      - in: query
        name: ticker
        description: the option ticker symbol, corresponding to the underlying security
        type: string
      - in: query
        name: type
        description: the contract type, either put or call
        type: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Options
      - Historical
---