---
swagger: "2.0"
x-collection-name: AWS Internet of Things
x-complete: 1
info:
  title: AWS Internet of Things API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetLoggingOptions:
    get:
      summary: Get Logging Options
      description: Gets the logging options.
      operationId: getLoggingOptions
      x-api-path-slug: actiongetloggingoptions-get
      parameters:
      - in: query
        name: logLevel
        description: The logging level
        type: string
      - in: query
        name: roleArn
        description: The ARN of the IAM role that grants access
        type: string
      responses:
        200:
          description: OK
      tags:
      - Logging Options
---