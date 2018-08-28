---
swagger: "2.0"
x-collection-name: moltin
x-complete: 0
info:
  title: Moltin API Get all Jobs for an Integration
  description: Get all jobs for an integration.
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
  /v2/integrations:
    get:
      summary: Get Integrations list
      description: Get integrations list.
      operationId: V2IntegrationsGet
      x-api-path-slug: v2integrations-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Integrations
      - List
    post:
      summary: Create an Integration
      description: Create an integration.
      operationId: V2IntegrationsPost
      x-api-path-slug: v2integrations-post
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
      - Integration
  /v2/integrations/{integrationID}:
    get:
      summary: Get an Integration
      description: Get an integration.
      operationId: V2IntegrationsByIntegrationIDGet
      x-api-path-slug: v2integrationsintegrationid-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: integrationID
      responses:
        200:
          description: Successful response
      tags:
      - Integration
    put:
      summary: Update an Integration
      description: Update an integration.
      operationId: V2IntegrationsByIntegrationIDPut
      x-api-path-slug: v2integrationsintegrationid-put
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
        name: integrationID
      responses:
        200:
          description: Successful response
      tags:
      - Integration
    delete:
      summary: Delete an Integration
      description: Delete an integration.
      operationId: V2IntegrationsByIntegrationIDDelete
      x-api-path-slug: v2integrationsintegrationid-delete
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: integrationID
      responses:
        200:
          description: Successful response
      tags:
      - Integration
  /v2/integrations/attributes:
    get:
      summary: Get Integration Attributes
      description: Get integration attributes.
      operationId: V2IntegrationsAttributesGet
      x-api-path-slug: v2integrationsattributes-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Integration
      - Attributes
  /v2/integrations/{integrationID}/logs:
    get:
      summary: Get Logs for an Integration
      description: Get logs for an integration.
      operationId: V2IntegrationsLogsByIntegrationIDGet
      x-api-path-slug: v2integrationsintegrationidlogs-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: integrationID
      responses:
        200:
          description: Successful response
      tags:
      - Logsan
      - Integration
  /v2/integrations/{integrationID}/jobs:
    get:
      summary: Get all Jobs for an Integration
      description: Get all jobs for an integration.
      operationId: V2IntegrationsJobsByIntegrationIDGet
      x-api-path-slug: v2integrationsintegrationidjobs-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: integrationID
      responses:
        200:
          description: Successful response
      tags:
      - Jobsan
      - Integration
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