---
acting_count: 26
action_class_counts:
  acting: 26
  connected: 10
api_specs:
- filename: keysavvy-authentication-api-openapi.yml
  format: yaml
  label: KeySavvy Authentication API
  slug: keysavvy-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keysavvy/refs/heads/main/openapi/keysavvy-authentication-api-openapi.yml
- filename: keysavvy-deal-documents-api-openapi.yml
  format: yaml
  label: KeySavvy Deal Documents API
  slug: keysavvy-deal-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keysavvy/refs/heads/main/openapi/keysavvy-deal-documents-api-openapi.yml
- filename: keysavvy-deal-management-api-openapi.yml
  format: yaml
  label: KeySavvy Deal Management API
  slug: keysavvy-deal-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keysavvy/refs/heads/main/openapi/keysavvy-deal-management-api-openapi.yml
- filename: keysavvy-documents-api-openapi.yml
  format: yaml
  label: KeySavvy Documents API
  slug: keysavvy-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keysavvy/refs/heads/main/openapi/keysavvy-documents-api-openapi.yml
- filename: keysavvy-keysavvy-partner-api-api-openapi.yml
  format: yaml
  label: KeySavvy KeySavvy Partner API
  slug: keysavvy-keysavvy-partner-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keysavvy/refs/heads/main/openapi/keysavvy-keysavvy-partner-api-api-openapi.yml
- filename: keysavvy-marketplace-management-api-openapi.yml
  format: yaml
  label: KeySavvy Marketplace Management API
  slug: keysavvy-marketplace-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keysavvy/refs/heads/main/openapi/keysavvy-marketplace-management-api-openapi.yml
- filename: keysavvy-organization-management-api-openapi.yml
  format: yaml
  label: KeySavvy Organization Management API
  slug: keysavvy-organization-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keysavvy/refs/heads/main/openapi/keysavvy-organization-management-api-openapi.yml
- filename: keysavvy-reporting-api-openapi.yml
  format: yaml
  label: KeySavvy Reporting API
  slug: keysavvy-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keysavvy/refs/heads/main/openapi/keysavvy-reporting-api-openapi.yml
- filename: keysavvy-user-management-api-openapi.yml
  format: yaml
  label: KeySavvy User Management API
  slug: keysavvy-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keysavvy/refs/heads/main/openapi/keysavvy-user-management-api-openapi.yml
- filename: keysavvy-vehicle-management-api-openapi.yml
  format: yaml
  label: KeySavvy Vehicle Management API
  slug: keysavvy-vehicle-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keysavvy/refs/heads/main/openapi/keysavvy-vehicle-management-api-openapi.yml
- filename: keysavvy-webhook-management-api-openapi.yml
  format: yaml
  label: KeySavvy Webhook Management API
  slug: keysavvy-webhook-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keysavvy/refs/heads/main/openapi/keysavvy-webhook-management-api-openapi.yml
consequence_counts:
  physical: 2
  read: 10
  write: 24
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Keysavvy Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /deal/{referenceId}/estimated-transfer-date
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /user/{referenceId}/login-link
operation_count: 36
overview: 'KeySavvy exposes 36 API operations that an AI agent could call, of which 26 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read, 24 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: KeySavvy
provider_slug: keysavvy
slug: keysavvy-agentic-access
source_filename: keysavvy-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: generated\nsource: openapi/keysavvy-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 36\n  by_action_class:\n    acting: 26\n    connected: 10\n  by_consequence:\n    write: 24\n    read: 10\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /webhook/dashboard\n  method: post\n  operationId: createWebhookDashboardSessionUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /marketplace\n  method: post\n  operationId: createMarketplace\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /marketplace/{referenceId}\n  method: get\n  operationId: getMarketplace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /marketplace/{referenceId}\n  method: patch\n  operationId: updateMarketplace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /marketplace/{referenceId}/logo\n  method: post\n  operationId: uploadMarketplaceLogo\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization\n  method: get\n  operationId: getOrganizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization\n  method: post\n  operationId: createOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{referenceId}\n  method: get\n  operationId: getOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /organization/{referenceId}\n  method: patch\n  operationId: updateOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{referenceId}/users\n  method: get\n  operationId: getOrganizationUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{referenceId}/users\n  method: post\n  operationId: addOrganizationUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /organization/{referenceId}/users/{userReferenceId}\n  method: get\n  operationId: getOrganizationUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{referenceId}/users/{userReferenceId}\n  method: delete\n  operationId: removeOrganizationUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user\n  method: post\n  operationId: createUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/{referenceId}\n\
  \  method: get\n  operationId: getUserDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/{referenceId}\n  method: patch\n  operationId: patchUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/{referenceId}\n  method: post\n  operationId: updateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/{referenceId}/summary\n  method: get\n  operationId: getUserSummary\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/{referenceId}/login-link\n  method: post\n  operationId: sendUserMagicLoginLink\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/{userReferenceId}/document\n  method: post\n  operationId: uploadUserDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vehicle\n  method: post\n  operationId: createVehicle\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vehicle/{referenceId}\n  method: get\n  operationId: getVehicleDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vehicle/{vehicleReferenceId}/document\n  method: post\n  operationId: uploadVehicleDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deal/{referenceId}/bill-of-lading-link\n  method: post\n  operationId: uploadBillOfLadingLink\n  x-agentic-access:\n    action-class: acting\n  \
  \  consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deal/{referenceId}/bill-of-lading-upload\n  method: post\n  operationId: uploadBillOfLading\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vehicle/{vehicleReferenceId}/deal\n  method: post\n  operationId: createVehicleDeal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deal\n  method:\
  \ post\n  operationId: createDeal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deal/{referenceId}\n  method: get\n  operationId: getDealDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deal/{referenceId}/price\n  method: patch\n  operationId: updateDealPrice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deal/{referenceId}/cancel\n  method: post\n  operationId: cancelDeal\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deal/{referenceId}/estimated-transfer-date\n  method: patch\n  operationId: updateEstimatedTransferDate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deal/{referenceId}/business-representative\n  method: patch\n  operationId: updateDealBusinessRepresentative\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deal/{referenceId}/buyer-organization\n  method: patch\n  operationId: updateDealBuyerOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deal/{dealReferenceId}/vehicle/document\n  method: post\n  operationId: uploadDealVehicleDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reporting/search\n  method: post\n  operationId: dealReportingSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth\n  method: post\n  operationId: authenticateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keysavvy/refs/heads/main/agentic-access/keysavvy-agentic-access.yml
summary_line: 36 operations · 26 acting
tags:
- Company
- Automotive
- Marketplace
- API
- FinTech
---
