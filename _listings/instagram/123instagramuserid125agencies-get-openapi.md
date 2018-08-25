---
swagger: "2.0"
x-collection-name: Instagram
x-complete: 0
info:
  title: Instagram Instagram User Agencies
  version: 1.0.0
  description: Instagram User Agencies
host: graph.facebook.com
basePath: /v3.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /&#123;instagram-user-id&#125;/agencies:
    get:
      summary: Instagram User Agencies
      description: Instagram User Agencies
      operationId: getInstagramUserAgencies
      x-api-path-slug: 123instagramuserid125agencies-get
      parameters:
      - in: query
        name: "294"
        description: Managing advertisements requires an access token with the extended
          permission for ads_management
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instagram
      - User
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