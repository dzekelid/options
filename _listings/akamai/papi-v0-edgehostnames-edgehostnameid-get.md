---
swagger: "2.0"
info:
  title: Akamai API Get an Edge Hostname
  description: Get an Edge Hostname
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
  /papi/v0/edgehostnames/{edgeHostnameId}:
    get:
      summary: Get an Edge Hostname
      description: Get an Edge Hostname
      operationId: papiv0edgehostnamesedgehostnameidcontractidgroupidoptions
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
      - papi
      - v0
      - edgehostnames
      - edgehostname
      - contract
      - group
      - options
definitions: []
x-collection-name: Akamai
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