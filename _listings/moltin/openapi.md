swagger: "2.0"
x-collection-name: moltin
x-complete: 1
info:
  title: Moltin
  description: -welcomethis-is-a-place-to-put-general-notes-and-extra-information-for-internal-use-to-get-started-designingdocumenting-this-api-select-a-version-on-the-left-
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