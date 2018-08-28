---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Create an address warehouse relation
  description: Create an address warehouse relation.
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
  /rest/accounts/addresses/contact_relations:
    get:
      summary: List address contact relations
      description: List address contact relations.
      operationId: getRestAccountsAddressesContactRelations
      x-api-path-slug: restaccountsaddressescontact-relations-get
      parameters:
      - in: query
        name: addressId
        description: Filter that restricts the search result to addresses with a specific
          ID
      - in: query
        name: contactId
        description: Filter that restricts the search result to contacts with a specific
          ID
      - in: query
        name: id
        description: Filter that restricts the search result to address contact relations
          with a specific ID
      - in: query
        name: isPrimary
        description: Filter that restricts the search result depending on the flag
          used
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: typeId
        description: Filter that restricts the search result to address types with
          a specific ID
      - in: query
        name: with
        description: Includes the specified address contact relation information in
          the results
      responses:
        200:
          description: OK
      tags:
      - List
      - Address
      - Contact
      - Relations
    post:
      summary: Create address contact relations
      description: Create address contact relations.
      operationId: postRestAccountsAddressesContactRelations
      x-api-path-slug: restaccountsaddressescontact-relations-post
      parameters:
      - in: body
        name: /rest/accounts/addresses/contact_relations
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Address
      - Contact
      - Relations
    put:
      summary: Update address contact relations
      description: Update address contact relations.
      operationId: putRestAccountsAddressesContactRelations
      x-api-path-slug: restaccountsaddressescontact-relations-put
      parameters:
      - in: body
        name: /rest/accounts/addresses/contact_relations
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Address
      - Contact
      - Relations
  /rest/accounts/addresses/pos_relations:
    get:
      summary: List address POS relations
      description: List address pos relations.
      operationId: getRestAccountsAddressesPosRelations
      x-api-path-slug: restaccountsaddressespos-relations-get
      parameters:
      - in: query
        name: itemsPerPage
        description: items per page
      - in: query
        name: page
        description: page
      - in: query
        name: with
        description: Includes the specified address pos relation information in the
          results
      responses:
        200:
          description: OK
      tags:
      - List
      - Address
      - POS
      - Relations
    post:
      summary: Create an address POS relation
      description: Create an address pos relation.
      operationId: postRestAccountsAddressesPosRelations
      x-api-path-slug: restaccountsaddressespos-relations-post
      responses:
        200:
          description: OK
      tags:
      - Address
      - POS
      - Relation
  /rest/items/variations/variation_sales_prices:
    get:
      summary: Get all sales price relations
      description: Gets all links between variations and sales prices including sales
        price data.
      operationId: getRestItemsVariationsVariationSalesPrices
      x-api-path-slug: restitemsvariationsvariation-sales-prices-get
      parameters:
      - in: query
        name: salesPriceId
        description: Filter that restricts the search result to the sales price data
          of variations linked to a specific sales price
      - in: query
        name: updatedAt
        description: Filter that restricts the search result to links between variations
          and sales prices updated after a specific point in time
      - in: query
        name: variationId
        description: Filter that restricts the search result to the sales price data
          of a specific variation
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Price
      - Relations
  /rest/properties/relations:
    delete:
      summary: Delete property relations
      description: Deletes property relations. The ID of the property relations must
        be specified.
      operationId: deleteRestPropertiesRelations
      x-api-path-slug: restpropertiesrelations-delete
      parameters:
      - in: query
        name: relationId
        description: The ID of the property relation
      responses:
        200:
          description: OK
      tags:
      - Property
      - Relations
    get:
      summary: List property relations
      description: Lists property relations.
      operationId: getRestPropertiesRelations
      x-api-path-slug: restpropertiesrelations-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Relations
    put:
      summary: Update relations
      description: Updates relations
      operationId: putRestPropertiesRelations
      x-api-path-slug: restpropertiesrelations-put
      parameters:
      - in: query
        name: relationId
        description: The ID of the property relation
      responses:
        200:
          description: OK
      tags:
      - Relations
    post:
      summary: Create a property relation
      description: Creates a property relation
      operationId: postRestPropertiesRelations
      x-api-path-slug: restpropertiesrelations-post
      parameters:
      - in: body
        name: /rest/properties/relations
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: propertyId
        description: The ID of the property
      - in: query
        name: relationTargetId
        description: The ID of the property relation target
      - in: query
        name: relationTypeIdentifier
        description: The identifier of the property relation type
      - in: query
        name: selectionRelationId
        description: The ID of the property selection relation
      responses:
        200:
          description: OK
      tags:
      - Property
      - Relation
  /rest/accounts/addresses/contact_relations/{addressContactRelationId}:
    delete:
      summary: Delete an address contact relation
      description: Deletes an address contact relation. The ID of the relation must
        be specified.
      operationId: deleteRestAccountsAddressesContactRelationsAddresscontactrelation
      x-api-path-slug: restaccountsaddressescontact-relationsaddresscontactrelationid-delete
      parameters:
      - in: path
        name: addressContactRelationId
      responses:
        200:
          description: OK
      tags:
      - Address
      - Contact
      - Relation
    get:
      summary: Get an address contact relation
      description: Gets an address contact relation. The ID of the address contact
        relation must be specified.
      operationId: getRestAccountsAddressesContactRelationsAddresscontactrelation
      x-api-path-slug: restaccountsaddressescontact-relationsaddresscontactrelationid-get
      parameters:
      - in: path
        name: addressContactRelationId
      responses:
        200:
          description: OK
      tags:
      - Address
      - Contact
      - Relation
  /rest/accounts/addresses/pos_relations/{addressPosRelationId}:
    delete:
      summary: Delete an address POS relation
      description: Deletes an address POS relation. The ID of the address POS relation
        must be specified.
      operationId: deleteRestAccountsAddressesPosRelationsAddressposrelation
      x-api-path-slug: restaccountsaddressespos-relationsaddressposrelationid-delete
      parameters:
      - in: path
        name: addressPosRelationId
      responses:
        200:
          description: OK
      tags:
      - Address
      - POS
      - Relation
    get:
      summary: Get an address POS relation
      description: Gets an address POS relation. The ID of the address POS relation
        must be specified.
      operationId: getRestAccountsAddressesPosRelationsAddressposrelation
      x-api-path-slug: restaccountsaddressespos-relationsaddressposrelationid-get
      parameters:
      - in: path
        name: addressPosRelationId
      responses:
        200:
          description: OK
      tags:
      - Address
      - POS
      - Relation
    put:
      summary: Update an address POS relation
      description: Updates an address POS relation. The ID of the address POS relation
        must be specified.
      operationId: putRestAccountsAddressesPosRelationsAddressposrelation
      x-api-path-slug: restaccountsaddressespos-relationsaddressposrelationid-put
      parameters:
      - in: path
        name: addressPosRelationId
      responses:
        200:
          description: OK
      tags:
      - Address
      - POS
      - Relation
  /rest/accounts/addresses/relation_types:
    get:
      summary: List address relation types
      description: List address relation types.
      operationId: getRestAccountsAddressesRelationTypes
      x-api-path-slug: restaccountsaddressesrelation-types-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Address
      - Relation
      - Types
  /rest/accounts/addresses/relations/types/applications/{application}/{lang}:
    get:
      summary: List address relation types
      description: |-
        Lists address relation types. The application and the language must be specified.
        <br>Possible applications:
        <ul>
        <li>contact</li>
        <li>order</li>
        <li>warehouse</li>
        <li>pos</li>
        </ul>
      operationId: getRestAccountsAddressesRelationsTypesApplicationsApplicationLang
      x-api-path-slug: restaccountsaddressesrelationstypesapplicationsapplicationlang-get
      parameters:
      - in: path
        name: application
      - in: path
        name: lang
      responses:
        200:
          description: OK
      tags:
      - List
      - Address
      - Relation
      - Types
  /rest/accounts/addresses/warehouse_relations:
    post:
      summary: Create an address warehouse relation
      description: Create an address warehouse relation.
      operationId: postRestAccountsAddressesWarehouseRelations
      x-api-path-slug: restaccountsaddresseswarehouse-relations-post
      responses:
        200:
          description: OK
      tags:
      - Address
      - Warehouse
      - Relation
  /rest/accounts/addresses/warehouse_relations/{relationId}:
    delete:
      summary: Delete an address warehouse relation
      description: Deletes an address warehouse relation. The ID of the relation must
        be specified.
      operationId: deleteRestAccountsAddressesWarehouseRelationsRelation
      x-api-path-slug: restaccountsaddresseswarehouse-relationsrelationid-delete
      parameters:
      - in: path
        name: relationId
      responses:
        200:
          description: OK
      tags:
      - Address
      - Warehouse
      - Relation
    put:
      summary: Update an address warehouse relation
      description: Updates an address warehouse relation. The ID of the relation must
        be specified.
      operationId: putRestAccountsAddressesWarehouseRelationsRelation
      x-api-path-slug: restaccountsaddresseswarehouse-relationsrelationid-put
      parameters:
      - in: path
        name: relationId
      responses:
        200:
          description: OK
      tags:
      - Address
      - Warehouse
      - Relation
  /rest/accounts/contact_relations/{accountContactRelationId}:
    delete:
      summary: Deletes an account contact relation. The ID of the account contact
        relation must be specified.
      description: Deletes an account contact relation. the id of the account contact
        relation must be specified..
      operationId: deleteRestAccountsContactRelationsAccountcontactrelation
      x-api-path-slug: restaccountscontact-relationsaccountcontactrelationid-delete
      parameters:
      - in: path
        name: accountContactRelationId
      responses:
        200:
          description: OK
      tags:
      - S
      - Account
      - Contact
      - Relation
      - ""
      - ID
      - Of
      - Account
      - Contact
      - Relation
      - Must
      - Be
      - Specified
    get:
      summary: Gets an account contact releation. The ID of the account contact relation
        must be specified.
      description: Gets an account contact releation. the id of the account contact
        relation must be specified..
      operationId: getRestAccountsContactRelationsAccountcontactrelation
      x-api-path-slug: restaccountscontact-relationsaccountcontactrelationid-get
      parameters:
      - in: path
        name: accountContactRelationId
      responses:
        200:
          description: OK
      tags:
      - S
      - Account
      - Contact
      - Releation
      - ""
      - ID
      - Of
      - Account
      - Contact
      - Relation
      - Must
      - Be
      - Specified
  /rest/properties/relations/markups:
    get:
      summary: List relation markups
      description: Lists relation markups.
      operationId: getRestPropertiesRelationsMarkups
      x-api-path-slug: restpropertiesrelationsmarkups-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Relation
      - Markups
    post:
      summary: Create a property relation markup
      description: Creates a property relation markup
      operationId: postRestPropertiesRelationsMarkups
      x-api-path-slug: restpropertiesrelationsmarkups-post
      parameters:
      - in: body
        name: /rest/properties/relations/markups
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: markup
        description: The property relation markup
      - in: query
        name: propertyRelationId
        description: The ID of the property elation
      - in: query
        name: variationSalesPriceId
        description: The ID of a variations sales price
      responses:
        200:
          description: OK
      tags:
      - Property
      - Relation
      - Markup
  /rest/properties/relations/markups/{relationMarkupId}:
    delete:
      summary: Delete a property relation markup
      description: Deletes a property relation markup
      operationId: deleteRestPropertiesRelationsMarkupsRelationmarkup
      x-api-path-slug: restpropertiesrelationsmarkupsrelationmarkupid-delete
      parameters:
      - in: path
        name: relationMarkupId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Relation
      - Markup
    get:
      summary: Get a property relation markup
      description: Gets a property relation markup. The ID of the property relation
        markup must be specified.
      operationId: getRestPropertiesRelationsMarkupsRelationmarkup
      x-api-path-slug: restpropertiesrelationsmarkupsrelationmarkupid-get
      parameters:
      - in: path
        name: relationMarkupId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Relation
      - Markup
    put:
      summary: Update a property relation markup
      description: Updates a property relation markup
      operationId: putRestPropertiesRelationsMarkupsRelationmarkup
      x-api-path-slug: restpropertiesrelationsmarkupsrelationmarkupid-put
      parameters:
      - in: path
        name: relationMarkupId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Relation
      - Markup
  /rest/properties/relations/values:
    get:
      summary: List property relation values
      description: Lists property relation values.
      operationId: getRestPropertiesRelationsValues
      x-api-path-slug: restpropertiesrelationsvalues-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Relation
      - Values
    post:
      summary: Create a property relation value
      description: Creates a property relation value.
      operationId: postRestPropertiesRelationsValues
      x-api-path-slug: restpropertiesrelationsvalues-post
      parameters:
      - in: body
        name: /rest/properties/relations/values
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: lang
        description: The lang of the property relation value
      - in: query
        name: propertyId
        description: The ID of the property
      - in: query
        name: value
        description: The value of the property relation
      responses:
        200:
          description: OK
      tags:
      - Property
      - Relation
      - Value
    put:
      summary: Update multiple property relation value
      description: Updates multiple property relation value
      operationId: putRestPropertiesRelationsValues
      x-api-path-slug: restpropertiesrelationsvalues-put
      responses:
        200:
          description: OK
      tags:
      - Multiple
      - Property
      - Relation
      - Value
  /rest/properties/relations/values/{propertiesRelationValueId}:
    delete:
      summary: Delete a property relation value
      description: Deletes a property relation value. The ID of the property relation
        value must be specified.
      operationId: deleteRestPropertiesRelationsValuesPropertiesrelationvalue
      x-api-path-slug: restpropertiesrelationsvaluespropertiesrelationvalueid-delete
      parameters:
      - in: path
        name: propertiesRelationValueId
      - in: query
        name: propertyRelationValueId
        description: The ID of the property relation value
      responses:
        200:
          description: OK
      tags:
      - Property
      - Relation
      - Value
    put:
      summary: Update a property relation value
      description: Updates a property relation value. The ID of the property relation
        value must be specified.
      operationId: putRestPropertiesRelationsValuesPropertiesrelationvalue
      x-api-path-slug: restpropertiesrelationsvaluespropertiesrelationvalueid-put
      parameters:
      - in: query
        name: $propertyRelationValueId
        description: The ID of the property relation value
      - in: path
        name: propertiesRelationValueId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Relation
      - Value
  /rest/properties/relations/values/{relationMarkupId}:
    get:
      summary: Get a property relation value
      description: Gets a property relation value. The ID of the property relation
        value must be specified.
      operationId: getRestPropertiesRelationsValuesRelationmarkup
      x-api-path-slug: restpropertiesrelationsvaluesrelationmarkupid-get
      parameters:
      - in: query
        name: propertyRelationId
        description: The ID of the property relation
      - in: path
        name: relationMarkupId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Relation
      - Value
  /rest/properties/relations/{relationId}:
    delete:
      summary: Delete a property relation
      description: Deletes a property relation. The ID of the property relation must
        be specified.
      operationId: deleteRestPropertiesRelationsRelation
      x-api-path-slug: restpropertiesrelationsrelationid-delete
      parameters:
      - in: path
        name: relationId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Relation
    get:
      summary: Get a property relation
      description: Gets a property relation. The ID of the property relation must
        be specified.
      operationId: getRestPropertiesRelationsRelation
      x-api-path-slug: restpropertiesrelationsrelationid-get
      parameters:
      - in: path
        name: relationId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Relation
    put:
      summary: Update a property relation
      description: Updates a property relation. The ID of the property relation must
        be specified.
      operationId: putRestPropertiesRelationsRelation
      x-api-path-slug: restpropertiesrelationsrelationid-put
      parameters:
      - in: path
        name: relationId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Relation
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