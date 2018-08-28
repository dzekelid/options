---
swagger: "2.0"
x-collection-name: Xero
x-complete: 0
info:
  title: Clarity Accounting X-related-model Tracking Categories Trackingcategory Options
  description: X-related-model trackingcategories trackingcategory options.
  contact:
    name: Xero Developer Team
    url: https://developer.xero.com
  version: "2.0"
host: api.xero.com
basePath: /api.xro/2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /TrackingCategories/{TrackingCategoryID}/Options:
    put:
      summary: Put Tracking Categories Trackingcategory Options
      description: Put trackingcategories trackingcategory options.
      operationId: putTrackingcategoriesTrackingcategoryOptions
      x-api-path-slug: trackingcategoriestrackingcategoryidoptions-put
      parameters:
      - in: query
        name: No Name
      - in: path
        name: TrackingCategoryID
      - in: body
        name: TrackingOptions
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - TrackingCategories
      - TrackingCategoryID
      - Options
    x-related-model:
      summary: X-related-model Tracking Categories Trackingcategory Options
      description: X-related-model trackingcategories trackingcategory options.
      operationId: x-related-modelTrackingcategoriesTrackingcategoryOptions
      x-api-path-slug: trackingcategoriestrackingcategoryidoptions-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - TrackingCategories
      - TrackingCategoryID
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