swagger: "2.0"
x-collection-name: Akeneo
x-complete: 1
info:
  title: Official Akeneo PIM API
  description: the-akeneo-api-brought-to-youfind-out-how-this-postman-collection-works-by-visiting-httpapi-akeneo-com
  version: 1.0.0
host: example.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/v1/attributes/main_color/options:
    get:
      summary: attribute options
      description: Attribute options.
      operationId: RestV1AttributesMainColorOptionsGet
      x-api-path-slug: restv1attributesmain-coloroptions-get
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Options
    patch:
      summary: attribute options (2.1 only)
      description: Assuming that the given code is the code of an existing attribute
      operationId: RestV1AttributesMainColorOptionsPatch
      x-api-path-slug: restv1attributesmain-coloroptions-patch
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Options
      - (2
      - "1"
      - Only)
    post:
      summary: attribute option
      description: Assuming that there is no "yellow" option already existing for
        the given attribute
      operationId: RestV1AttributesMainColorOptionsPost
      x-api-path-slug: restv1attributesmain-coloroptions-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Option
  /rest/v1/attributes/main_color/options/white:
    get:
      summary: attribute option
      description: Assuming that the given codes are respectively the code of an existing
        attribute and an existing option of this attribute
      operationId: RestV1AttributesMainColorOptionsWhiteGet
      x-api-path-slug: restv1attributesmain-coloroptionswhite-get
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Option
    patch:
      summary: attribute option
      description: Assuming that the given code is the code of an existing attribute
      operationId: RestV1AttributesMainColorOptionsWhitePatch
      x-api-path-slug: restv1attributesmain-coloroptionswhite-patch
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Option