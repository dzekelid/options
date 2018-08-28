swagger: "2.0"
x-collection-name: AWS S3
x-complete: 1
info:
  title: No Title
  version: 1.0.0
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