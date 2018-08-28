---
swagger: "2.0"
x-collection-name: moltin
x-complete: 0
info:
  title: Moltin API Update a flow
  description: Update a flow.
  version: 1.0.0
host: api.moltin.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/flows:
    get:
      summary: Get all flows
      description: Get all flows.
      operationId: V2FlowsGet2
      x-api-path-slug: v2flows-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Flows
    post:
      summary: Create a flow
      description: Create a flow.
      operationId: V2FlowsPost
      x-api-path-slug: v2flows-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Flow
  /v2/flows/{flowID}:
    get:
      summary: Get a flow
      description: Get a flow.
      operationId: V2FlowsByFlowIDGet
      x-api-path-slug: v2flowsflowid-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: flowID
      responses:
        200:
          description: Successful response
      tags:
      - Flow
    put:
      summary: Update a flow
      description: Update a flow.
      operationId: V2FlowsByFlowIDPut
      x-api-path-slug: v2flowsflowid-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: flowID
      responses:
        200:
          description: Successful response
      tags:
      - Flow
    delete:
      summary: Delete a flow
      description: Delete a flow.
      operationId: V2FlowsByFlowIDDelete
      x-api-path-slug: v2flowsflowid-delete
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: flowID
      responses:
        200:
          description: Successful response
      tags:
      - Flow
  /v2/flows/{flowSlug}/entries:
    get:
      summary: Get all entries on a flow
      description: Get all entries on a flow.
      operationId: V2FlowsEntriesByFlowSlugGet
      x-api-path-slug: v2flowsflowslugentries-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: flowSlug
      responses:
        200:
          description: Successful response
      tags:
      - Entries
      - "On"
      - Flow
  /v2/flows/{flowSlug}/fields:
    get:
      summary: Get all fields on a flow
      description: Get all fields on a flow.
      operationId: V2FlowsFieldsByFlowSlugGet
      x-api-path-slug: v2flowsflowslugfields-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: flowSlug
      responses:
        200:
          description: Successful response
      tags:
      - Fields
      - "On"
      - Flow
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