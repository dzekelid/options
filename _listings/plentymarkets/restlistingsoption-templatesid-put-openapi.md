---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Update option template
  description: Updates an option template by ID.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/accounts/addresses/{addressId}/options:
    get:
      summary: List address options
      description: Lists address options. The ID of the address must be specified.
      operationId: getRestAccountsAddressesAddressOptions
      x-api-path-slug: restaccountsaddressesaddressidoptions-get
      parameters:
      - in: path
        name: addressId
      responses:
        200:
          description: OK
      tags:
      - List
      - Address
      - Options
    delete:
      summary: Delete an address option by the address ID
      description: Deletes an address option. The ID of the address must be specified.
      operationId: deleteRestAccountsAddressesAddressOptions
      x-api-path-slug: restaccountsaddressesaddressidoptions-delete
      parameters:
      - in: path
        name: addressId
      responses:
        200:
          description: OK
      tags:
      - Address
      - Option
      - By
      - Address
      - ID
    post:
      summary: Create an address option
      description: Creates an address option. The ID of the address must be specified.
      operationId: postRestAccountsAddressesAddressOptions
      x-api-path-slug: restaccountsaddressesaddressidoptions-post
      parameters:
      - in: path
        name: addressId
      responses:
        200:
          description: OK
      tags:
      - Address
      - Option
    put:
      summary: Update the address options for an address
      description: Update the address options for an address.
      operationId: putRestAccountsAddressesAddressOptions
      x-api-path-slug: restaccountsaddressesaddressidoptions-put
      parameters:
      - in: path
        name: addressId
      responses:
        200:
          description: OK
      tags:
      - Address
      - Optionsan
      - Address
  /rest/accounts/contacts/{contactId}/options:
    get:
      summary: List contact options by the contact ID
      description: Lists contact options. The ID of the contact must be specified.
      operationId: getRestAccountsContactsContactOptions
      x-api-path-slug: restaccountscontactscontactidoptions-get
      parameters:
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - List
      - Contact
      - Options
      - By
      - Contact
      - ID
    delete:
      summary: Delete a contact option by the contact ID
      description: Deletes a contact option for an existing contact. The ID of the
        contact must be specified.
      operationId: deleteRestAccountsContactsContactOptions
      x-api-path-slug: restaccountscontactscontactidoptions-delete
      parameters:
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Option
      - By
      - Contact
      - ID
    post:
      summary: Create a contact option by the contact ID
      description: Creates a contact option for an existing contact. The ID of the
        contact must be specified.
      operationId: postRestAccountsContactsContactOptions
      x-api-path-slug: restaccountscontactscontactidoptions-post
      parameters:
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Option
      - By
      - Contact
      - ID
    put:
      summary: Update a contact option by the contact ID
      description: Updates a contact option for an existing contact. The ID of the
        contact must be specified.
      operationId: putRestAccountsContactsContactOptions
      x-api-path-slug: restaccountscontactscontactidoptions-put
      parameters:
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Option
      - By
      - Contact
      - ID
  /rest/orders:
    get:
      summary: List orders by filter options
      description: List orders by filter options.
      operationId: getRestOrders
      x-api-path-slug: restorders-get
      parameters:
      - in: query
        name: clientId
        description: Filter that restricts the search result to order from one client
      - in: query
        name: contactId
        description: Filter that restricts the search result to orders of one order
          contact
      - in: query
        name: createdAtFrom
        description: Filter that restricts the search result to orders that were created
          on the specified date
      - in: query
        name: createdAtTo
        description: Filter that restricts the search result to orders that were created
          within a certain period of time
      - in: query
        name: externalOrderId
        description: Filter that restricts the search result to an external order
          id
      - in: query
        name: hasDocument
        description: Filter that restricts the search result to orders which hold
          the given document type
      - in: query
        name: includedItem
        description: Filter that restricts the search result to orders with a certain
          item
      - in: query
        name: includedVariation
        description: Filter that restricts the search result to orders with a certain
          variation
      - in: query
        name: isEbayPlus
        description: Filter that restricts the search result to orders with ebay plus
      - in: query
        name: itemsPerPage
        description: The number of orders to be displayed per page
      - in: query
        name: orderIds
        description: Filter that restricts the search result to orders
      - in: query
        name: orderType
        description: Filter that restricts the search result to orders of specific
          order types
      - in: query
        name: outgoingItemsBookedAtFrom
        description: Filter that restricts the search result to orders where the outgoing
          items were booked on the specified date
      - in: query
        name: outgoingItemsBookedAtTo
        description: Filter that restricts the search result to orders where the outgoing
          items were booked within a specified period of time
      - in: query
        name: ownerUserId
        description: Filter that restricts the search result to orders of one owner
      - in: query
        name: page
        description: The page to get
      - in: query
        name: paidAtFrom
        description: Filter that restricts the search result to orders that received
          a payment on the specified date
      - in: query
        name: paidAtTo
        description: Filter that restricts the search result to orders that received
          a payment within a certain period of time
      - in: query
        name: paymentStatus
        description: Filter that restricts the search result to order with a specific
          payment status
      - in: query
        name: referrerId
        description: Filter that restricts the search result to orders from one order
          referrer
      - in: query
        name: shippingProfileId
        description: Filter that restricts the search result to orders with a specific
          shipping profile
      - in: query
        name: statusFrom
        description: Filter that restricts the search result to orders in a specific
          order status
      - in: query
        name: statusTo
        description: Filter that restricts the search result to orders within a range
          of order statuses
      - in: query
        name: supplierId
        description: Filter that restricts the search result to orders that include
          order items with variations from a supplier
      - in: query
        name: updatedAtFrom
        description: Filter that restricts the search result to orders that were last
          updated on the specified date
      - in: query
        name: updatedAtTo
        description: Filter that restricts the search result to orders that were last
          updated within a specified period of time
      - in: query
        name: warehouseId
        description: Filter that restricts the search result to orders with a specific
          main warehouse
      - in: query
        name: with
        description: Load additional relations for an order
      responses:
        200:
          description: OK
      tags:
      - List
      - Orders
      - By
      - Filter
      - Options
  /rest/properties/groups/options:
    get:
      summary: List group options
      description: Lists group options.
      operationId: getRestPropertiesGroupsOptions
      x-api-path-slug: restpropertiesgroupsoptions-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Group
      - Options
    post:
      summary: Create a group option
      description: Creates a group option
      operationId: postRestPropertiesGroupsOptions
      x-api-path-slug: restpropertiesgroupsoptions-post
      parameters:
      - in: body
        name: /rest/properties/groups/options
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: groupOptionIdentifier
        description: The groupOptionIdentifier of the group name
      - in: query
        name: propertyGroupId
        description: The ID of the property group
      - in: query
        name: value
        description: The value of the group name
      responses:
        200:
          description: OK
      tags:
      - Group
      - Option
  /rest/properties/options:
    get:
      summary: List property options
      description: Lists property options.
      operationId: getRestPropertiesOptions
      x-api-path-slug: restpropertiesoptions-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Options
    post:
      summary: Create a property option
      description: Creates a property option.
      operationId: postRestPropertiesOptions
      x-api-path-slug: restpropertiesoptions-post
      parameters:
      - in: body
        name: /rest/properties/options
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: propertyId
        description: ID of the property
      - in: query
        name: typeOptionIdentifier
        description: The identifier of the property option type
      responses:
        200:
          description: OK
      tags:
      - Property
      - Option
  /rest/accounts/addresses/option_types:
    get:
      summary: List address option types
      description: List address option types.
      operationId: getRestAccountsAddressesOptionTypes
      x-api-path-slug: restaccountsaddressesoption-types-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Address
      - Option
      - Types
    post:
      summary: Create an address option type
      description: Create an address option type.
      operationId: postRestAccountsAddressesOptionTypes
      x-api-path-slug: restaccountsaddressesoption-types-post
      parameters:
      - in: body
        name: /rest/accounts/addresses/option_types
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Address
      - Option
      - Type
  /rest/accounts/addresses/option_types/{optionTypeId}:
    delete:
      summary: Delete an address option type
      description: Deletes an address option type. The ID of the option type must
        be specified.
      operationId: deleteRestAccountsAddressesOptionTypesOptiontype
      x-api-path-slug: restaccountsaddressesoption-typesoptiontypeid-delete
      parameters:
      - in: path
        name: optionTypeId
      responses:
        200:
          description: OK
      tags:
      - Address
      - Option
      - Type
    get:
      summary: Get an address option type
      description: Gets an address option type. The ID of the option type must be
        specified.
      operationId: getRestAccountsAddressesOptionTypesOptiontype
      x-api-path-slug: restaccountsaddressesoption-typesoptiontypeid-get
      parameters:
      - in: path
        name: optionTypeId
      responses:
        200:
          description: OK
      tags:
      - Address
      - Option
      - Type
    put:
      summary: Update an address option type
      description: Updates an address option type. The ID of the option type must
        be specified.
      operationId: putRestAccountsAddressesOptionTypesOptiontype
      x-api-path-slug: restaccountsaddressesoption-typesoptiontypeid-put
      parameters:
      - in: body
        name: /rest/accounts/addresses/option_types/{optionTypeId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: optionTypeId
      responses:
        200:
          description: OK
      tags:
      - Address
      - Option
      - Type
  /rest/accounts/addresses/options/{optionId}:
    delete:
      summary: Delete an address option by the option ID
      description: Deletes an address option. The ID of the option must be specified.
      operationId: deleteRestAccountsAddressesOptionsOption
      x-api-path-slug: restaccountsaddressesoptionsoptionid-delete
      parameters:
      - in: path
        name: optionId
      responses:
        200:
          description: OK
      tags:
      - Address
      - Option
      - By
      - Option
      - ID
    get:
      summary: Get an address option
      description: Gets an address option. The ID of the option must be specified.
      operationId: getRestAccountsAddressesOptionsOption
      x-api-path-slug: restaccountsaddressesoptionsoptionid-get
      parameters:
      - in: path
        name: optionId
      responses:
        200:
          description: OK
      tags:
      - Address
      - Option
    put:
      summary: Update an address option
      description: Updates an address option. The ID of the option must be specified.
      operationId: putRestAccountsAddressesOptionsOption
      x-api-path-slug: restaccountsaddressesoptionsoptionid-put
      parameters:
      - in: path
        name: optionId
      responses:
        200:
          description: OK
      tags:
      - Address
      - Option
  /rest/accounts/contacts/option_sub_types:
    get:
      summary: List contact option sub-types
      description: List contact option sub-types.
      operationId: getRestAccountsContactsOptionSubTypes
      x-api-path-slug: restaccountscontactsoption-sub-types-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Contact
      - Option
      - Sub-types
    post:
      summary: Create a contact option sub-type
      description: Create a contact option sub-type.
      operationId: postRestAccountsContactsOptionSubTypes
      x-api-path-slug: restaccountscontactsoption-sub-types-post
      parameters:
      - in: body
        name: /rest/accounts/contacts/option_sub_types
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Option
      - Sub-type
  /rest/accounts/contacts/option_sub_types/{optionSubTypeId}:
    delete:
      summary: Delete a contact option sub-type
      description: Deletes a contact option sub-type. The ID of the option sub-type
        must be specified.
      operationId: deleteRestAccountsContactsOptionSubTypesOptionsubtype
      x-api-path-slug: restaccountscontactsoption-sub-typesoptionsubtypeid-delete
      parameters:
      - in: path
        name: optionSubTypeId
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Option
      - Sub-type
    get:
      summary: Get a contact option sub-type
      description: Gets a contact option sub-type. The ID of the option sub-type must
        be specified.
      operationId: getRestAccountsContactsOptionSubTypesOptionsubtype
      x-api-path-slug: restaccountscontactsoption-sub-typesoptionsubtypeid-get
      parameters:
      - in: path
        name: optionSubTypeId
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Option
      - Sub-type
    put:
      summary: Update a contact option sub-type
      description: Updates a contact option sub-type. The ID of the option sub-type
        must be specified.
      operationId: putRestAccountsContactsOptionSubTypesOptionsubtype
      x-api-path-slug: restaccountscontactsoption-sub-typesoptionsubtypeid-put
      parameters:
      - in: body
        name: /rest/accounts/contacts/option_sub_types/{optionSubTypeId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: optionSubTypeId
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Option
      - Sub-type
  /rest/accounts/contacts/option_types:
    get:
      summary: List contact option types
      description: List contact option types.
      operationId: getRestAccountsContactsOptionTypes
      x-api-path-slug: restaccountscontactsoption-types-get
      parameters:
      - in: query
        name: with
        description: Lists possible option sub-types for each listed option if the
          parameter subTypes is set
      responses:
        200:
          description: OK
      tags:
      - List
      - Contact
      - Option
      - Types
    post:
      summary: Create a contact option type
      description: Create a contact option type.
      operationId: postRestAccountsContactsOptionTypes
      x-api-path-slug: restaccountscontactsoption-types-post
      parameters:
      - in: body
        name: /rest/accounts/contacts/option_types
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Option
      - Type
  /rest/accounts/contacts/option_types/{optionTypeId}:
    delete:
      summary: Delete a contact option type
      description: Deletes a contact option type. The ID of the option type must be
        specified.
      operationId: deleteRestAccountsContactsOptionTypesOptiontype
      x-api-path-slug: restaccountscontactsoption-typesoptiontypeid-delete
      parameters:
      - in: path
        name: optionTypeId
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Option
      - Type
    get:
      summary: Get a contact option type
      description: Gets a contact option type. The ID of the option type must be specified.
      operationId: getRestAccountsContactsOptionTypesOptiontype
      x-api-path-slug: restaccountscontactsoption-typesoptiontypeid-get
      parameters:
      - in: path
        name: optionTypeId
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Option
      - Type
    put:
      summary: Update a contact option type
      description: Updates a contact option type. The ID of the option type must be
        specified.
      operationId: putRestAccountsContactsOptionTypesOptiontype
      x-api-path-slug: restaccountscontactsoption-typesoptiontypeid-put
      parameters:
      - in: body
        name: /rest/accounts/contacts/option_types/{optionTypeId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: optionTypeId
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Option
      - Type
  /rest/accounts/contacts/options/{optionId}:
    delete:
      summary: Delete a contact option by the option ID
      description: Deletes a contact option. The ID of the option must be specified.
      operationId: deleteRestAccountsContactsOptionsOption
      x-api-path-slug: restaccountscontactsoptionsoptionid-delete
      parameters:
      - in: path
        name: optionId
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Option
      - By
      - Option
      - ID
    get:
      summary: Get a contact option by the option ID
      description: Gets a contact option. The ID of the option must be specified.
      operationId: getRestAccountsContactsOptionsOption
      x-api-path-slug: restaccountscontactsoptionsoptionid-get
      parameters:
      - in: path
        name: optionId
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Option
      - By
      - Option
      - ID
    put:
      summary: Update a contact option by the option ID
      description: Updates a contact option. The ID of the option must be specified.
      operationId: putRestAccountsContactsOptionsOption
      x-api-path-slug: restaccountscontactsoptionsoptionid-put
      parameters:
      - in: path
        name: optionId
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Option
      - By
      - Option
      - ID
  /rest/accounts/contacts/{contactId}/options/validate:
    get:
      summary: Validate a contact option by a given value
      description: validates a contact option by a given value
      operationId: getRestAccountsContactsContactOptionsValate
      x-api-path-slug: restaccountscontactscontactidoptionsvalidate-get
      parameters:
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - Validate
      - Contact
      - Option
      - By
      - Given
      - Value
  /rest/listings/option_templates:
    post:
      summary: Create option template
      description: Creates an option template.
      operationId: postRestListingsOptionTemplates
      x-api-path-slug: restlistingsoption-templates-post
      parameters:
      - in: body
        name: /rest/listings/option_templates
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Option
      - Template
  /rest/listings/option_templates/preview:
    get:
      summary: Get a preview list of option templates
      description: Gets a preview list of all available listing option templates.
      operationId: getRestListingsOptionTemplatesPreview
      x-api-path-slug: restlistingsoption-templatespreview-get
      responses:
        200:
          description: OK
      tags:
      - Preview
      - List
      - Of
      - Option
      - Templates
  /rest/listings/option_templates/{id}:
    delete:
      summary: Delete option template
      description: Deletes an option template by ID.
      operationId: deleteRestListingsOptionTemplates
      x-api-path-slug: restlistingsoption-templatesid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Option
      - Template
    get:
      summary: Get option template
      description: Gets an option template by ID.
      operationId: getRestListingsOptionTemplates
      x-api-path-slug: restlistingsoption-templatesid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Option
      - Template
    put:
      summary: Update option template
      description: Updates an option template by ID.
      operationId: putRestListingsOptionTemplates
      x-api-path-slug: restlistingsoption-templatesid-put
      parameters:
      - in: body
        name: /rest/listings/option_templates/{id}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Option
      - Template
  /rest/properties/groups/options/{groupOptionId}:
    delete:
      summary: Delete a group option
      description: Deletes a group option. The ID of the group option must be specified.
      operationId: deleteRestPropertiesGroupsOptionsGroupoption
      x-api-path-slug: restpropertiesgroupsoptionsgroupoptionid-delete
      parameters:
      - in: path
        name: groupOptionId
      responses:
        200:
          description: OK
      tags:
      - Group
      - Option
    get:
      summary: Get a group option
      description: Gets a group option. The ID of the group option must be specified.
      operationId: getRestPropertiesGroupsOptionsGroupoption
      x-api-path-slug: restpropertiesgroupsoptionsgroupoptionid-get
      parameters:
      - in: path
        name: groupOptionId
      responses:
        200:
          description: OK
      tags:
      - Group
      - Option
    put:
      summary: Update a group option
      description: Updates a group option. The ID of the group option must be specified.
      operationId: putRestPropertiesGroupsOptionsGroupoption
      x-api-path-slug: restpropertiesgroupsoptionsgroupoptionid-put
      parameters:
      - in: path
        name: groupOptionId
      responses:
        200:
          description: OK
      tags:
      - Group
      - Option
  /rest/properties/options/{propertyOptionId}:
    delete:
      summary: Delete a property option
      description: Deletes a property option. The ID of the proeprty option must be
        specified.
      operationId: deleteRestPropertiesOptionsPropertyoption
      x-api-path-slug: restpropertiesoptionspropertyoptionid-delete
      parameters:
      - in: path
        name: propertyOptionId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Option
    get:
      summary: Get a property option
      description: Gets a property option. The ID of the property option must be specified.
      operationId: getRestPropertiesOptionsPropertyoption
      x-api-path-slug: restpropertiesoptionspropertyoptionid-get
      parameters:
      - in: path
        name: propertyOptionId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Option
    put:
      summary: Update a property option
      description: Updates a property option. The ID of the property option must be
        specified.
      operationId: putRestPropertiesOptionsPropertyoption
      x-api-path-slug: restpropertiesoptionspropertyoptionid-put
      parameters:
      - in: query
        name: $propertyOptionId
        description: The ID of the property option
      - in: path
        name: propertyOptionId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Option
  /rest/accounts/contacts/group_functions:
    post:
      summary: Apply selected group function options for given contact IDs
      description: Applies selected group function options for given contact IDs.
      operationId: postRestAccountsContactsGroupFunctions
      x-api-path-slug: restaccountscontactsgroup-functions-post
      parameters:
      - in: query
        name: addressLabelTemplate
        description: An address label template ID
      - in: query
        name: contactList
        description: A list of contact IDs
      - in: query
        name: emailTemplate
        description: An email template ID
      - in: query
        name: newsletter
        description: A newsletter folder ID
      responses:
        200:
          description: OK
      tags:
      - Apply
      - Selected
      - Group
      - Function
      - Optionsgiven
      - Contact
      - IDs
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