swagger: "2.0"
x-collection-name: Instagram
x-complete: 1
info:
  title: Instagram
  version: 1.0.0
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