---
swagger: "2.0"
x-collection-name: CollabNet
x-complete: 0
info:
  title: CollabNet TeamForge API Documentation Removes integration data for an object
    by namespace name
  version: 1.0.0
  description: Removes integration data for an object by namespace name.
basePath: /ctfrest/foundation/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /integrationdata/myself/{namespaceid}:
    delete:
      summary: Removes integration data for current user by namespace id
      description: Removes integration data for current user by namespace id.
      operationId: removeMyIntegrationData
      x-api-path-slug: integrationdatamyselfnamespaceid-delete
      parameters:
      - in: query
        name: dataname
        description: Data name
      - in: path
        name: namespaceid
        description: Namespace id
      responses:
        200:
          description: OK
      tags:
      - Removes
      - Integration
      - Datacurrent
      - User
      - By
      - Namespace
    put:
      summary: Sets integration data for current user by namespace id
      description: Sets integration data for current user by namespace id.
      operationId: setMyIntegrationData
      x-api-path-slug: integrationdatamyselfnamespaceid-put
      parameters:
      - in: body
        name: body
        description: Integration data
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: namespaceid
        description: Namespace id
      responses:
        200:
          description: OK
      tags:
      - Sets
      - Integration
      - Datacurrent
      - User
      - By
      - Namespace
    get:
      summary: Gets integration data for current user by namespace id
      description: Gets integration data for current user by namespace id.
      operationId: getMyIntegrationData
      x-api-path-slug: integrationdatamyselfnamespaceid-get
      parameters:
      - in: query
        name: dataname
        description: Data name
      - in: path
        name: namespaceid
        description: Namespace id
      responses:
        200:
          description: OK
      tags:
      - Integration
      - Datacurrent
      - User
      - By
      - Namespace
  /integrationdata/myself/by-name/{namespace}:
    delete:
      summary: Removes integration data for current user by namespace name
      description: Removes integration data for current user by namespace name.
      operationId: removeMyIntegrationDataByName
      x-api-path-slug: integrationdatamyselfbynamenamespace-delete
      parameters:
      - in: query
        name: dataname
        description: Data name
      - in: path
        name: namespace
        description: Namespace name
      responses:
        200:
          description: OK
      tags:
      - Removes
      - Integration
      - Datacurrent
      - User
      - By
      - Namespace
      - Name
    put:
      summary: Sets integration data for current user by namespace name
      description: Sets integration data for current user by namespace name.
      operationId: setMyIntegrationDataByName
      x-api-path-slug: integrationdatamyselfbynamenamespace-put
      parameters:
      - in: body
        name: body
        description: Integration data
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: createNamespace
        description: Create namespace if missing?
      - in: path
        name: namespace
        description: Namespace name
      responses:
        200:
          description: OK
      tags:
      - Sets
      - Integration
      - Datacurrent
      - User
      - By
      - Namespace
      - Name
    get:
      summary: Gets integration data for current user by namespace name
      description: Gets integration data for current user by namespace name.
      operationId: getMyIntegrationDataByName
      x-api-path-slug: integrationdatamyselfbynamenamespace-get
      parameters:
      - in: query
        name: dataname
        description: Data name
      - in: path
        name: namespace
        description: Namespace name
      responses:
        200:
          description: OK
      tags:
      - Integration
      - Datacurrent
      - User
      - By
      - Namespace
      - Name
  /integrationdata/by-objectid/{objectid}/{namespaceid}:
    delete:
      summary: Removes integration data for an object by namespace id
      description: Removes integration data for an object by namespace id.
      operationId: removeIntegrationData
      x-api-path-slug: integrationdatabyobjectidobjectidnamespaceid-delete
      parameters:
      - in: query
        name: dataname
        description: Data name
      - in: path
        name: namespaceid
        description: Namespace id
      - in: path
        name: objectid
        description: Object id
      responses:
        200:
          description: OK
      tags:
      - Removes
      - Integration
      - Dataan
      - Object
      - By
      - Namespace
    put:
      summary: Sets integration data for an object by namespace id
      description: Sets integration data for an object by namespace id.
      operationId: setIntegrationData
      x-api-path-slug: integrationdatabyobjectidobjectidnamespaceid-put
      parameters:
      - in: body
        name: body
        description: Integration data
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: namespaceid
        description: Namespace id
      - in: path
        name: objectid
        description: Object id
      responses:
        200:
          description: OK
      tags:
      - Sets
      - Integration
      - Dataan
      - Object
      - By
      - Namespace
    get:
      summary: Gets integration data for an object by namespace id
      description: Gets integration data for an object by namespace id.
      operationId: getIntegrationData
      x-api-path-slug: integrationdatabyobjectidobjectidnamespaceid-get
      parameters:
      - in: query
        name: dataname
        description: Data name
      - in: path
        name: namespaceid
        description: Namespace id
      - in: path
        name: objectid
        description: Object id
      responses:
        200:
          description: OK
      tags:
      - Integration
      - Dataan
      - Object
      - By
      - Namespace
  /integrationdata/by-objectid/{objectid}/by-name/{namespace}:
    delete:
      summary: Removes integration data for an object by namespace name
      description: Removes integration data for an object by namespace name.
      operationId: removeIntegrationDataByName
      x-api-path-slug: integrationdatabyobjectidobjectidbynamenamespace-delete
      parameters:
      - in: query
        name: dataname
        description: Data name
      - in: path
        name: namespace
        description: Namespace name
      - in: path
        name: objectid
        description: Object id
      responses:
        200:
          description: OK
      tags:
      - Removes
      - Integration
      - Dataan
      - Object
      - By
      - Namespace
      - Name
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