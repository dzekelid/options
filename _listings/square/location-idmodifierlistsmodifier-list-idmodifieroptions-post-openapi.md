---
swagger: "2.0"
x-collection-name: Square
x-complete: 0
info:
  title: Square Connect API Post Location Modifier Lists Modifier List Modifier Options
  description: Creates an item modifier option and adds it to a modifier list.
  termsOfService: https://connect.squareup.com/tos
  contact:
    name: Square Developer Platform
    url: https://squareup.com/developers
    email: developers@squareup.com
  version: 1.0.0
host: connect.squareup.com
basePath: v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{location_id}/modifier-lists/{modifier_list_id}/modifier-options:
    post:
      summary: Post Location Modifier Lists Modifier List Modifier Options
      description: Creates an item modifier option and adds it to a modifier list.
      operationId: postLocationModifierListsModifierListModifierOptions
      x-api-path-slug: location-idmodifierlistsmodifier-list-idmodifieroptions-post
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: location_id
        description: The ID of the items associated location
      - in: path
        name: modifier_list_id
        description: The ID of the modifier list to edit
      responses:
        200:
          description: OK
      tags:
      - Location
      - Modifier-lists
      - Modifier
      - List
      - Modifier-options
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