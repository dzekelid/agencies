---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Saves or updates the envelope template for an agency
  version: 1.0.0
  description: Saves or updates the envelope template for an agency.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/admin/system/ListAgencies:
    get:
      summary: Lists the name and ID of all agencies in the system.
      description: Lists the name and id of all agencies in the system..
      operationId: System_ListAgenciesByincludeSuspended
      x-api-path-slug: apiadminsystemlistagencies-get
      parameters:
      - in: query
        name: includeSuspended
        description: if set to true [include suspended]
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Name
      - ID
      - Of
      - ""
      - Agencies
      - In
      - System
  /api/agency/branches:
    get:
      summary: Get the branches for an agency
      description: Get the branches for an agency.
      operationId: Agency_Branches
      x-api-path-slug: apiagencybranches-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Branchesan
      - Agency
  /api/agency/milestoneconfigurations:
    get:
      summary: Get the milestone configurations for an agency
      description: Get the milestone configurations for an agency.
      operationId: Agency_MilestoneConfigurations
      x-api-path-slug: apiagencymilestoneconfigurations-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Milestone
      - Configurationsan
      - Agency
  /api/agency/administrators:
    get:
      summary: Get the administrators for an agency
      description: Get the administrators for an agency.
      operationId: Agency_Administrators
      x-api-path-slug: apiagencyadministrators-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Administratorsan
      - Agency
  /api/agency/accountmanager:
    get:
      summary: Get the account manager for an agency
      description: Get the account manager for an agency.
      operationId: Agency_AccountManager
      x-api-path-slug: apiagencyaccountmanager-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Account
      - Manageran
      - Agency
  /api/agency/meetingplaces:
    get:
      summary: Get meeting places for an agency
      description: Get meeting places for an agency.
      operationId: Agency_MeetingPlaces
      x-api-path-slug: apiagencymeetingplaces-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Meeting
      - Placesan
      - Agency
  /api/agency/savemeetingplace:
    post:
      summary: Saves a new meeting place to that particular agency
      description: Saves a new meeting place to that particular agency.
      operationId: Agency_SaveMeetingPlaceBydataContract
      x-api-path-slug: apiagencysavemeetingplace-post
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Saves
      - New
      - Meeting
      - Place
      - To
      - That
      - Particular
      - Agency
  /api/agency/fees:
    get:
      summary: Get fees for logged in agency
      description: Get fees for logged in agency.
      operationId: Agency_FeesBytransactionTypeBydefaultOnly
      x-api-path-slug: apiagencyfees-get
      parameters:
      - in: query
        name: defaultOnly
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: transactionType
        description: The transaction type of the fee to retrieve
      responses:
        200:
          description: OK
      tags:
      - Feeslogged
      - In
      - Agency
  /api/agency/updatefee:
    put:
      summary: Add or update fee for logged in agency.
      description: Add or update fee for logged in agency..
      operationId: Agency_UpdateAgencyFeeByfeeDataContract
      x-api-path-slug: apiagencyupdatefee-put
      parameters:
      - in: body
        name: feeDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Update
      - Feelogged
      - In
      - Agency
  /api/agency/deletefee/{defaultFeeId}:
    delete:
      summary: Delete fee for logged in agency.
      description: Delete fee for logged in agency..
      operationId: Agency_DeleteAgencyFeeBydefaultFeeId
      x-api-path-slug: apiagencydeletefeedefaultfeeid-delete
      parameters:
      - in: path
        name: defaultFeeId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Feelogged
      - In
      - Agency
  /api/agency/teams:
    get:
      summary: Returns a list of team groups for the agency.
      description: Returns a list of team groups for the agency..
      operationId: Agency_TeamsBypageSizeBypageNumberByteamType
      x-api-path-slug: apiagencyteams-get
      parameters:
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: teamType
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Team
      - Groupsthe
      - Agency
  /api/agency/feestructure:
    get:
      summary: Gets the fee structure of the agency
      description: Gets the fee structure of the agency.
      operationId: Agency_GetFeeStructure
      x-api-path-slug: apiagencyfeestructure-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Fee
      - Structure
      - Of
      - Agency
  /api/agency/{id}/getbrand:
    get:
      summary: Get a specific brand by brandId or default agency brand if brandId
        is not supplied.
      description: Get a specific brand by brandid or default agency brand if brandid
        is not supplied..
      operationId: Agency_GetAgencyBrandByidBybrandId
      x-api-path-slug: apiagencyidgetbrand-get
      parameters:
      - in: query
        name: brandId
        description: The id of brand to get
      - in: path
        name: id
        description: The id of an agency
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Specific
      - Brand
      - By
      - BrandId
      - Default
      - Agency
      - Brand
      - If
      - BrandId
      - Is
      - Not
      - Supplied
  /api/agency/tenantclause:
    get:
      summary: Get meeting places for an agency
      description: Get meeting places for an agency.
      operationId: Agency_TenantClause
      x-api-path-slug: apiagencytenantclause-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Meeting
      - Placesan
      - Agency
  /api/Agency:
    get:
      summary: Get details of the current users agency
      description: Get details of the current users agency.
      operationId: Agency_Get
      x-api-path-slug: apiagency-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Details
      - Of
      - Current
      - Users
      - Agency
  /api/admin/agency/{id}/setfeestructure:
    post:
      summary: Sets the fee structure on an agency
      description: Sets the fee structure on an agency.
      operationId: AgencyAdmin_SetFeeStructureByidByfeeStructure
      x-api-path-slug: apiadminagencyidsetfeestructure-post
      parameters:
      - in: body
        name: feeStructure
        description: The fee structure text
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The agency id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Sets
      - Fee
      - Structure
      - "On"
      - Agency
  /api/analytics/campaigns:
    get:
      summary: returns a list of all of the campaigns for an agency
      description: Returns a list of all of the campaigns for an agency.
      operationId: Analytics_GetCampaigns
      x-api-path-slug: apianalyticscampaigns-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - ""
      - Of
      - Campaignsan
      - Agency
  /api/branding/getallbrands:
    get:
      summary: Get all brands with details for an agency
      description: Get all brands with details for an agency.
      operationId: Branding_GetAllBrandsForAgency
      x-api-path-slug: apibrandinggetallbrands-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Brands
      - Detailsan
      - Agency
  /api/Branding:
    get:
      summary: Gets a sumary all of the brands for a agency
      description: Gets a sumary all of the brands for a agency.
      operationId: Branding_Get
      x-api-path-slug: apibranding-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Sumary
      - ""
      - Of
      - Brandsa
      - Agency
  /api/documentgeneration/saveenvelopetemplate:
    post:
      summary: Saves or updates the envelope template for an agency
      description: Saves or updates the envelope template for an agency.
      operationId: DocumentGeneration_SaveEnvelopeTemplateByenvelopeTemplate
      x-api-path-slug: apidocumentgenerationsaveenvelopetemplate-post
      parameters:
      - in: body
        name: envelopeTemplate
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Saves
      - Updates
      - Envelope
      - Templatean
      - Agency
  /api/documentgeneration/saveenvelopetemplatepack:
    post:
      summary: Saves or updates envelope template correspondence for a an agency
      description: Saves or updates envelope template correspondence for a an agency.
      operationId: DocumentGeneration_SaveEnvelopeTemplatePackByenvelopeTemplatePack
      x-api-path-slug: apidocumentgenerationsaveenvelopetemplatepack-post
      parameters:
      - in: body
        name: envelopeTemplatePack
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Saves
      - Updates
      - Envelope
      - Template
      - Correspondencea
      - Agency
  /api/documentgeneration/lettertemplate/{letterTemplateId}:
    get:
      summary: Returns a list of lettertemplates associated to this agency
      description: Returns a list of lettertemplates associated to this agency.
      operationId: DocumentGeneration_GetLetterTemplateByletterTemplateId
      x-api-path-slug: apidocumentgenerationlettertemplatelettertemplateid-get
      parameters:
      - in: path
        name: letterTemplateId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Lettertemplates
      - Associated
      - To
      - This
      - Agency
  /api/documentgeneration/mergetemplates:
    get:
      summary: Returns a list of lettertemplates associated to this agency
      description: Returns a list of lettertemplates associated to this agency.
      operationId: DocumentGeneration_GetPrintableMergeTemplates
      x-api-path-slug: apidocumentgenerationmergetemplates-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Lettertemplates
      - Associated
      - To
      - This
      - Agency
  /api/documentgeneration/unusedmergetemplates:
    get:
      summary: Returns a list of lettertemplates associated to this agency that are
        not currently used in any envelope templates
      description: Returns a list of lettertemplates associated to this agency that
        are not currently used in any envelope templates.
      operationId: DocumentGeneration_GetUnusedMergeTemplates
      x-api-path-slug: apidocumentgenerationunusedmergetemplates-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Lettertemplates
      - Associated
      - To
      - This
      - Agency
      - That
      - Are
      - Not
      - Currently
      - Used
      - In
      - Any
      - Envelope
      - Templates
  /api/documentgeneration/templatesusinganalytics/{analyticsId}:
    get:
      summary: Returns a list of lettertemplates associated to this agency and to
        a particular google analyitics campaign
      description: Returns a list of lettertemplates associated to this agency and
        to a particular google analyitics campaign.
      operationId: DocumentGeneration_GetTemplatesUsingAnalyticsByanalyticsId
      x-api-path-slug: apidocumentgenerationtemplatesusinganalyticsanalyticsid-get
      parameters:
      - in: path
        name: analyticsId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Lettertemplates
      - Associated
      - To
      - This
      - Agency
      - To
      - Particular
      - Google
      - Analyitics
      - Campaign
  /api/documentgeneration/insertabletemplates:
    get:
      summary: Returns a list of insertable templates associated to this agency
      description: Returns a list of insertable templates associated to this agency.
      operationId: DocumentGeneration_GetPrintableInsertableTemplates
      x-api-path-slug: apidocumentgenerationinsertabletemplates-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Insertable
      - Templates
      - Associated
      - To
      - This
      - Agency
  /api/documentgeneration/headertemplates:
    get:
      summary: Returns a list of header templates associated to this agency with their
        associated brand info
      description: Returns a list of header templates associated to this agency with
        their associated brand info.
      operationId: DocumentGeneration_GetPrintableHeaderTemplates
      x-api-path-slug: apidocumentgenerationheadertemplates-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Header
      - Templates
      - Associated
      - To
      - This
      - Agency
      - Their
      - Associated
      - Brand
      - Info
  /api/documentgeneration/envelopetemplates:
    get:
      summary: Returns a list of envelope templates associated to this agency
      description: Returns a list of envelope templates associated to this agency.
      operationId: DocumentGeneration_GetEnvelopeTemplates
      x-api-path-slug: apidocumentgenerationenvelopetemplates-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Envelope
      - Templates
      - Associated
      - To
      - This
      - Agency
  /api/documentgeneration/envelopetemplatepacks:
    get:
      summary: Returns a list of envelope template packs associated to this agency
      description: Returns a list of envelope template packs associated to this agency.
      operationId: DocumentGeneration_GetEnvelopeTemplatePacks
      x-api-path-slug: apidocumentgenerationenvelopetemplatepacks-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Envelope
      - Template
      - Packs
      - Associated
      - To
      - This
      - Agency
  /api/documentgeneration/envelopetemplatepacktypes:
    get:
      summary: Returns a list of envelope template packs associated to this agency
      description: Returns a list of envelope template packs associated to this agency.
      operationId: DocumentGeneration_GetEnvelopeTemplatePackTypesByinUseOnly
      x-api-path-slug: apidocumentgenerationenvelopetemplatepacktypes-get
      parameters:
      - in: query
        name: inUseOnly
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Envelope
      - Template
      - Packs
      - Associated
      - To
      - This
      - Agency
  /api/documentgeneration/emailtemplates:
    get:
      summary: Returns a list of email templates associated to this agency
      description: Returns a list of email templates associated to this agency.
      operationId: DocumentGeneration_GetEmailTemplates
      x-api-path-slug: apidocumentgenerationemailtemplates-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Email
      - Templates
      - Associated
      - To
      - This
      - Agency
  /api/documentgeneration/templates/{templateType}:
    get:
      summary: Returns a list of mergable templates for any type associated to this
        agency
      description: Returns a list of mergable templates for any type associated to
        this agency.
      operationId: DocumentGeneration_GetTemplatesBytemplateType
      x-api-path-slug: apidocumentgenerationtemplatestemplatetype-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: templateType
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Mergable
      - Templatesany
      - Type
      - Associated
      - To
      - This
      - Agency
  /api/documentgeneration/smstemplates:
    get:
      summary: Returns a list of sms templates associated to this agency
      description: Returns a list of sms templates associated to this agency.
      operationId: DocumentGeneration_GetSmsTemplates
      x-api-path-slug: apidocumentgenerationsmstemplates-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Sms
      - Templates
      - Associated
      - To
      - This
      - Agency
  /api/enlistedfeature/getvalidforagency:
    get:
      summary: Gets all the active features for an agency
      description: Gets all the active features for an agency.
      operationId: EnlistedFeature_GetAllValidEnlistedFeaturesForAgency
      x-api-path-slug: apienlistedfeaturegetvalidforagency-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - ""
      - Active
      - Featuresan
      - Agency
  /api/featureprovisioning/enrollagency:
    post:
      summary: Enrolls an agency into a feature
      description: Enrolls an agency into a feature.
      operationId: FeatureProvisioning_EnrollAgencyInFeatureByfeatureSystemName
      x-api-path-slug: apifeatureprovisioningenrollagency-post
      parameters:
      - in: query
        name: featureSystemName
        description: The SystemName of the feature
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Enrolls
      - Agency
      - Into
      - Feature
  /api/progression/lettings/{id}/resetmilestones:
    post:
      summary: Reset tenant role milestones back to agency defaults
      description: Reset tenant role milestones back to agency defaults.
      operationId: LettingsProgression_ResetRoleMilestonesToDefaultByid
      x-api-path-slug: apiprogressionlettingsidresetmilestones-post
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Reset
      - Tenant
      - Role
      - Milestones
      - Back
      - To
      - Agency
      - Defaults
  /api/progression/lettings/resetdefaultmilestones:
    post:
      summary: Reset agency default milestones back to global defaults
      description: Reset agency default milestones back to global defaults.
      operationId: LettingsProgression_ResetMilestonesToDefault
      x-api-path-slug: apiprogressionlettingsresetdefaultmilestones-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Reset
      - Agency
      - Default
      - Milestones
      - Back
      - To
      - Global
      - Defaults
  /api/role/{id}/getbrandportalexclusions:
    get:
      summary: Get all brands with details for an agency
      description: Get all brands with details for an agency.
      operationId: Role_GetBrandPortalExclusionsByid
      x-api-path-slug: apiroleidgetbrandportalexclusions-get
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Brands
      - Detailsan
      - Agency
  /api/role/{id}/savebrandportalexclusions:
    post:
      summary: Get all brands with details for an agency
      description: Get all brands with details for an agency.
      operationId: Role_SaveBrandPortalExclusionsByidBybrandsToSave
      x-api-path-slug: apiroleidsavebrandportalexclusions-post
      parameters:
      - in: body
        name: brandsToSave
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Brands
      - Detailsan
      - Agency
  /api/admin/system/sendNotificationToAllUsersInAgency:
    post:
      summary: Send a live notification to all active users in an agency
      description: Send a live notification to all active users in an agency.
      operationId: System_SendNotificationToAgencyUsersByagencyIdBysendNotification
      x-api-path-slug: apiadminsystemsendnotificationtoallusersinagency-post
      parameters:
      - in: query
        name: agencyId
        description: The agency identifier
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: sendNotification
        description: The send notification
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Send
      - Live
      - Notification
      - To
      - ""
      - Active
      - Users
      - In
      - Agency
  /api/negotiator/getarchived:
    get:
      summary: Get all archived Negotiators for the Agency's branch.
      description: Get all archived negotiators for the agency's branch..
      operationId: Negotiator_GetArchivedByteamIdBypageSizeBypageNumber
      x-api-path-slug: apinegotiatorgetarchived-get
      parameters:
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: teamId
        description: (optional) teamId to get negotiators for
      responses:
        200:
          description: OK
      tags:
      - Archived
      - Negotiatorsthe
      - Agencys
      - Branch
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