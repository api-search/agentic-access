---
acting_count: 160
action_class_counts:
  acting: 160
  connected: 124
api_specs:
- filename: loadsmart-shipperguide-openapi.yml
  format: yaml
  label: Loadsmart ShipperGuide API
  slug: loadsmart-shipperguide-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loadsmart/refs/heads/main/openapi/loadsmart-shipperguide-openapi.yml
- filename: loadsmart-opendock-openapi.yml
  format: yaml
  label: Opendock Nova (Neutron) API
  slug: loadsmart-opendock-nova-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loadsmart/refs/heads/main/openapi/loadsmart-opendock-openapi.yml
consequence_counts:
  physical: 14
  read: 124
  safety-critical: 122
  write: 24
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 122
kind: agentic-access
layout: agentic-access
method: generated
name: Loadsmart Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/v2/shipments/{shipment_id}/stops/{stop_id}/confirm_appointment
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /appointment
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /appointment/reserve
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /appointment/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /appointment/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /appointment/{id}/recurring
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /appointment/{id}/recurring
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /appointment/{id}/set-eta
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /appointment/{id}/tag
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /appointment/{id}/tag
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /appointment/{id}/undo-latest-status
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /asset-container
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /asset-container/event
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /asset-container/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /asset-container/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /asset-visit
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /asset-visit/event
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /asset-visit/link-unplanned-checkin-to-appointment
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /asset-visit/unlink-checkin-from-appointment
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /asset-visit/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /asset-visit/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /asset-visit/{id}/attach/{assetContainerId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /asset-visit/{id}/check-in-acknowledgment
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /asset-visit/{id}/detach/{assetContainerId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /auth/login
operation_count: 284
overview: 'Loadsmart exposes 284 API operations that an AI agent could call, of which 160 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 124 read, 24 write, 14 physical, and 122 safety-critical.


  122 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Loadsmart
provider_slug: loadsmart
slug: loadsmart-agentic-access
source_filename: loadsmart-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/loadsmart-opendock-openapi.yml, openapi/loadsmart-shipperguide-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 284\n  by_action_class:\n    connected: 124\n    acting: 160\n  by_consequence:\n    read: 124\n    safety-critical: 122\n    write: 24\n    physical: 14\n  human_in_the_loop_required: 122\noperations:\n- path: /\n  method: get\n  operationId: AppController_getBase\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /version\n  method: get\n  operationId: AppController_getVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app-environment\n  method: get\n  operationId: AppController_getAppEnvironment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /warehouse/{id}\n  method: get\n  operationId: getOneBaseWarehouseControllerWarehouse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /warehouse/{id}\n  method: patch\n  operationId: updateOneBaseWarehouseControllerWarehouse\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /warehouse/{id}\n  method: delete\n  operationId:\
  \ deleteOneBaseWarehouseControllerWarehouse\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /warehouse\n  method: get\n  operationId: getManyBaseWarehouseControllerWarehouse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /warehouse\n  method: post\n  operationId: createOneBaseWarehouseControllerWarehouse\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n\
  - path: /warehouse/{id}/custom-forms\n  method: patch\n  operationId: WarehouseController_updateLoadTypesCustomForms\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /warehouse/{id}/custom-forms\n  method: post\n  operationId: WarehouseController_createLoadTypesCustomForms\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /warehouse/{id}/get-hours-of-operation\n  method: post\n  operationId: WarehouseController_getHOOPs\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /user/invite\n  method: post\n  operationId: UserController_invite\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /user/{id}\n  method: get\n  operationId: getOneBaseUserControllerUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/{id}\n  method: delete\n  operationId: deleteOneBaseUserControllerUser\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /user/{id}\n  method: patch\n  operationId: updateOneBaseUserControllerUser\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /user\n  method: get\n  operationId: getManyBaseUserControllerUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/email-available/{email}\n  method: get\n  operationId: UserController_isEmailAvailable\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/change-password\n  method: post\n  operationId: UserController_changePassword\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /user/accept-tc\n  method: post\n  operationId: UserController_acceptTC\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /carrier\n  method: get\n  operationId: getManyBaseCarrierControllerUser\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /carrier\n  method: post\n  operationId: createOneBaseCarrierControllerUser\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /carrier/booked\n  method: get\n  operationId: CarrierController_getManyBooked\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /carrier/{id}/org-carrier-settings\n  method: get\n  operationId: CarrierController_getOrgCarrierSettingsOrg\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /carrier/{id}/org-carrier-settings\n  method: patch\n  operationId: CarrierController_updateOrgCarrierSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /carrier/org-carrier-settings/{id}\n  method: get\n  operationId: CarrierController_getOrgCarrierSettingsCarrier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /carrier/preview\n  method: post\n  operationId: CarrierController_getCarrierPreviewToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n   \
  \   exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /carrier/settings\n  method: get\n  operationId: CarrierController_getCarrierSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /carrier/settings/favorite-warehouses\n  method: get\n  operationId: CarrierController_getFavoriteWarehouses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /carrier/settings/favorite-warehouses\n  method: post\n  operationId: CarrierController_addFavoriteWarehouse\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /carrier/settings/favorite-warehouses\n  method: delete\n  operationId: CarrierController_removeFavoriteWarehouse\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /carrier/{id}\n  method: get\n  operationId: getOneBaseCarrierControllerUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /org/{id}\n  method: get\n  operationId: getOneBaseOrgControllerOrg\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /org/{id}\n  method:\
  \ patch\n  operationId: updateOneBaseOrgControllerOrg\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /org/{orgId}/report-search\n  method: post\n  operationId: OrgController_createReportSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /org/{orgId}/report-search\n  method: get\n  operationId: OrgController_getAllReportSearches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n- path: /org/{orgId}/report-search/{reportSearchKey}\n  method: patch\n  operationId: OrgController_updateReportSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /org/{orgId}/report-search/{reportSearchKey}\n  method: delete\n  operationId: OrgController_deleteReportSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /org/{orgId}/favorite-carriers\n  method: patch\n  operationId: OrgController_updateFavoriteCarriers\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /org/{id}/custom-tags\n  method: patch\n  operationId: OrgController_updateCustomTags\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /company\n  method: get\n  operationId: getManyBaseCompanyControllerCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company\n  method: post\n  operationId:\
  \ createOneBaseCompanyControllerCompany\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /company/{id}\n  method: get\n  operationId: getOneBaseCompanyControllerCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/login\n  method: post\n  operationId: AuthController_login\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /auth/refresh\n\
  \  method: get\n  operationId: AuthController_refresh\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/profile\n  method: get\n  operationId: AuthController_getProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/me\n  method: get\n  operationId: AuthController_getProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dock\n  method: post\n  operationId: createOneBaseDockControllerDock\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /dock\n  method: get\n  operationId: getManyBaseDockControllerDock\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dock/{id}\n  method: patch\n  operationId: updateOneBaseDockControllerDock\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /dock/{id}\n  method: delete\n  operationId: deleteOneBaseDockControllerDock\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n \
  \     human-in-the-loop: required\n    audit: required\n- path: /dock/{id}\n  method: get\n  operationId: getOneBaseDockControllerDock\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dock/sort\n  method: post\n  operationId: DockController_updateSort\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /dock/{id}/compute-availability\n  method: post\n  operationId: DockController_availability\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /dock/{id}/get-availability\n  method: post\n  operationId: DockController_availability\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /dock/compute-open-dates\n  method: post\n  operationId: DockController_openDates\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /dock/{id}/capacity\n  method: post\n  operationId: DockController_createCapacityChildDock\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /dock/{id}/capacity/{childId}\n  method: delete\n  operationId: DockController_unlinkCapacityDock\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /loadtype\n  method: post\n  operationId: createOneBaseLoadTypeControllerLoadType\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /loadtype\n  method: get\n  operationId: getManyBaseLoadTypeControllerLoadType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /loadtype/{id}\n  method: delete\n  operationId: deleteOneBaseLoadTypeControllerLoadType\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /loadtype/{id}\n  method: get\n  operationId: getOneBaseLoadTypeControllerLoadType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /loadtype/{id}\n  method: patch\n  operationId: updateOneBaseLoadTypeControllerLoadType\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /loadtype/{id}/get-availability\n  method: post\n  operationId: LoadTypeController_availability\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /loadtype/{id}/appointment-count\n  method: get\n  operationId: LoadTypeController_getAppointmentCount\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /loadtype-group\n  method: post\n  operationId: LoadTypeGroupController_createLoadTypeGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /loadtype-group\n  method: get\n  operationId: LoadTypeGroupController_getLoadTypeGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /loadtype-group/{id}\n  method: patch\n  operationId: LoadTypeGroupController_updateLoadTypeGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n\
  \      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /loadtype-group/{id}\n  method: delete\n  operationId: LoadTypeGroupController_deleteLoadTypeGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /unit-limit/configuration\n  method: post\n  operationId: UnitLimitController_setUpConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n\
  - path: /unit-limit/configuration\n  method: get\n  operationId: UnitLimitController_getConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /unit-limit/count\n  method: get\n  operationId: UnitLimitController_getCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /unit-limit/validate\n  method: post\n  operationId: UnitLimitController_validateUnitLimit\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /custom-forms/flow\n  method: post\n  operationId: createOneBaseFlowControllerFlow\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /custom-forms/flow\n  method: get\n  operationId: getManyBaseFlowControllerFlow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /custom-forms/flow/{id}\n  method: patch\n  operationId: updateOneBaseFlowControllerFlow\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /custom-forms/flow/{id}\n  method: get\n  operationId:\
  \ getOneBaseFlowControllerFlow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /custom-forms/flow/{id}\n  method: delete\n  operationId: deleteOneBaseFlowControllerFlow\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /custom-forms/form\n  method: post\n  operationId: createOneBaseFormControllerForm\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path:\
  \ /custom-forms/form\n  method: get\n  operationId: getManyBaseFormControllerForm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /custom-forms/form/{id}\n  method: patch\n  operationId: updateOneBaseFormControllerForm\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /custom-forms/form/{id}\n  method: get\n  operationId: getOneBaseFormControllerForm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /custom-forms/form/{id}\n  method: delete\n  operationId: deleteOneBaseFormControllerForm\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /custom-forms/form/sort/{id}\n  method: patch\n  operationId: FormController_sortFormFields\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /custom-forms/field\n  method: post\n  operationId: createOneBaseFieldControllerField\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /custom-forms/field\n  method: get\n  operationId: getManyBaseFieldControllerField\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /custom-forms/field/{id}\n  method: patch\n  operationId: updateOneBaseFieldControllerField\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /custom-forms/field/{id}\n  method: get\n  operationId: getOneBaseFieldControllerField\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /custom-forms/field/{id}\n  method: delete\n  operationId: deleteOneBaseFieldControllerField\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /custom-forms/form-field\n  method: post\n  operationId: createOneBaseFormFieldControllerFormField\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /custom-forms/form-field\n  method: get\n  operationId: getManyBaseFormFieldControllerFormField\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /custom-forms/form-field/{id}\n  method: patch\n  operationId: updateOneBaseFormFieldControllerFormField\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /custom-forms/form-field/{id}\n  method: get\n  operationId: getOneBaseFormFieldControllerFormField\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /custom-forms/form-field/{id}\n  method: delete\n  operationId: deleteOneBaseFormFieldControllerFormField\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /custom-forms/trigger\n  method: get\n  operationId: getManyBaseTriggerControllerTrigger\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /custom-forms/trigger\n  method: post\n  operationId: createOneBaseTriggerControllerTrigger\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /custom-forms/trigger/{id}\n  method: patch\n  operationId: updateOneBaseTriggerControllerTrigger\n  x-agentic-access:\n \
  \   action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /custom-forms/trigger/{id}\n  method: delete\n  operationId: deleteOneBaseTriggerControllerTrigger\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /custom-forms/trigger/{id}\n  method: get\n  operationId: getOneBaseTriggerControllerTrigger\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\n\n# --- truncated at 32 KB (90\
  \ KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/loadsmart/refs/heads/main/agentic-access/loadsmart-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loadsmart/refs/heads/main/agentic-access/loadsmart-agentic-access.yml
summary_line: 284 operations · 160 acting · 122 human-in-the-loop
tags:
- Freight
- Logistics
- Transportation
- Supply Chain
- Digital Freight
- Freight Brokerage
- Truckload
- LTL
- Drayage
- Flatbed
- Multimodal
- TMS
- Dock Scheduling
- Yard Management
- Warehouse
- 4PL
- FreightTech
---
