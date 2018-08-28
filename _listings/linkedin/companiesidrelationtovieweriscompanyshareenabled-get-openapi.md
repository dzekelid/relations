---
swagger: "2.0"
x-collection-name: LinkedIn
x-complete: 0
info:
  title: LinkedIn Get Companies Relation To Viewer Is Company Share Enabled
  description: Get companies  relation to viewer is company share enabled
  version: 1.0.0
host: api.linkedin.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /companies/{id}/relation-to-viewer/is-company-share-enabled:
    get:
      summary: Get Companies Relation To Viewer Is Company Share Enabled
      description: Get companies  relation to viewer is company share enabled
      operationId: getCompaniesRelationToViewerIsCompanyShareEnabled
      x-api-path-slug: companiesidrelationtovieweriscompanyshareenabled-get
      responses:
        200:
          description: OK
      tags:
      - Companies
      - ""
      - Relation
      - To
      - Viewer
      - Is
      - Company
      - Share
      - Enabled
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