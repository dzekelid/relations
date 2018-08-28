---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Delete property relations
  description: Deletes property relations. The ID of the property relations must be
    specified.
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