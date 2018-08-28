swagger: "2.0"
x-collection-name: Xero
x-complete: 1
info:
  title: Xero oAuth 1a
  description: a-collection-to-authenticate-to-the-xero-api-using-oauth1-0a
  version: 1.0.0
host: api.xero.com
basePath: /
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
  /TrackingCategories/{TrackingCategoryID}/Options/{TrackingOptionID}:
    delete:
      summary: Delete Tracking Categories Trackingcategory Options Trackingoption
      description: Delete trackingcategories trackingcategory options trackingoption.
      operationId: deleteTrackingcategoriesTrackingcategoryOptionsTrackingoption
      x-api-path-slug: trackingcategoriestrackingcategoryidoptionstrackingoptionid-delete
      parameters:
      - in: path
        name: TrackingCategoryID
      - in: path
        name: TrackingOptionID
      responses:
        200:
          description: OK
      tags:
      - TrackingCategories
      - TrackingCategoryID
      - Options
      - TrackingOptionID
    x-related-model:
      summary: X-related-model Tracking Categories Trackingcategory Options Trackingoption
      description: X-related-model trackingcategories trackingcategory options trackingoption.
      operationId: x-related-modelTrackingcategoriesTrackingcategoryOptionsTrackingoption
      x-api-path-slug: trackingcategoriestrackingcategoryidoptionstrackingoptionid-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - TrackingCategories
      - TrackingCategoryID
      - Options
      - TrackingOptionID