---
swagger: "2.0"
x-collection-name: Clover
x-complete: 0
info:
  title: Clover Create or delete item/option association
  version: 1.0.0
  description: See the description for 'get all item groups'.
host: /merchants
basePath: https://api.clover.com
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/merchants/{mId}/options:
    get:
      summary: Get all options
      description: See the description for 'get all item groups'.
      operationId: GetOptions
      x-api-path-slug: v3merchantsmidoptions-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: []'
      - in: query
        name: filter
        description: 'Filter fields: [modifiedTime, item'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Options
  /v3/merchants/{mId}/attributes/{attributeId}/options:
    get:
      summary: Get all options with a given attribute
      description: Get all options with a given attribute.
      operationId: GetOptionsByAttribute
      x-api-path-slug: v3merchantsmidattributesattributeidoptions-get
      parameters:
      - in: path
        name: attributeId
        description: Attribute Id
      - in: query
        name: expand
        description: 'Expandable fields: []'
      - in: query
        name: filter
        description: 'Filter fields: [modifiedTime, item'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Attributes
      - AttributeId
      - Options
    post:
      summary: Create an option
      description: Create an option.
      operationId: CreateOption
      x-api-path-slug: v3merchantsmidattributesattributeidoptions-post
      parameters:
      - in: path
        name: attributeId
        description: Attribute Id
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: []'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Attributes
      - AttributeId
      - Options
  /v3/merchants/{mId}/attributes/{attributeId}/options/{optionId}:
    get:
      summary: Get all options with a given attribute
      description: Get all options with a given attribute.
      operationId: GetOptionsByAttribute
      x-api-path-slug: v3merchantsmidattributesattributeidoptionsoptionid-get
      parameters:
      - in: path
        name: attributeId
        description: Attribute Id
      - in: query
        name: expand
        description: 'Expandable fields: []'
      - in: query
        name: filter
        description: 'Filter fields: [modifiedTime, item'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: optionId
        description: Option Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Attributes
      - AttributeId
      - Options
      - OptionId
    post:
      summary: Update an option
      description: Update an option.
      operationId: UpdateOption
      x-api-path-slug: v3merchantsmidattributesattributeidoptionsoptionid-post
      parameters:
      - in: path
        name: attributeId
        description: Attribute Id
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: []'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: optionId
        description: Option Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Attributes
      - AttributeId
      - Options
      - OptionId
    delete:
      summary: Delete an option
      description: Delete an option.
      operationId: DeleteOption
      x-api-path-slug: v3merchantsmidattributesattributeidoptionsoptionid-delete
      parameters:
      - in: path
        name: attributeId
        description: Attribute Id
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: optionId
        description: Option Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Attributes
      - AttributeId
      - Options
      - OptionId
  /v3/merchants/{mId}/option_items:
    post:
      summary: Create or delete item/option association
      description: See the description for 'get all item groups'.
      operationId: CreateOrDeleteOptionItems
      x-api-path-slug: v3merchantsmidoption-items-post
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Option
      - Items
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