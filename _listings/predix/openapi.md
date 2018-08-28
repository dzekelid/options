swagger: "2.0"
x-collection-name: Predix
x-complete: 1
info:
  title: VIEWS
  version: 1.0.0
host: thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /instances/{instanceId}/sparkproxy/**:
    options:
      summary: Options Instances Instanceid Sparkproxy **
      description: Options instances instanceid sparkproxy **.
      operationId: getInstanceSparkProxyUsingOPTIONS
      x-api-path-slug: instancesinstanceidsparkproxy-options
      parameters:
      - in: path
        name: instanceId
        description: instanceId
      responses:
        200:
          description: Successful response
      tags:
      - Options
      - Instances
      - Instanceid
      - Sparkproxy
      - '**'