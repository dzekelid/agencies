---
swagger: "2.0"
x-collection-name: Code.gov
x-complete: 0
info:
  title: Code.gov Get a list of agencies
  description: Get a list of agencies.
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