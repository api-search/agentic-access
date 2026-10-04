---
acting_count: 79
action_class_counts:
  acting: 79
  connected: 53
api_specs:
- filename: flueid-account-api-openapi.yml
  format: yaml
  label: Flueid Account API
  slug: flueid-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-account-api-openapi.yml
- filename: flueid-accountpartner-api-openapi.yml
  format: yaml
  label: Flueid Account Partner API
  slug: flueid-accountpartner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-accountpartner-api-openapi.yml
- filename: flueid-clientcompanies-api-openapi.yml
  format: yaml
  label: Flueid Client Companies API
  slug: flueid-clientcompanies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-clientcompanies-api-openapi.yml
- filename: flueid-documents-api-openapi.yml
  format: yaml
  label: Flueid Documents API
  slug: flueid-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-documents-api-openapi.yml
- filename: flueid-farms-api-openapi.yml
  format: yaml
  label: Flueid Farms API
  slug: flueid-farms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-farms-api-openapi.yml
- filename: flueid-neworders-api-openapi.yml
  format: yaml
  label: Flueid New Orders API
  slug: flueid-neworders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-neworders-api-openapi.yml
- filename: flueid-orderdocumentsettings-api-openapi.yml
  format: yaml
  label: Flueid Order Document Settings API
  slug: flueid-orderdocumentsettings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-orderdocumentsettings-api-openapi.yml
- filename: flueid-orderoptions-api-openapi.yml
  format: yaml
  label: Flueid Order Options API
  slug: flueid-orderoptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-orderoptions-api-openapi.yml
- filename: flueid-orders-api-openapi.yml
  format: yaml
  label: Flueid Orders API
  slug: flueid-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-orders-api-openapi.yml
- filename: flueid-partnerordersettings-api-openapi.yml
  format: yaml
  label: Flueid Partner Order Settings API
  slug: flueid-partnerordersettings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-partnerordersettings-api-openapi.yml
- filename: flueid-partners-api-openapi.yml
  format: yaml
  label: Flueid Partners API
  slug: flueid-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-partners-api-openapi.yml
- filename: flueid-permissions-api-openapi.yml
  format: yaml
  label: Flueid Permissions API
  slug: flueid-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-permissions-api-openapi.yml
- filename: flueid-public-api-openapi.yml
  format: yaml
  label: Flueid Public API
  slug: flueid-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-public-api-openapi.yml
- filename: flueid-settings-api-openapi.yml
  format: yaml
  label: Flueid Settings API
  slug: flueid-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-settings-api-openapi.yml
- filename: flueid-order-events-api-openapi.yml
  format: yaml
  label: Flueid Order Events API
  slug: flueid-order-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-order-events-api-openapi.yml
- filename: flueid-property-data-api-openapi.yml
  format: yaml
  label: Flueid Property Data API
  slug: flueid-property-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/openapi/flueid-property-data-api-openapi.yml
