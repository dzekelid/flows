---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Insights Get Flows
  description: Get flows.
  termsOfService: urn:tos
  version: 1.0.0
host: insights-api.data-services.predix.io
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /flow-templates/{flowTemplateId}/flows:
    get:
      summary: Get Flow Templates Flowtemplateid Flows
      description: Get flow templates flowtemplateid flows.
      operationId: getFlowsUsingGET_1
      x-api-path-slug: flowtemplatesflowtemplateidflows-get
      parameters:
      - in: path
        name: flowTemplateId
        description: flowTemplateId
      - in: query
        name: maxUpdateTime
        description: maxUpdateTime
      - in: query
        name: minUpdateTime
        description: minUpdateTime
      - in: query
        name: name
        description: name
      - in: query
        name: page
        description: Results page you want to retrieve (0
      - in: query
        name: size
        description: Number of records per page
      - in: query
        name: sort
        description: 'Sorting criteria in the format: property(,asc|desc)'
      - in: query
        name: tag
        description: tag
      - in: query
        name: type
        description: type
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
      - Flows
    post:
      summary: Post Flow Templates Flowtemplateid Flows
      description: Post flow templates flowtemplateid flows.
      operationId: saveFlowUsingPOST_1
      x-api-path-slug: flowtemplatesflowtemplateidflows-post
      parameters:
      - in: path
        name: flowTemplateId
        description: flowTemplateId
      - in: query
        name: launch
        description: launch
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
      - Flows
  /flow-templates/{flowTemplateId}/flows/{flowId}:
    get:
      summary: Get Flow Templates Flowtemplateid Flows Flowid
      description: Get flow templates flowtemplateid flows flowid.
      operationId: getFlowUsingGET_1
      x-api-path-slug: flowtemplatesflowtemplateidflowsflowid-get
      parameters:
      - in: path
        name: flowId
        description: flowId
      - in: path
        name: flowTemplateId
        description: flowTemplateId
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
      - Flows
      - Flowid
    post:
      summary: Post Flow Templates Flowtemplateid Flows Flowid
      description: Post flow templates flowtemplateid flows flowid.
      operationId: updateFlowUsingPOST_1
      x-api-path-slug: flowtemplatesflowtemplateidflowsflowid-post
      parameters:
      - in: body
        name: flow
        description: flow
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: flowId
        description: flowId
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
      - Flows
      - Flowid
    delete:
      summary: Delete Flow Templates Flowtemplateid Flows Flowid
      description: Delete flow templates flowtemplateid flows flowid.
      operationId: deleteFlowUsingDELETE_1
      x-api-path-slug: flowtemplatesflowtemplateidflowsflowid-delete
      parameters:
      - in: path
        name: flowId
        description: flowId
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
      - Flows
      - Flowid
  /flow-templates/{flowTemplateId}/flows/{flowId}/config:
    get:
      summary: Get Flow Templates Flowtemplateid Flows Flowid Config
      description: Get flow templates flowtemplateid flows flowid config.
      operationId: listFlowConfigFilesUsingGET_1
      x-api-path-slug: flowtemplatesflowtemplateidflowsflowidconfig-get
      parameters:
      - in: path
        name: flowId
        description: flowId
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
      - Flows
      - Flowid
      - Config
    post:
      summary: Post Flow Templates Flowtemplateid Flows Flowid Config
      description: Post flow templates flowtemplateid flows flowid config.
      operationId: addFlowConfigFileUsingPOST_1
      x-api-path-slug: flowtemplatesflowtemplateidflowsflowidconfig-post
      parameters:
      - in: path
        name: flowId
        description: flowId
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
      - Flows
      - Flowid
      - Config
  /flow-templates/{flowTemplateId}/flows/{flowId}/config/{fileName}:
    get:
      summary: Get Flow Templates Flowtemplateid Flows Flowid Config Filename
      description: Get flow templates flowtemplateid flows flowid config filename.
      operationId: getFlowConfigFileUsingGET_1
      x-api-path-slug: flowtemplatesflowtemplateidflowsflowidconfigfilename-get
      parameters:
      - in: path
        name: fileName
        description: fileName
      - in: path
        name: flowId
        description: flowId
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
      - Flows
      - Flowid
      - Config
      - Filename
    delete:
      summary: Delete Flow Templates Flowtemplateid Flows Flowid Config Filename
      description: Delete flow templates flowtemplateid flows flowid config filename.
      operationId: deleteFlowConfigFileUsingDELETE_1
      x-api-path-slug: flowtemplatesflowtemplateidflowsflowidconfigfilename-delete
      parameters:
      - in: path
        name: fileName
        description: fileName
      - in: path
        name: flowId
        description: flowId
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
      - Flows
      - Flowid
      - Config
      - Filename
  /flow-templates/{flowTemplateId}/flows/{flowId}/launch:
    post:
      summary: Post Flow Templates Flowtemplateid Flows Flowid Launch
      description: Post flow templates flowtemplateid flows flowid launch.
      operationId: launchUsingPOST_1
      x-api-path-slug: flowtemplatesflowtemplateidflowsflowidlaunch-post
      parameters:
      - in: path
        name: flowId
        description: flowId
      - in: body
        name: launchRequest
        description: launchRequest
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
      - Flows
      - Flowid
      - Launch
  /flow-templates/{flowTemplateId}/flows/{flowId}/stop:
    post:
      summary: Post Flow Templates Flowtemplateid Flows Flowid Stop
      description: Post flow templates flowtemplateid flows flowid stop.
      operationId: stopUsingPOST_1
      x-api-path-slug: flowtemplatesflowtemplateidflowsflowidstop-post
      parameters:
      - in: path
        name: flowId
        description: flowId
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
      - Flows
      - Flowid
      - Stop
  /flow-templates/{flowTemplateId}/flows/{flowId}/tags:
    get:
      summary: Get Flow Templates Flowtemplateid Flows Flowid Tags
      description: Get flow templates flowtemplateid flows flowid tags.
      operationId: getFlowTagsUsingGET
      x-api-path-slug: flowtemplatesflowtemplateidflowsflowidtags-get
      parameters:
      - in: path
        name: flowId
        description: flowId
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
      - Flows
      - Flowid
      - Tags
    post:
      summary: Post Flow Templates Flowtemplateid Flows Flowid Tags
      description: Post flow templates flowtemplateid flows flowid tags.
      operationId: saveFlowTagsUsingPOST_1
      x-api-path-slug: flowtemplatesflowtemplateidflowsflowidtags-post
      parameters:
      - in: path
        name: flowId
        description: flowId
      - in: body
        name: tags
        description: tags
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
      - Flows
      - Flowid
      - Tags
  /flows:
    get:
      summary: Get Flows
      description: Get flows.
      operationId: getFlowsUsingGET
      x-api-path-slug: flows-get
      parameters:
      - in: query
        name: maxUpdateTime
        description: maxUpdateTime
      - in: query
        name: minUpdateTime
        description: minUpdateTime
      - in: query
        name: name
        description: name
      - in: query
        name: page
        description: Results page you want to retrieve (0
      - in: query
        name: size
        description: Number of records per page
      - in: query
        name: sort
        description: 'Sorting criteria in the format: property(,asc|desc)'
      - in: query
        name: tag
        description: tag
      - in: query
        name: type
        description: type
      responses:
        200:
          description: Successful response
      tags:
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