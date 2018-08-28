swagger: "2.0"
x-collection-name: LinkedIn
x-complete: 1
info:
  title: LinkedIn
  description: bring-user-profiles-and-professional-networks-to-your-apps-
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