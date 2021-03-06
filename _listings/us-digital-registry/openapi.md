swagger: "2.0"
x-collection-name: US Digital Registry
x-complete: 1
info:
  title: U.S. Digital Registry Tag API
  description: provides-a-access-to-the-list-of-tags-applied-to-federal-government-agencies-and-their-social-media-accounts-
  version: 1.0.0
host: usdigitalregistry.digitalgov.gov
basePath: /api/v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /agencies.json:
    get:
      summary: Agencies
      description: This lists all active agencies in the system. These agencies can
        be used to query for social media accounts, mobile products, and galleries.
      operationId: Api::V1::Agencies#index
      x-api-path-slug: agencies-json-get
      parameters:
      - in: query
        name: no_accounts
        description: Including this parameter with value true will cause the endpoint
          to include agencies that have no account in the system
        type: string
        format: string
      - in: query
        name: page
        description: Page number
      - in: query
        name: page_size
        description: Number of results per page
      - in: query
        name: q
        description: String to compare to the name & acronym of the agencies
      responses:
        200:
          description: OK
      tags:
      - Agencies
  /agencies/{id}.json:
    get:
      summary: Agency
      description: This returns an agency based on an ID.
      operationId: Api::V1::Agencies#show
      x-api-path-slug: agenciesid-json-get
      parameters:
      - in: path
        name: id
        description: ID of the agency
      responses:
        200:
          description: OK
      tags:
      - Agencies