consequence_counts:
  physical: 33
  read: 53
  safety-critical: 1
  write: 45
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Flueid Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/Account/ResetPassword
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/Account/ResendTempPassword
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/Account/SendUsersToDataWarehouse
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/NewOrders/CalculateCloseDate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/NewOrders/CheckDuplicateOrder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/NewOrders/CompanyAccountManagers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/NewOrders/CreateOrder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/NewOrders/DefaultOrderContacts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/NewOrders/OrderContactOptions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/NewOrders/OrderDetailsOptions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/NewOrders/OrderTypeOptions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/NewOrders/RelatedOfficers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/OrderDocumentSettings/DeleteOrderDocument
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/OrderDocumentSettings/DeleteOrderDocumentTypeSetting
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/OrderDocumentSettings/GetOrderDocumentList
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/OrderDocumentSettings/SaveOrderDocument
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/OrderDocumentSettings/SaveOrderDocumentTypeSetting
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/OrderEvents/PostDocument
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/OrderOptions/SaveEntityLookupCodes
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/Orders/DecisionReplaceBuyers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/Orders/DownloadTrailingDocument
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/Orders/GetDocument
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/Orders/ModifyDecisionOrderData
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/Orders/RunDateDownUpdate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/Orders/RunFullUpdate
operation_count: 132
overview: 'Flueid exposes 132 API operations that an AI agent could call, of which 79 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 53 read, 45 write, 33 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Flueid
provider_slug: flueid
slug: flueid-agentic-access
source_filename: flueid-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/flueid-account-api-openapi.yml, openapi/flueid-accountpartner-api-openapi.yml,\n  openapi/flueid-clientcompanies-api-openapi.yml, openapi/flueid-documents-api-openapi.yml,\n  openapi/flueid-farms-api-openapi.yml, openapi/flueid-neworders-api-openapi.yml, openapi/flueid-order-events-api-openapi.yml,\n  openapi/flueid-orderdocumentsettings-api-openapi.yml, openapi/flueid-orderoptions-api-openapi.yml,\n  openapi/flueid-orders-api-openapi.yml, openapi/flueid-partnerordersettings-api-openapi.yml,\n  openapi/flueid-partners-api-openapi.yml, openapi/flueid-permissions-api-openapi.yml, openapi/flueid-property-data-api-openapi.yml,\n  openapi/flueid-public-api-openapi.yml, openapi/flueid-settings-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment.\
  \ See research/curity/agentic-governance/.\nsummary:\n  operations: 132\n  by_action_class:\n    acting: 79\n    connected: 53\n  by_consequence:\n    write: 45\n    read: 53\n    physical: 33\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /api/Account/SearchUsers\n  method: post\n  operationId: postApiAccountSearchUsers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Account/ValidateUser\n  method: get\n  operationId: getApiAccountValidateUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Account/PartnerUserRoles\n  method: get\n  operationId: getApiAccountPartnerUserRoles\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Account/RealEstateUserRoles\n  method: get\n  operationId: getApiAccountRealEstateUserRoles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Account/FinanceUserRoles\n  method: get\n  operationId: getApiAccountFinanceUserRoles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Account/SearchOfficersOrAccountExecs\n  method: post\n  operationId: postApiAccountSearchOfficersOrAccountExecs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /api/Account/PullUpCardContent\n  method: get\n  operationId: getApiAccountPullUpCardContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Account/UserSettings\n  method: get\n  operationId: getApiAccountUserSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Account/GetUserProfile\n  method: get\n  operationId: getApiAccountGetUserProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Account/GetUserProfileById\n  method: get\n  operationId: getApiAccountGetUserProfileById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Account/UpdateUserBasicProfile\n\
  \  method: post\n  operationId: postApiAccountUpdateUserBasicProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Account/UpdateUserCompanySettings\n  method: post\n  operationId: postApiAccountUpdateUserCompanySettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Account/UpdateUserPhoto\n  method: post\n  operationId: postApiAccountUpdateUserPhoto\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Account/UpdateUserCompanyLogo\n  method: post\n  operationId: postApiAccountUpdateUserCompanyLogo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Account/UpdateTermsAcceptance\n  method: get\n  operationId: getApiAccountUpdateTermsAcceptance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Account/UpdatePartnerAssociation\n  method: post\n  operationId: postApiAccountUpdatePartnerAssociation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Account/SearchAssistantUsers\n  method: get\n  operationId: getApiAccountSearchAssistantUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Account/UpdateUserAssistants\n  method: post\n  operationId: postApiAccountUpdateUserAssistants\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Account/SendUsersToDataWarehouse\n  method: post\n  operationId: postApiAccountSendUsersToDataWarehouse\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Account/SignUpUser\n  method: post\n  operationId: postApiAccountSignUpUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Account/ApproveUser\n  method: post\n  operationId: postApiAccountApproveUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Account/UpdateUserStatus\n\
  \  method: post\n  operationId: postApiAccountUpdateUserStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Account/ResendTempPassword\n  method: post\n  operationId: postApiAccountResendTempPassword\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Account/ResetPassword\n  method: post\n  operationId: postApiAccountResetPassword\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/AccountPartner/GetActivePartners\n  method: get\n  operationId: getApiAccountPartnerGetActivePartners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/AccountPartner/SetCurrentPartner\n  method: post\n  operationId: postApiAccountPartnerSetCurrentPartner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/ClientCompanies/ClientCompanyDivisions\n  method: get\n  operationId: getApiClientCompaniesClientCompanyDivisions\n  x-agentic-access:\n  \
  \  action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ClientCompanies/AllClientCompanies\n  method: get\n  operationId: getApiClientCompaniesAllClientCompanies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ClientCompanies/SearchClientCompanies\n  method: post\n  operationId: postApiClientCompaniesSearchClientCompanies\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/ClientCompanies/ClientCompany\n  method: get\n  operationId: getApiClientCompaniesClientCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ClientCompanies/SaveClientCompany\n  method: post\n  operationId: postApiClientCompaniesSaveClientCompany\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Documents/GetHyperLinkedDocuments\n  method: get\n  operationId: getApiDocumentsGetHyperLinkedDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Farms/SearchFarmGeoPoints\n  method: post\n  operationId: postApiFarmsSearchFarmGeoPoints\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Farms/SearchFarmProps\n  method: post\n  operationId: postApiFarmsSearchFarmProps\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Farms/FarmOverview\n  method: post\n  operationId: postApiFarmsFarmOverview\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Farms/SaveFarm\n  method: post\n  operationId: postApiFarmsSaveFarm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Farms/GetFarm\n  method: get\n  operationId: getApiFarmsGetFarm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Farms/GetAllFarms\n  method: get\n  operationId: getApiFarmsGetAllFarms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Farms/SaveFarmProperty\n  method: post\n  operationId: postApiFarmsSaveFarmProperty\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /api/Farms/RenameFarm\n  method: post\n  operationId: postApiFarmsRenameFarm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Farms/DeleteFarm\n  method: post\n  operationId: postApiFarmsDeleteFarm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Farms/FarmFilters\n  method: get\n  operationId: getApiFarmsFarmFilters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Farms/SaveFarmFilter\n\
  \  method: post\n  operationId: postApiFarmsSaveFarmFilter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Farms/DeleteFarmFilter\n  method: post\n  operationId: postApiFarmsDeleteFarmFilter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Farms/FarmReport\n  method: get\n  operationId: getApiFarmsFarmReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Farms/UploadExcelFarm\n  method: post\n  operationId:\
  \ postApiFarmsUploadExcelFarm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Farms/FixNotFoundPropertyForFarm\n  method: post\n  operationId: postApiFarmsFixNotFoundPropertyForFarm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Farms/AddPropertyToFarm\n  method: post\n  operationId: postApiFarmsAddPropertyToFarm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Farms/DeletePropertyFromFarm\n  method: post\n  operationId: postApiFarmsDeletePropertyFromFarm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Farms/MarkFarmUploadViewed\n  method: post\n  operationId: postApiFarmsMarkFarmUploadViewed\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/NewOrders/CreateOrder\n  method: post\n  operationId: postApiNewOrdersCreateOrder\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/NewOrders/RetrieveOrderSubmission\n  method: get\n  operationId: getApiNewOrdersRetrieveOrderSubmission\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/NewOrders/CheckDuplicateOrder\n  method: post\n  operationId: postApiNewOrdersCheckDuplicateOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/NewOrders/SearchRelatedBizSrcUsers\n\
  \  method: get\n  operationId: getApiNewOrdersSearchRelatedBizSrcUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/NewOrders/SearchOrderContact\n  method: get\n  operationId: getApiNewOrdersSearchOrderContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/NewOrders/DefaultOrderContacts\n  method: post\n  operationId: postApiNewOrdersDefaultOrderContacts\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/NewOrders/BusinessSourceRoles\n  method: get\n  operationId: getApiNewOrdersBusinessSourceRoles\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/NewOrders/RelatedAssistants\n  method: get\n  operationId: getApiNewOrdersRelatedAssistants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/NewOrders/RelatedOfficers\n  method: post\n  operationId: postApiNewOrdersRelatedOfficers\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/NewOrders/CompanyAccountManagers\n  method: post\n  operationId: postApiNewOrdersCompanyAccountManagers\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/NewOrders/OrderTypeOptions\n  method: post\n  operationId: postApiNewOrdersOrderTypeOptions\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/NewOrders/OrderContactOptions\n  method: post\n  operationId: postApiNewOrdersOrderContactOptions\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/NewOrders/OrderDetailsOptions\n  method: post\n  operationId: postApiNewOrdersOrderDetailsOptions\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/NewOrders/CalculateCloseDate\n  method: post\n  operationId: postApiNewOrdersCalculateCloseDate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /api/NewOrders/CompanyTitleOfficers\n  method: post\n  operationId: postApiNewOrdersCompanyTitleOfficers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/OrderEvents/OrderHistory\n  method: get\n  operationId: getApiOrderEventsOrderHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/OrderEvents/PostDocument\n  method: post\n  operationId: postApiOrderEventsPostDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /api/OrderDocumentSettings/GetOrderDocumentList\n  method: post\n  operationId: postApiOrderDocumentSettingsGetOrderDocumentList\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/OrderDocumentSettings/SaveOrderDocument\n  method: post\n  operationId: postApiOrderDocumentSettingsSaveOrderDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/OrderDocumentSettings/DeleteOrderDocument\n  method: post\n\
  \  operationId: postApiOrderDocumentSettingsDeleteOrderDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/OrderDocumentSettings/SaveOrderDocumentTypeSetting\n  method: post\n  operationId: postApiOrderDocumentSettingsSaveOrderDocumentTypeSetting\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/OrderDocumentSettings/DeleteOrderDocumentTypeSetting\n  method: post\n  operationId: postApiOrderDocumentSettingsDeleteOrderDocumentTypeSetting\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/OrderOptions/GetAllLookupCodesForCompany\n  method: get\n  operationId: getApiOrderOptionsGetAllLookupCodesForCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/OrderOptions/SaveEntityLookupCodes\n  method: post\n  operationId: postApiOrderOptionsSaveEntityLookupCodes\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/Orders/SearchOrders\n  method: post\n  operationId: postApiOrdersSearchOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Orders/OrderDetail\n  method: get\n  operationId: getApiOrdersOrderDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Orders/RunFullUpdate\n  method: post\n  operationId: postApiOrdersRunFullUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Orders/RunDateDownUpdate\n  method: post\n  operationId: postApiOrdersRunDateDownUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Orders/GetDocument\n  method: post\n  operationId: postApiOrdersGetDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /api/Orders/UpdateOrderStatus\n  method: post\n  operationId: postApiOrdersUpdateOrderStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Orders/GetDecisionOrderData\n  method: get\n  operationId: getApiOrdersGetDecisionOrderData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Orders/ModifyDecisionOrderData\n  method: post\n  operationId: postApiOrdersModifyDecisionOrderData\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Orders/DecisionReplaceBuyers\n  method: post\n  operationId: postApiOrdersDecisionReplaceBuyers\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/Orders/DownloadTrailingDocument\n  method: post\n  operationId: postApiOrdersDownloadTrailingDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/PartnerOrderSettings/PartnerOrderSettings\n  method: get\n  operationId: getApiPartnerOrderSettingsPartnerOrderSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/PartnerOrderSettings/SetPartnerOrderSettings\n  method: post\n  operationId: postApiPartnerOrderSettingsSetPartnerOrderSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/PartnerOrderSettings/TxmSettings\n  method: get\n  operationId: getApiPartnerOrderSettingsTxmSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api/PartnerOrderSettings/SetTxmSettings\n  method: post\n  operationId: postApiPartnerOrderSettingsSetTxmSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/PartnerOrderSettings/DecisionSettings\n  method: get\n  operationId: getApiPartnerOrderSettingsDecisionSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/PartnerOrderSettings/SetDecisionSettings\n  method: post\n  operationId: postApiPartnerOrderSettingsSetDecisionSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n  \
  \  token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/PartnerOrderSettings/D4aSettings\n  method: get\n  operationId: getApiPartnerOrderSettingsD4aSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\n\n# --- truncated at 32 KB (44 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/agentic-access/flueid-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flueid/refs/heads/main/agentic-access/flueid-agentic-access.yml
summary_line: 132 operations · 79 acting · 1 human-in-the-loop
tags:
- Company
- Real Estate
- Title Insurance
- Mortgage
- Property Data
- Verification of Title
- Financial Services
- Lending
- PropTech
- Settlement Services
---
