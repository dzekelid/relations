---
swagger: "2.0"
x-collection-name: Google Partners
x-complete: 0
info:
  title: Google Partners API Delete user Company Relation
  description: Deletes a user's company relation. Unaffiliaites the user from a company.
  contact:
    name: Google
    url: https://google.com
  version: v2
host: partners.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/users/{userId}/companyRelation:
    delete:
      summary: Delete user Company Relation
      description: Deletes a user's company relation. Unaffiliaites the user from
        a company.
      operationId: partners.users.deleteCompanyRelation
      x-api-path-slug: v2usersuseridcompanyrelation-delete
      parameters:
      - in: query
        name: requestMetadata.experimentIds
        description: Experiment IDs the current request belongs to
      - in: query
        name: requestMetadata.locale
        description: Locale to use for the current request
      - in: query
        name: requestMetadata.partnersSessionId
        description: Google Partners session ID
      - in: query
        name: requestMetadata.trafficSource.trafficSourceId
        description: Identifier to indicate where the traffic comes from
      - in: query
        name: requestMetadata.trafficSource.trafficSubId
        description: Second level identifier to indicate where the traffic comes from
      - in: query
        name: requestMetadata.userOverrides.ipAddress
        description: IP address to use instead of the users geo-located IP address
      - in: query
        name: requestMetadata.userOverrides.userId
        description: Logged-in user ID to impersonate instead of the users ID
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - Relation
    put:
      summary: Create user Company Relation
      description: Creates a user's company relation. Affiliates the user to a company.
      operationId: partners.users.createCompanyRelation
      x-api-path-slug: v2usersuseridcompanyrelation-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: requestMetadata.experimentIds
        description: Experiment IDs the current request belongs to
      - in: query
        name: requestMetadata.locale
        description: Locale to use for the current request
      - in: query
        name: requestMetadata.partnersSessionId
        description: Google Partners session ID
      - in: query
        name: requestMetadata.trafficSource.trafficSourceId
        description: Identifier to indicate where the traffic comes from
      - in: query
        name: requestMetadata.trafficSource.trafficSubId
        description: Second level identifier to indicate where the traffic comes from
      - in: query
        name: requestMetadata.userOverrides.ipAddress
        description: IP address to use instead of the users geo-located IP address
      - in: query
        name: requestMetadata.userOverrides.userId
        description: Logged-in user ID to impersonate instead of the users ID
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
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