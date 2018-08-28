---
swagger: "2.0"
x-collection-name: AWS API Gateway
x-complete: 0
info:
  title: AWS API Gateway API Integration Delete
  version: 1.0.0
  description: Deletes an integration.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /restapis/fugvjdxtri/resources/3kzxbg5sa2/methods/GET/integration/responses/200:
    patch:
      summary: Integrationresponse Update
      description: Changes information about an integration response.
      operationId: integrationresponseUpdate
      x-api-path-slug: restapisfugvjdxtriresources3kzxbg5sa2methodsgetintegrationresponses200-patch
      parameters:
      - in: header
        name: '&quot;op&quot;'
        type: string
      - in: header
        name: '&quot;patchOperations&quot;'
        type: string
      - in: header
        name: '&quot;path&quot;'
        type: string
      - in: header
        name: '&quot;value&quot;'
        type: string
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: body
        name: from
        description: Not supported
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Host
        type: string
      - in: body
        name: op
        description: An update operation to be performed with this PATCH request
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: path
        description: The op operation&#39;s target, as identified by a JSON Pointer
          value that references a location within the targeted resource
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: value
        description: The new target value of the update operation
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Integrations
    delete:
      summary: Integration Delete
      description: Deletes an integration response.
      operationId: integrationresponseDelete
      x-api-path-slug: restapisfugvjdxtriresources3kzxbg5sa2methodsgetintegrationresponses200-delete
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Integrations
    put:
      summary: Integrationresponse Put
      description: Set up an IntegrationResponse for the integration.
      operationId: integrationresponsePut
      x-api-path-slug: restapisfugvjdxtriresources3kzxbg5sa2methodsgetintegrationresponses200-put
      parameters:
      - in: header
        name: '&quot;method.response.header.Content-Type&quot;'
        type: string
      - in: header
        name: '&quot;responseParameters&quot;'
        type: string
      - in: header
        name: '&quot;selectionPattern&quot;'
        type: string
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: body
        name: 'CONVERT_TO_BINARY: Converts a response payload from a Base64-encoded
          string to the corresponding binary blob.'
        description: 'CONVERT_TO_TEXT: Converts a response payload from a binary blob
          to a Base64-encoded string'
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Integrations
    get:
      summary: Integration Responses
      description: Specifies the integration&#39;s responses.
      operationId: integrationResponses
      x-api-path-slug: restapisfugvjdxtriresources3kzxbg5sa2methodsgetintegrationresponses200-get
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Integrations
      - Responses
  /restapis/fugvjdxtri/resources/3kzxbg5sa2/methods/GET/integration:
    patch:
      summary: Integration Update
      description: Changes information about an integration.
      operationId: integrationUpdate
      x-api-path-slug: restapisfugvjdxtriresources3kzxbg5sa2methodsgetintegration-patch
      parameters:
      - in: header
        name: '&quot;op&quot;'
        type: string
      - in: header
        name: '&quot;patchOperations&quot;'
        type: string
      - in: header
        name: '&quot;path&quot;'
        type: string
      - in: header
        name: '&quot;value&quot;'
        type: string
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: body
        name: from
        description: Not supported
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Host
        type: string
      - in: body
        name: op
        description: An update operation to be performed with this PATCH request
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: path
        description: The op operation&#39;s target, as identified by a JSON Pointer
          value that references a location within the targeted resource
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: value
        description: The new target value of the update operation
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Integration
    delete:
      summary: Integration Delete
      description: Deletes an integration.
      operationId: integrationDelete
      x-api-path-slug: restapisfugvjdxtriresources3kzxbg5sa2methodsgetintegration-delete
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Integration
    put:
      summary: Integration Put
      description: Set up the method&#39;s integration request.
      operationId: integrationPut
      x-api-path-slug: restapisfugvjdxtriresources3kzxbg5sa2methodsgetintegration-put
      parameters:
      - in: header
        name: '&quot;application/json&quot;'
        type: string
      - in: header
        name: '&quot;httpMethod&quot;'
        type: string
      - in: header
        name: '&quot;integration.request.header.Content-Type&quot;'
        type: string
      - in: header
        name: '&quot;passthroughBehavior&quot;'
        type: string
      - in: header
        name: '&quot;requestParameters&quot;'
        type: string
      - in: header
        name: '&quot;requestTemplates&quot;'
        type: string
      - in: header
        name: '&quot;type&quot;'
        type: string
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: body
        name: WHEN_NO_MATCH passes the request body for unmapped content types through
          to the integration back end without transformation.
        description: NEVER rejects unmapped content types with an HTTP 415 &#39;Unsupported
          Media Type&#39; response
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Integration
      - Put
  /restapis/uojnr9hd57/resources/0cjtch/methods/GET/integration:
    get:
      summary: Method Integration
      description: Gets the method&#39;s integration responsible for passing the client-submitted
        request to the back end and performing necessary transformations to make the
        request compliant with the back end.
      operationId: methodIntegration
      x-api-path-slug: restapisuojnr9hd57resources0cjtchmethodsgetintegration-get
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Length
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Method
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