---
swagger: "2.0"
x-collection-name: Intrinio
x-complete: 0
info:
  title: Intrinio API Option Expirations
  description: Returns all option contract expiration dates for a given ticker.
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
        description: ' the option ticker symbol, corresponding to the underlying security'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Options
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