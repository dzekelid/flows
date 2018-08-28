---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Insights Get Flow Templates Flowtemplateid Download
  description: Get flow templates flowtemplateid download.
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
    post:
      summary: Post Flows
      description: Post flows.
      operationId: saveDirectFlowUsingPOST
      x-api-path-slug: flows-post
      responses:
        200:
          description: Successful response
      tags:
      - Flows
  /flows/tags:
    get:
      summary: Get Flows Tags
      description: Get flows tags.
      operationId: getAllFlowTagsUsingGET
      x-api-path-slug: flowstags-get
      responses:
        200:
          description: Successful response
      tags:
      - Flows
      - Tags
  /flows/{flowId}:
    post:
      summary: Post Flows Flowid
      description: Post flows flowid.
      operationId: updateDirectFlowUsingPOST
      x-api-path-slug: flowsflowid-post
      parameters:
      - in: path
        name: flowId
        description: flowId
      responses:
        200:
          description: Successful response
      tags:
      - Flows
      - Flowid
    delete:
      summary: Delete Flows Flowid
      description: Delete flows flowid.
      operationId: deleteFlowUsingDELETE
      x-api-path-slug: flowsflowid-delete
      parameters:
      - in: path
        name: flowId
        description: flowId
      responses:
        200:
          description: Successful response
      tags:
      - Flows
      - Flowid
  /flows/{flowId}/config:
    get:
      summary: Get Flows Flowid Config
      description: Get flows flowid config.
      operationId: listFlowConfigFilesUsingGET
      x-api-path-slug: flowsflowidconfig-get
      parameters:
      - in: path
        name: flowId
        description: flowId
      responses:
        200:
          description: Successful response
      tags:
      - Flows
      - Flowid
      - Config
    post:
      summary: Post Flows Flowid Config
      description: Post flows flowid config.
      operationId: addFlowConfigFileUsingPOST
      x-api-path-slug: flowsflowidconfig-post
      parameters:
      - in: path
        name: flowId
        description: flowId
      responses:
        200:
          description: Successful response
      tags:
      - Flows
      - Flowid
      - Config
  /flows/{flowId}/config/{fileName}:
    get:
      summary: Get Flows Flowid Config Filename
      description: Get flows flowid config filename.
      operationId: getFlowConfigFileUsingGET
      x-api-path-slug: flowsflowidconfigfilename-get
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
      - Flows
      - Flowid
      - Config
      - Filename
    delete:
      summary: Delete Flows Flowid Config Filename
      description: Delete flows flowid config filename.
      operationId: deleteFlowConfigFileUsingDELETE
      x-api-path-slug: flowsflowidconfigfilename-delete
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
      - Flows
      - Flowid
      - Config
      - Filename
  /flows/{flowId}/create-template:
    post:
      summary: Post Flows Flowid Create Template
      description: Post flows flowid create template.
      operationId: createTemplateFromDirectFlowUsingPOST
      x-api-path-slug: flowsflowidcreatetemplate-post
      parameters:
      - in: path
        name: flowId
        description: flowId
      responses:
        200:
          description: Successful response
      tags:
      - Flows
      - Flowid
      - Template
  /flows/{flowId}/download:
    get:
      summary: Get Flows Flowid Download
      description: Get flows flowid download.
      operationId: getFlowAnalyticFileUsingGET
      x-api-path-slug: flowsflowiddownload-get
      parameters:
      - in: path
        name: flowId
        description: flowId
      responses:
        200:
          description: Successful response
      tags:
      - Flows
      - Flowid
      - Download
  /flows/{flowId}/tags:
    post:
      summary: Post Flows Flowid Tags
      description: Post flows flowid tags.
      operationId: saveFlowTagsUsingPOST
      x-api-path-slug: flowsflowidtags-post
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
      - Flows
      - Flowid
      - Tags
  /flows/{flowName}:
    get:
      summary: Get Flows Flowname
      description: Get flows flowname.
      operationId: getFlowUsingGET
      x-api-path-slug: flowsflowname-get
      parameters:
      - in: path
        name: flowName
        description: flowName
      - in: query
        name: id
        description: id
      responses:
        200:
          description: Successful response
      tags:
      - Flows
      - Flowname
  /flows/{flowName}/launch:
    post:
      summary: Post Flows Flowname Launch
      description: Post flows flowname launch.
      operationId: launchUsingPOST
      x-api-path-slug: flowsflownamelaunch-post
      parameters:
      - in: path
        name: flowName
        description: flowName
      - in: body
        name: launchRequest
        description: launchRequest
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Flows
      - Flowname
      - Launch
  /flows/{flowName}/stop:
    post:
      summary: Post Flows Flowname Stop
      description: Post flows flowname stop.
      operationId: stopUsingPOST
      x-api-path-slug: flowsflownamestop-post
      parameters:
      - in: path
        name: flowName
        description: flowName
      responses:
        200:
          description: Successful response
      tags:
      - Flows
      - Flowname
      - Stop
  /flow-templates:
    get:
      summary: Get Flow Templates
      description: Get flow templates.
      operationId: getFlowTemplatesUsingGET
      x-api-path-slug: flowtemplates-get
      parameters:
      - in: query
        name: displayShellTemplates
        description: displayShellTemplates
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
    post:
      summary: Post Flow Templates
      description: Post flow templates.
      operationId: saveFlowTemplateUsingPOST
      x-api-path-slug: flowtemplates-post
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
  /flow-templates/tags:
    get:
      summary: Get Flow Templates Tags
      description: Get flow templates tags.
      operationId: getAllFlowTemplateTagsUsingGET
      x-api-path-slug: flowtemplatestags-get
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Tags
  /flow-templates/{flowTemplateId}:
    get:
      summary: Get Flow Templates Flowtemplateid
      description: Get flow templates flowtemplateid.
      operationId: getFlowTemplateUsingGET
      x-api-path-slug: flowtemplatesflowtemplateid-get
      parameters:
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
    post:
      summary: Post Flow Templates Flowtemplateid
      description: Post flow templates flowtemplateid.
      operationId: updateFlowTemplateUsingPOST
      x-api-path-slug: flowtemplatesflowtemplateid-post
      parameters:
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
    put:
      summary: Put Flow Templates Flowtemplateid
      description: Put flow templates flowtemplateid.
      operationId: updateFlowTemplateUsingPUT
      x-api-path-slug: flowtemplatesflowtemplateid-put
      parameters:
      - in: body
        name: flowTemplate
        description: flowTemplate
        schema:
          $ref: '#/definitions/holder'
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
    delete:
      summary: Delete Flow Templates Flowtemplateid
      description: Delete flow templates flowtemplateid.
      operationId: deleteFlowTemplateUsingDELETE
      x-api-path-slug: flowtemplatesflowtemplateid-delete
      parameters:
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
  /flow-templates/{flowTemplateId}/download:
    get:
      summary: Get Flow Templates Flowtemplateid Download
      description: Get flow templates flowtemplateid download.
      operationId: getFlowTemplateFileUsingGET
      x-api-path-slug: flowtemplatesflowtemplateiddownload-get
      parameters:
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
      - Download
  /flow-templates/{flowTemplateId}/list:
    get:
      summary: Get Flow Templates Flowtemplateid List
      description: Get flow templates flowtemplateid list.
      operationId: listFlowTemplateAnalyticFileUsingGET
      x-api-path-slug: flowtemplatesflowtemplateidlist-get
      parameters:
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
      - List
  /flow-templates/{flowTemplateId}/tags:
    get:
      summary: Get Flow Templates Flowtemplateid Tags
      description: Get flow templates flowtemplateid tags.
      operationId: getTemplateTagsUsingGET
      x-api-path-slug: flowtemplatesflowtemplateidtags-get
      parameters:
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
      - Tags
    post:
      summary: Post Flow Templates Flowtemplateid Tags
      description: Post flow templates flowtemplateid tags.
      operationId: saveTemplateTagsUsingPOST
      x-api-path-slug: flowtemplatesflowtemplateidtags-post
      parameters:
      - in: path
        name: flowTemplateId
        description: flowTemplateId
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
      - Tags
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