---
swagger: "2.0"
x-collection-name: Square
x-complete: 1
info:
  title: Square Connect API
  description: client-library-for-accessing-the-square-connect-apis
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
  /{location_id}/modifier-lists/{modifier_list_id}/modifier-options/{modifier_option_id}:
    put:
      summary: Put Location Modifier Lists Modifier List Modifier Options Modifier
        Option
      description: Put location modifier lists modifier list modifier options modifier
        option.
      operationId: putLocationModifierListsModifierListModifierOptionsModifierOption
      x-api-path-slug: location-idmodifierlistsmodifier-list-idmodifieroptionsmodifier-option-id-put
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
      - in: path
        name: modifier_option_id
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
      - Modifier
      - Option
    delete:
      summary: Delete Location Modifier Lists Modifier List Modifier Options Modifier
        Option
      description: Delete location modifier lists modifier list modifier options modifier
        option.
      operationId: deleteLocationModifierListsModifierListModifierOptionsModifierOption
      x-api-path-slug: location-idmodifierlistsmodifier-list-idmodifieroptionsmodifier-option-id-delete
      parameters:
      - in: path
        name: location_id
        description: The ID of the items associated location
      - in: path
        name: modifier_list_id
        description: The ID of the modifier list to delete
      - in: path
        name: modifier_option_id
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
      - Modifier
      - Option
---