---
swagger: "2.0"
x-collection-name: AWS S3
x-complete: 0
info:
  title: AWS S3 OPTIONS object
  version: 1.0.0
  description: A browser can send this preflight request to Amazon S3 to determine
    if it can send an actualrequest with the specific origin, HTTP method, and headers
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ObjectName:
    options:
      summary: OPTIONS object
      description: A browser can send this preflight request to Amazon S3 to determine
        if it can send an actualrequest with the specific origin, HTTP method, and
        headers
      operationId: options-object
      x-api-path-slug: objectname-options
      responses:
        200:
          description: OK
      tags:
      - OPTIONS
      - Object
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