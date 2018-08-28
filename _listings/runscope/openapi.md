swagger: "2.0"
x-collection-name: Runscope
x-complete: 1
info:
  title: Runscope
  description: manage-runscope-programmatically-
  version: 1.0.0
host: api.runscope.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /teams/{teamId}/integrations:
    get:
      summary: Get Teams Integrations
      description: Team integrations list
      operationId: teams.teamId.integrations.get
      x-api-path-slug: teamsteamidintegrations-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Teams
      - Integrations