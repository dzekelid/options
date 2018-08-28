---
swagger: "2.0"
x-collection-name: 3dcart
x-complete: 0
info:
  title: 3dcart Get the advanced options from a specific Product
  version: 1.0.0
  description: Get the advanced options from a specific product.
host: apirest.3dcart.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /3dCartWebAPI/v1/Categories/{categoryid}/Options:
    get:
      summary: Get the options from a specific Category
      description: Get the options from a specific category.
      operationId: Category_GetAllCategoryOptions
      x-api-path-slug: 3dcartwebapiv1categoriescategoryidoptions-get
      parameters:
      - in: path
        name: categoryid
        description: Catalog ID
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Options
      - From
      - Specific
      - Category
    put:
      summary: Updates a collection of options from a specific Category
      description: Updates a collection of options from a specific category.
      operationId: Category_Update
      x-api-path-slug: 3dcartwebapiv1categoriescategoryidoptions-put
      parameters:
      - in: path
        name: categoryid
        description: CategoryID
      - in: body
        name: options
        description: A Json or XML object containing the new options
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Collection
      - Of
      - Options
      - From
      - Specific
      - Category
    post:
      summary: Adds a new OptionSet to the system
      description: Adds a new optionset to the system.
      operationId: Category_Post
      x-api-path-slug: 3dcartwebapiv1categoriescategoryidoptions-post
      parameters:
      - in: path
        name: categoryid
        description: Category ID
      - in: body
        name: optionset
        description: A Json or XML object containing the new optionset
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - OptionSet
      - To
      - System
  /3dCartWebAPI/v1/Categories/{categoryid}/Options/{optionsetid}:
    put:
      summary: Updates specific options from a specific Category
      description: Updates specific options from a specific category.
      operationId: Category_Update
      x-api-path-slug: 3dcartwebapiv1categoriescategoryidoptionsoptionsetid-put
      parameters:
      - in: path
        name: categoryid
        description: CategoryID
      - in: body
        name: option
        description: A Json or XML object containing the new options
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: optionsetid
        description: OptionSetID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Specific
      - Options
      - From
      - Specific
      - Category
  /3dCartWebAPI/v1/Products/{catalogid}/AdvancedOptions:
    get:
      summary: Get the advanced options from a specific Product
      description: Get the advanced options from a specific product.
      operationId: Products_GetAllProductAdvancedOptions
      x-api-path-slug: 3dcartwebapiv1productscatalogidadvancedoptions-get
      parameters:
      - in: path
        name: catalogid
        description: Catalog ID
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Advanced
      - Options
      - From
      - Specific
      - Product
    put:
      summary: Updates a collection of advanced options from a specific Product
      description: Updates a collection of advanced options from a specific product.
      operationId: Products_Update
      x-api-path-slug: 3dcartwebapiv1productscatalogidadvancedoptions-put
      parameters:
      - in: body
        name: advancedoptions
        description: A Json or XML object containing the new advanced options
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: catalogid
        description: CatalogID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Collection
      - Of
      - Advanced
      - Options
      - From
      - Specific
      - Product
  /3dCartWebAPI/v1/Products/{catalogid}/AdvancedOptions/{advancedoptioncode}:
    put:
      summary: Updates specific advanced options from a specific Product
      description: Updates specific advanced options from a specific product.
      operationId: Products_Update
      x-api-path-slug: 3dcartwebapiv1productscatalogidadvancedoptionsadvancedoptioncode-put
      parameters:
      - in: body
        name: advancedoption
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: advancedoptioncode
        description: AdvancedOptionCode
      - in: path
        name: catalogid
        description: CatalogID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Specific
      - Advanced
      - Options
      - From
      - Specific
      - Product
  /3dCartWebAPI/v1/Products/{catalogid}/Options:
    get:
      summary: Get the options from a specific Product
      description: Get the options from a specific product.
      operationId: Products_GetAllProductOptions
      x-api-path-slug: 3dcartwebapiv1productscatalogidoptions-get
      parameters:
      - in: path
        name: catalogid
        description: Catalog ID
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Options
      - From
      - Specific
      - Product
    put:
      summary: Updates a collection of options from a specific Product
      description: Updates a collection of options from a specific product.
      operationId: Products_Update
      x-api-path-slug: 3dcartwebapiv1productscatalogidoptions-put
      parameters:
      - in: path
        name: catalogid
        description: CatalogID
      - in: body
        name: options
        description: A Json or XML object containing the new options
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Collection
      - Of
      - Options
      - From
      - Specific
      - Product
    post:
      summary: Adds a new OptionSet to the system
      description: Adds a new optionset to the system.
      operationId: Products_Post
      x-api-path-slug: 3dcartwebapiv1productscatalogidoptions-post
      parameters:
      - in: path
        name: catalogid
        description: Catalog ID
      - in: body
        name: optionset
        description: A Json or XML object containing the new optionset
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - OptionSet
      - To
      - System
  /3dCartWebAPI/v1/Products/{catalogid}/Options/{optionsetid}:
    put:
      summary: Updates specific options from a specific Product
      description: Updates specific options from a specific product.
      operationId: Products_Update
      x-api-path-slug: 3dcartwebapiv1productscatalogidoptionsoptionsetid-put
      parameters:
      - in: path
        name: catalogid
        description: CatalogID
      - in: body
        name: option
        description: A Json or XML object containing the new options
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: optionsetid
        description: OptionSetID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Specific
      - Options
      - From
      - Specific
      - Product
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