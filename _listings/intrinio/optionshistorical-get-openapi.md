---
swagger: "2.0"
x-collection-name: Intrinio
x-complete: 0
info:
  title: Intrinio API Historical Prices
  description: Returns the historical prices for the given option contract.
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