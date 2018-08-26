---
swagger: "2.0"
x-collection-name: Docsmore
x-complete: 0
info:
  title: Docsmore Get All Document Flows
  description: Get all document flows.
  version: "1.0"
host: api.docsmore.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/docflow/getdocflows:
    get:
      summary: Get All Document Flows
      description: Get all document flows.
      operationId: ApiDocflowGetdocflowsGet
      x-api-path-slug: apidocflowgetdocflows-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Document
      - Flows
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