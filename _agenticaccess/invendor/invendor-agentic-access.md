---
acting_count: 194
action_class_counts:
  acting: 194
  connected: 159
api_specs:
- filename: invendor-common-openapi-original.json
  format: json
  label: Invendor Common API
  slug: invendor-common-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/invendor/refs/heads/main/openapi/invendor-common-openapi-original.json
- filename: invendor-reporting-openapi-original.json
  format: json
  label: Invendor Reporting API
  slug: invendor-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/invendor/refs/heads/main/openapi/invendor-reporting-openapi-original.json
consequence_counts:
  physical: 21
  read: 159
  safety-critical: 3
  write: 170
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Invendor Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/Accounts/{accountId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/Users/{userId}/password-reset-email
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/Users/{userId}/reset-mfa
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/Devices/{deviceId}/command
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/Items/bulk
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/Items/sendToTenant
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/Locations/{locationId}/accounts/{accountId}/order-notifications
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/Locations/{locationId}/order-notifications
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/Locations/{locationId}/vendors/{accountIdToUpdate}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/Orders/location/param
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/Orders/location/{locationId}/param
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/Orders/purchase
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/Orders/replenishment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/Orders/{orderId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/Orders/{orderId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/Orders/{orderId}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/Orders/{orderId}/complete
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/Orders/{orderId}/confirm
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/Orders/{orderId}/journal/reception
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/Orders/{orderId}/line
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/Orders/{orderId}/line/{orderLineId}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/Orders/{orderId}/lines
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/Orders/{orderId}/receive
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/Orders/{orderId}/ship
operation_count: 353
overview: 'Invendor exposes 353 API operations that an AI agent could call, of which 194 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 159 read, 170 write, 21 physical, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Invendor
provider_slug: invendor
slug: invendor-agentic-access
source_filename: invendor-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/invendor-common-openapi-original.json, openapi/invendor-reporting-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 353\n  by_action_class:\n    connected: 159\n    acting: 194\n  by_consequence:\n    read: 159\n    write: 170\n    safety-critical: 3\n    physical: 21\n  human_in_the_loop_required: 3\noperations:\n- path: /v1/Accounts/me\n  method: get\n  operationId: My account details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Accounts\n  method: get\n  operationId: Accounts list\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    scope:\n    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Accounts\n  method: post\n  operationId: Create account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Accounts/{accountId}\n  method: get\n  operationId: Account details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Accounts/{accountId}\n  method: put\n  operationId: Update account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Accounts/{accountId}\n  method: delete\n  operationId: Delete account\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/Accounts/fromInvitation\n  method: post\n  operationId: Create account from invitation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Accounts/{accountId}/fromInvitation\n\
  \  method: put\n  operationId: Create account linked settings from invitation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Accounts/{accountId}/linkedLocations\n  method: put\n  operationId: Update linked account locations mapping\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Accounts/{accountId}/linkedOperations\n  method: put\n  operationId: Update linked account operations mapping\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Accounts/{accountId}/profiles\n  method: post\n  operationId: Add related profile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Accounts/{accountId}/profiles/{userProfileId}\n  method: delete\n  operationId: Delete related profile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Accounts/vendors\n  method: get\n  operationId: Account vendors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Accounts/invitation\n  method: get\n  operationId: Client accepts vendor invitation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Accounts/invitation\n  method: post\n  operationId: Vendor invitation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Accounts/linkedClientsTenants\n\
  \  method: get\n  operationId: Account's clients' tenants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Accounts/{accountId}/linkedSettings/validation\n  method: get\n  operationId: Validate linked account configuration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Accounts/integration\n  method: delete\n  operationId: Delete account integration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Accounts/validate\n  method: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Accounts/validate\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/Auth/login\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/Auth/logout\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/Auth/status\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Barcodes/item/scaleLocker\n  method: get\n  operationId: Get all items barcodes for scale lockers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/DataJobs\n  method: get\n  operationId: GetDataJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/DataJobs/{jobId}/download\n  method: get\n  operationId: DownloadDataJobResult\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    scope:\n    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Devices/commands\n  method: get\n  operationId: Device commands\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Devices\n  method: get\n  operationId: Devices list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Devices/{deviceId}\n  method: get\n  operationId: Device details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Devices/{deviceId}\n  method: put\n  operationId: Update tenant device information\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Devices/{deviceId}\n  method: delete\n  operationId: Delete tenant device\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Devices/{deviceId}/command\n  method: post\n  operationId: Send command to the device\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Devices/locations/{locationId}/sync_users\n  method: post\n  operationId: Sync location users in related devices\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Devices/{deviceId}/heartbeats\n  method: get\n  operationId: Device heartbeats list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Devices/{deviceId}/events\n  method: get\n  operationId: Device events list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    scope:\n    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Devices/dedicated/register/pre\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Devices/{deviceId}/regen\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Devices/free-cabinets\n  method: get\n  operationId: Free cabinets list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n\
  \    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Dimensions\n  method: get\n  operationId: GetDimensionsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Dimensions\n  method: post\n  operationId: CreateDimension\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Dimensions/{id}\n  method: get\n  operationId: GetDimensionDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Dimensions/{id}\n  method: put\n  operationId:\
  \ UpdateDimension\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Dimensions/{id}\n  method: delete\n  operationId: DeleteDimension\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Dimensions/{id}/operations\n  method: get\n  operationId: GetDimensionOperations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Dimensions/properties\n\
  \  method: get\n  operationId: GetAllUsedDimensionProperties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Dimensions/values/properties\n  method: get\n  operationId: GetAllUsedDimensionValueProperties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Dimensions/params\n  method: get\n  operationId: Account dimensions parameters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Dimensions/params\n  method: post\n  operationId: Account dimensions parameters\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - io.common\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Dimensions/{dimId}/values\n  method: get\n  operationId: Get dimension values\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Dimensions/{dimId}/values\n  method: post\n  operationId: CreateDimensionValue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Dimensions/{dimId}/values\n  method: put\n  operationId: UpdateDimensionValue\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Dimensions/{dimId}/values/{valueId}\n  method: get\n  operationId: GetDimensionValue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Dimensions/{dimId}/values/{valueId}/parents\n  method: get\n  operationId: GetDimensionValueParents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Dimensions/{dimId}/values/{valueId}/children\n  method: get\n  operationId: GetDimensionValueChildren\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    scope:\n    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Dimensions/{dimId}/values/{valueId}/children\n  method: post\n  operationId: SaveDimensionValueChildren\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Dimensions/{dimId}/values/bulk\n  method: post\n  operationId: CreateDimensionValuesBulk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Dimensions/{dimId}/values/bulk\n  method: delete\n  operationId: DeleteDimensionValuesBulk\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Doors\n  method: get\n  operationId: Get doors list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/DynamicScanContent/datasources\n  method: get\n  operationId: DynamicContentFieldDatasources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/DynamicScanContent/datasources/{operationId}\n  method: get\n  operationId: OperationDynamicContentFieldDatasources\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    scope:\n    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ExtendedProperties/{affinity}\n  method: get\n  operationId: Get global extended properties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ExtendedProperties/{affinity}/{ownerId}\n  method: get\n  operationId: Get extended properties for the object\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ExtendedProperties/{affinity}/{ownerId}\n  method: post\n  operationId: Create extended property for the object\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ExtendedProperties/{affinity}/{ownerId}/{key}\n  method: put\n  operationId: Update extended property for the object\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ExtendedProperties/{affinity}/{ownerId}/{key}\n  method: delete\n  operationId: Delete extended property for the object\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/FlagTypes\n  method: get\n  operationId: Get flag types\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/FlagTypes\n  method: post\n  operationId: Create flag type\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/FlagTypes/{id}\n  method: get\n  operationId: Get flag type\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/FlagTypes/{id}\n  method: put\n  operationId: Update flag type\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/FlagTypes/{id}\n  method: delete\n  operationId: Delete flag type\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/GlobalSettings/types\n  method: get\n  operationId: Get global settings types list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/GlobalSettings\n  method: get\n  operationId: Get global settings list\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/GlobalSettings\n  method: post\n  operationId: Create global setting\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/GlobalSettings/{id}\n  method: get\n  operationId: Get a global setting by it's id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/GlobalSettings/{id}\n  method: put\n  operationId: Change global setting\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n\
  \    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/GlobalSettings/{id}\n  method: delete\n  operationId: Delete global setting\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/GlobalSettings/bulk\n  method: put\n  operationId: Bulk update global settings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /v1/GlobalSettings/logo\n  method: get\n  operationId: Get tenant logo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/GlobalSettings/logo\n  method: post\n  operationId: Upload tenant logo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/GlobalSettings/logo/url\n  method: post\n  operationId: Update tenant logo URL\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n   \
  \   - high-value\n    audit: required\n- path: /v1/ItemQuantities\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ItemQuantities/stockValue\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Items\n  method: get\n  operationId: GetItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Items\n  method: post\n  operationId: CreateItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Items/{serviceId}/items\n  method: get\n  operationId: GetServiceItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Items/{itemId}\n  method: get\n  operationId: GetItemDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Items/{itemId}\n  method: put\n  operationId: UpdateItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Items/{itemId}\n  method: delete\n\
  \  operationId: DeleteItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Items/{itemId}/conversions\n  method: get\n  operationId: GetItemUnitConversions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Items/{itemId}/altitems\n  method: get\n  operationId: GetItemAltItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Items/{itemId}/altitems\n  method: post\n  operationId: CreateItemAltItem\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: write\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Items/{itemId}/altitems\n  method: put\n  operationId: UpdateItemAltItemByItemId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Items/{itemId}/altitems\n  method: delete\n  operationId: DeleteItemAltItemByItemId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Items/altitems/{altItemId}\n  method: put\n  operationId: UpdateItemAltItemById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Items/altitems/{altItemId}\n  method: delete\n  operationId: DeleteItemAltItemById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Items/altitems/bulk\n  method: post\n  operationId: BulkUpsertAltItems\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Items/properties\n  method: get\n  operationId: GetAllUsedItemProperties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Items/definedProperties\n  method: get\n  operationId: Get defined properties for items\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - io.common\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Items/definedProperties\n  method: post\n  operationId: Create item defined property with parameters\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n\
  \    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Items/definedProperties/{id}\n  method: put\n  operationId: Update item defined property with parameters\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Items/definedProperties/{id}\n  method: delete\n  operationId: Delete item defined propety with parameters\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - io.common\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /v1/Items/definedProperties/bulk\n  method: post\n  operationId: Create or\n\n# --- truncated at 32 KB (111 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/invendor/refs/heads/main/agentic-access/invendor-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/invendor/refs/heads/main/agentic-access/invendor-agentic-access.yml
summary_line: 353 operations · 194 acting · 3 human-in-the-loop
tags:
- Company
- Inventory Management
- Vendor Managed Inventory
- Industrial Vending
- Supply Chain
- Warehouse Management
- Asset Tracking
---
