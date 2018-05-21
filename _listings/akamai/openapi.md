---
swagger: "2.0"
x-collection-name: Akamai
x-complete: 1
info:
  title: Akamai API
  description: the-akamai-api-for-managing-your-akamai-service
  version: 1.0.0
host: developer.akamai.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /papi/v0/edgehostnames/:
    get:
      summary: List Edge Hostnames
      description: List Edge Hostnames
      operationId: papiv0edgehostnamescontractidgroupidoptions
      x-api-path-slug: papiv0edgehostnames-get
      parameters:
      - in: query
        name: contractId
        description: Unique identifier for the contract
        type: string
      - in: query
        name: groupId
        description: Unique identifier for the group
        type: string
      - in: query
        name: options
        description: Comma-separated list of options to enable; mapDetails enables
          extra mapping-related information
        type: string
      responses:
        200:
          description: OK
      tags:
      - Papi
      - V0
      - Edgehostnames
      - Contract
      - group
      - options
    post:
      summary: Create a New Edge Hostname
      description: Create a New Edge Hostname
      operationId: papiv0edgehostnamescontractidgroupidoptions
      x-api-path-slug: papiv0edgehostnames-post
      parameters:
      - in: query
        name: contractId
        description: Unique identifier for the contract
        type: string
      - in: query
        name: groupId
        description: Unique identifier for the group
        type: string
      - in: query
        name: options
        description: Comma-separated list of options to enable; mapDetails enables
          extra mapping-related information
        type: string
      responses:
        200:
          description: OK
      tags:
      - Papi
      - V0
      - Edgehostnames
      - Contract
      - group
      - options
  /papi/v0/edgehostnames/{edgeHostnameId}:
    get:
      summary: Get an Edge Hostname
      description: Get an Edge Hostname
      operationId: papiv0edgehostnamesedgehostnameidcontractidgroupidoptions
      x-api-path-slug: papiv0edgehostnamesedgehostnameid-get
      parameters:
      - in: query
        name: contractId
        description: Unique identifier for the contract
        type: string
      - in: query
        name: edgeHostnameId
        description: Unique identifier for the edge hostname
        type: string
      - in: query
        name: groupId
        description: Unique identifier for the group
        type: string
      - in: query
        name: options
        description: Comma-separated list of options to enable; mapDetails enables
          extra mapping-related information
        type: string
      responses:
        200:
          description: OK
      tags:
      - Papi
      - V0
      - Edgehostnames
      - Edgehostname
      - Contract
      - group
      - options
---