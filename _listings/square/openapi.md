---
swagger: "2.0"
x-collection-name: Square
x-complete: 1
info:
  title: Square Connect
  description: client-library-for-accessing-the-square-connect-apis
  termsOfService: https://connect.squareup.com/tos
  contact:
    name: Square Developer Platform
    url: https://squareup.com/developers
    email: developers@squareup.com
  version: "2.0"
host: connect.squareup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/{location_id}/items/{item_id}/modifier-lists/{modifier_list_id}:
    delete:
      summary: Removes a modifier list association from an item, meaning modifier
        options from the list can no longer be applied to the item.
      description: Removes a modifier list association from an item, meaning modifier
        options from the list can no longer be applied to the item.
      operationId: RemoveModifierList
      x-api-path-slug: v1location-iditemsitem-idmodifierlistsmodifier-list-id-delete
      parameters:
      - in: path
        name: item_id
        description: The ID of the item to remove the modifier list from
      - in: path
        name: location_id
        description: The ID of the items associated location
      - in: path
        name: modifier_list_id
        description: The ID of the modifier list to remove
      responses:
        200:
          description: OK
      tags:
      - Removes
      - Modifier
      - List
      - Association
      - From
      - Item
      - ""
      - Meaning
      - Modifier
      - Options
      - From
      - List
      - Can
      - "No"
      - Longer
      - Be
      - Applied
      - To
      - Item
    put:
      summary: Associates a modifier list with an item, meaning modifier options from
        the list can be applied to the item.
      description: Associates a modifier list with an item, meaning modifier options
        from the list can be applied to the item.
      operationId: ApplyModifierList
      x-api-path-slug: v1location-iditemsitem-idmodifierlistsmodifier-list-id-put
      parameters:
      - in: path
        name: item_id
        description: The ID of the item to add the modifier list to
      - in: path
        name: location_id
        description: The ID of the items associated location
      - in: path
        name: modifier_list_id
        description: The ID of the modifier list to apply
      responses:
        200:
          description: OK
      tags:
      - Associates
      - Modifier
      - List
      - Item
      - ""
      - Meaning
      - Modifier
      - Options
      - From
      - List
      - Can
      - Be
      - Applied
      - To
      - Item
  /v1/{location_id}/modifier-lists/{modifier_list_id}:
    delete:
      summary: Deletes an existing item modifier list and all modifier options associated
        with it.
      description: Deletes an existing item modifier list and all modifier options
        associated with it.
      operationId: DeleteModifierList
      x-api-path-slug: v1location-idmodifierlistsmodifier-list-id-delete
      parameters:
      - in: path
        name: location_id
        description: The ID of the items associated location
      - in: path
        name: modifier_list_id
        description: The ID of the modifier list to delete
      responses:
        200:
          description: OK
      tags:
      - S
      - Existing
      - Item
      - Modifier
      - List
      - ""
      - Modifier
      - Options
      - Associated
      - It
---