---
swagger: "2.0"
x-collection-name: Akeneo
x-complete: 0
info:
  title: Akeneo PIM API attribute options
  description: Attribute options.
  version: 1.0.0
host: example.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/v1/attributes/main_color/options:
    get:
      summary: attribute options
      description: Attribute options.
      operationId: RestV1AttributesMainColorOptionsGet
      x-api-path-slug: restv1attributesmain-coloroptions-get
      responses:
        200:
          description: OK
      tags:
      - Attribute
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