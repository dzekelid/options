---
swagger: "2.0"
x-collection-name: Broadleaf Commerce
x-complete: 0
info:
  title: Broadleaf Commerce API Options Error
  description: Options error.
  version: 1.0.0
host: demo.broadleafcommerce.org
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /docsreload:
    options:
      summary: Options Docsreload
      description: Options docsreload.
      operationId: optionsDocsreload
      x-api-path-slug: docsreload-options
      responses:
        200:
          description: OK
      tags:
      - Options
      - Docsreload
  /error:
    options:
      summary: Options Error
      description: Options error.
      operationId: optionsError
      x-api-path-slug: error-options
      responses:
        200:
          description: OK
      tags:
      - Options
      - Error
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