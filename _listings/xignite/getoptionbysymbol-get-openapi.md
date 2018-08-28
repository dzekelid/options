---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Global Option Master Get Option By Symbol
  description: Get details on an option.
  version: 1.0.0
host: globaloptionmaster.xignite.com
basePath: xGlobalOptionMaster.json/XigniteGlobalOptionMaster
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetFutureOptionsByStrikePrice:
    get:
      summary: Get Future Options By Strike Price
      description: Returns an option chain for a future contract matching a list of
        prices.
      operationId: postGetfutureoptionsbystrikeprice
      x-api-path-slug: getfutureoptionsbystrikeprice-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Future
      - Options
      - By
      - Strike
      - Price
  /GetFutureOption:
    get:
      summary: Get Future Option
      description: Returns a specific future option.
      operationId: postGetfutureoption
      x-api-path-slug: getfutureoption-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Future
      - Option
  /GetFutureOptionChain:
    get:
      summary: Get Future Option Chain
      description: Returns an option chain for a future contract.
      operationId: postGetfutureoptionchain
      x-api-path-slug: getfutureoptionchain-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Future
      - Option
      - Chain
  /GetFutureOptionQuote:
    get:
      summary: Get Future Option Quote
      description: Returns a delayed future option quote for a future option.
      operationId: GetFutureOptionQuote
      x-api-path-slug: getfutureoptionquote-get
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
      - Option
      - Quote
  /GetAllOptionQuotes:
    get:
      summary: Get All Option Quotes
      description: Returns all delayed future option quotes for a future contract.
      operationId: GetAllOptionQuotes
      x-api-path-slug: getalloptionquotes-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Option
      - Quotes
  /GetFutureOptionQuotes:
    get:
      summary: Get Future Option Quotes
      description: Returns delayed future option quotes for multiple future options.
      operationId: GetFutureOptionQuotes
      x-api-path-slug: getfutureoptionquotes-get
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
      - Option
      - Quotes
  /GetLatestFutureOptionQuote:
    get:
      summary: Get Latest Future Option Quote
      description: Returns latest delayed quote for multiple future option.
      operationId: GetLatestFutureOptionQuote
      x-api-path-slug: getlatestfutureoptionquote-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Latest
      - Future
      - Option
      - Quote
  /GetLatestFutureOptionQuotes:
    get:
      summary: Get Latest Future Option Quotes
      description: Returns latest delayed quotes for multiple future options.
      operationId: GetLatestFutureOptionQuotes
      x-api-path-slug: getlatestfutureoptionquotes-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Latest
      - Future
      - Option
      - Quotes
  /ListOptionChain:
    get:
      summary: List Option Chain
      description: Returns a list of options on a future contract
      operationId: ListOptionChain
      x-api-path-slug: listoptionchain-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - List
      - Option
      - Chain
  /GetUnderlyingForOption:
    get:
      summary: Get Underlying For Option
      description: Get details on an underlying instrument for the option symbol provided.
      operationId: GetUnderlyingForOption
      x-api-path-slug: getunderlyingforoption-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Underlying
      - Option
  /GetOptionBySymbol:
    get:
      summary: Get Option By Symbol
      description: Get details on an option.
      operationId: GetOptionBySymbol
      x-api-path-slug: getoptionbysymbol-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Option
      - Symbol
  /GetOptionChain:
    get:
      summary: Get Option Chain
      description: Get the option chain for the underlying instrument.
      operationId: GetOptionChain
      x-api-path-slug: getoptionchain-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Option
      - Chain
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