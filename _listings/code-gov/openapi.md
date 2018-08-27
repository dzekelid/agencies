swagger: "2.0"
x-collection-name: Code.gov
x-complete: 1
info:
  title: Code.gov API
  description: code-gov-api-documentation--while-using-this-documentation-locally-please-choose-to-
  version: 1.0.0
host: api.code.gov
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /agencies:
    get:
      summary: Get a list of agencies
      description: Get a list of agencies.
      operationId: getAgencies
      x-api-path-slug: agencies-get
      parameters:
      - in: query
        name: from
        description: Specify an offset to return
      - in: query
        name: size
        description: Number of agencies to return
      responses:
        200:
          description: OK
      tags:
      - Agencies