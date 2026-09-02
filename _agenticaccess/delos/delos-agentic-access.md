---
acting_count: 23
action_class_counts:
  acting: 23
  connected: 16
api_specs:
- filename: delos-actions-api-openapi.yml
  format: yaml
  label: Delos Actions API
  slug: delos-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delos/refs/heads/main/openapi/delos-actions-api-openapi.yml
- filename: delos-admin-installations-api-openapi.yml
  format: yaml
  label: Delos Admin/installations API
  slug: delos-admin-installations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delos/refs/heads/main/openapi/delos-admin-installations-api-openapi.yml
- filename: delos-admin-products-api-openapi.yml
  format: yaml
  label: Delos Admin/products API
  slug: delos-admin-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delos/refs/heads/main/openapi/delos-admin-products-api-openapi.yml
- filename: delos-admin-products-bundles-api-openapi.yml
  format: yaml
  label: Delos Admin/products Bundles API
  slug: delos-admin-products-bundles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delos/refs/heads/main/openapi/delos-admin-products-bundles-api-openapi.yml
- filename: delos-admin-users-api-openapi.yml
  format: yaml
  label: Delos Admin/users API
  slug: delos-admin-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delos/refs/heads/main/openapi/delos-admin-users-api-openapi.yml
- filename: delos-global-api-openapi.yml
  format: yaml
  label: Delos Global API
  slug: delos-global-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delos/refs/heads/main/openapi/delos-global-api-openapi.yml
- filename: delos-installations-api-openapi.yml
  format: yaml
  label: Delos Installations API
  slug: delos-installations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delos/refs/heads/main/openapi/delos-installations-api-openapi.yml
- filename: delos-local-accounts-api-openapi.yml
  format: yaml
  label: Delos Local Accounts API
  slug: delos-local-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delos/refs/heads/main/openapi/delos-local-accounts-api-openapi.yml
- filename: delos-products-api-openapi.yml
  format: yaml
  label: Delos Products API
  slug: delos-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delos/refs/heads/main/openapi/delos-products-api-openapi.yml
- filename: delos-sessions-api-openapi.yml
  format: yaml
  label: Delos Sessions API
  slug: delos-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delos/refs/heads/main/openapi/delos-sessions-api-openapi.yml
- filename: delos-users-api-openapi.yml
  format: yaml
  label: Delos Users API
  slug: delos-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delos/refs/heads/main/openapi/delos-users-api-openapi.yml
consequence_counts:
  physical: 1
  read: 16
  safety-critical: 1
  write: 21
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Delos Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /users/product-invitations/{invitationId}/revoke
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /local-accounts/transfer
operation_count: 39
overview: 'Delos exposes 39 API operations that an AI agent could call, of which 23 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read, 21 write, 1 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Delos
provider_slug: delos
slug: delos-agentic-access
source_filename: delos-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: generated\nsource: openapi/delos-wellcube-cloud-be-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 39\n  by_action_class:\n    acting: 23\n    connected: 16\n  by_consequence:\n    write: 21\n    read: 16\n    safety-critical: 1\n    physical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /sessions\n  method: post\n  operationId: sessionCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/validate\n  method: get\n  operationId: sessionValidate\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /limited-sessions\n  method: post\n  operationId: limitedSessionCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /limited-sessions/refresh\n  method: post\n  operationId: limitedSessionRefresh\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{userId}/products\n  method: get\n  operationId: userProductsList\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/product-invitations\n  method: post\n  operationId: userProductInvitationCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/product-invitations/{invitationId}\n  method: get\n  operationId: userProductInvitationShow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/product-invitations/{invitationId}/confirm\n  method: post\n  operationId: userProductInvitationConfirm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/product-invitations/{invitationId}/revoke\n  method: post\n  operationId: userProductInvitationRevoke\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /users/product-invitations/{invitationId}/renew\n  method: post\n  operationId: userProductInvitationRenew\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/users/cognito-sessions\n  method: post\n  operationId:\
  \ adminUserCognitoSessionCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/users/limited-cognito-sessions\n  method: post\n  operationId: adminUserLimitedCognitoSessionCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/users/{userId}/products\n  method: get\n  operationId: adminUserProductsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/users/{userId}/products/{productId}\n  method:\
  \ post\n  operationId: adminUserProductsCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/users/{userId}/products/{productId}\n  method: put\n  operationId: adminUserProductsUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/users/{userId}/products/{productId}\n  method: delete\n  operationId: adminUserProductsDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/installations\n  method: get\n  operationId: adminInstallationsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/installations/{installationId}/products\n  method: get\n  operationId: adminInstallationsListAssociatedProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/installations/{installationId}/stats\n  method: get\n  operationId: adminInstallationStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/products\n  method: get\n  operationId: adminProductList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/products\n  method: post\n  operationId: adminProductCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/products/{productId}/stats\n  method: get\n  operationId: adminProductStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/products/{productId}\n  method: get\n  operationId: adminProductShow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/products/{productId}\n  method: put\n  operationId: adminProductUpdate\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/products/{productId}\n  method: delete\n  operationId: adminProductDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/products-bundles/aws\n  method: get\n  operationId: adminProductsBundlesAWSList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /actions/{actionId}\n  method: post\n  operationId: actionSubmit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /actions/{actionId}\n  method: get\n  operationId: actionShow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products\n  method: get\n  operationId: productList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /installations\n  method: get\n  operationId: installationsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /local-accounts/link\n  method: post\n  operationId: localAccountLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /local-accounts/share\n  method: post\n  operationId: localAccountShare\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /local-accounts/transfer\n  method: post\n  operationId: localAccountTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /local-accounts/{localAccountId}\n\
  \  method: put\n  operationId: localAccountUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /local-accounts/{localAccountId}/set-global\n  method: post\n  operationId: localAccountSetGlobal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/local-accounts/migrate-to-federated\n  method: post\n  operationId: localAccountMigrateToFederated\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /global/execute-nva\n  method: post\n  operationId: globalExecuteNVA\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /global/jobs/{jobId}\n  method: get\n  operationId: globalJobsShow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /global/jobs/{jobId}/results\n  method: get\n  operationId: globalJobsGetResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/delos/refs/heads/main/agentic-access/delos-agentic-access.yml
summary_line: 39 operations · 23 acting · 1 human-in-the-loop
tags:
- wellness-real-estate
- Indoor Air Quality
- indoor-environmental-quality
- IoT
- Smart Buildings
- Building Automation
- Air Purification
- environmental-sensors
- Commercial Real Estate
- healthy-buildings
- Hospitality
- ESG
---
