---
swagger: "2.0"
info:
  title: U.S. Digital Registry Agency API
  description: Provides access to a list of federal agencies.
  version: "1.0"
host: usdigitalregistry.digitalgov.gov
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /agencies/{id}.json:
    get:
      summary: Agency
      description: This returns an agency based on an ID
      operationId: Api::V1::Agencies#show
      parameters:
      - in: path
        name: id
        description: ID of the agency
      responses:
        200:
          description: OK
      tags:
      - agencies
definitions:
  metadata:
    properties:
      results:
        description: The results.
        type: array
  results:
    properties: []
  agency:
    properties: []
x-collection-name: U.S. Digital Registry
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