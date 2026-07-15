---
acting_count: 604
action_class_counts:
  acting: 604
  connected: 273
api_specs:
- filename: frontegg-identity-openapi.yml
  format: yaml
  label: Frontegg Authentication and Identity Management API
  slug: frontegg-identity
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frontegg/refs/heads/main/openapi/frontegg-identity-openapi.yml
- filename: frontegg-tenants-openapi.yml
  format: yaml
  label: Frontegg Account Management API
  slug: frontegg-tenants
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frontegg/refs/heads/main/openapi/frontegg-tenants-openapi.yml
- filename: frontegg-sso-openapi.yml
  format: yaml
  label: Frontegg Single Sign-On API
  slug: frontegg-sso
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frontegg/refs/heads/main/openapi/frontegg-sso-openapi.yml
- filename: frontegg-scim-openapi.yml
  format: yaml
  label: Frontegg SCIM Provisioning API
  slug: frontegg-scim
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frontegg/refs/heads/main/openapi/frontegg-scim-openapi.yml
- filename: frontegg-entitlements-openapi.yml
  format: yaml
  label: Frontegg Entitlements API
  slug: frontegg-entitlements
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frontegg/refs/heads/main/openapi/frontegg-entitlements-openapi.yml
- filename: frontegg-entitlements-agent-openapi.yml
  format: yaml
  label: Frontegg Entitlements Agent (PDP)
  slug: frontegg-entitlements-agent
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frontegg/refs/heads/main/openapi/frontegg-entitlements-agent-openapi.yml
- filename: frontegg-applications-openapi.yml
  format: yaml
  label: Frontegg Multi-Apps API
  slug: frontegg-applications
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frontegg/refs/heads/main/openapi/frontegg-applications-openapi.yml
- filename: frontegg-audits-openapi.yml
  format: yaml
  label: Frontegg Audits API
  slug: frontegg-audits
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frontegg/refs/heads/main/openapi/frontegg-audits-openapi.yml
- filename: frontegg-env-auth-openapi.yml
  format: yaml
  label: Frontegg Environment Authentication API
  slug: frontegg-env-auth
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frontegg/refs/heads/main/openapi/frontegg-env-auth-openapi.yml
- filename: frontegg-combined-openapi.yml
  format: yaml
  label: Frontegg Combined API
  slug: frontegg-combined
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frontegg/refs/heads/main/openapi/frontegg-combined-openapi.yml
- filename: frontegg-webhooks-asyncapi.yml
  format: yaml
  label: Frontegg Webhooks
  slug: frontegg-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/frontegg/refs/heads/main/asyncapi/frontegg-webhooks-asyncapi.yml
consequence_counts:
  read: 273
  safety-critical: 578
  write: 26
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 578
kind: agentic-access
layout: agentic-access
method: generated
name: Frontegg Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /export/csv
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /export/csv
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /export/csv/v2
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /export/csv/v2
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /resources/account-settings/v1
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /resources/account-settings/v1
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /resources/applications/user-tenants/active/v1
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /resources/applications/user-tenants/active/v1
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /resources/applications/v1
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /resources/applications/v1
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /resources/applications/v1
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /resources/applications/v1
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /resources/approval-flows/v1
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /resources/approval-flows/v1
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /resources/approval-flows/v1/approver-action
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /resources/approval-flows/v1/approver-action
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /resources/approval-flows/v1/step-up/execute
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /resources/approval-flows/v1/step-up/execute
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /resources/approval-flows/v1/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /resources/approval-flows/v1/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /resources/approval-flows/v1/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /resources/approval-flows/v1/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /resources/approval-flows/v1/{id}/execute
operation_count: 877
overview: 'Frontegg exposes 877 API operations that an AI agent could call, of which 604 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 273 read, 26 write, and 578 safety-critical.


  578 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Frontegg
provider_slug: frontegg
slug: frontegg-agentic-access
source_filename: frontegg-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/frontegg-applications-openapi.yml, openapi/frontegg-audits-openapi.yml, openapi/frontegg-combined-openapi.yml,\n  openapi/frontegg-entitlements-agent-openapi.yml, openapi/frontegg-entitlements-openapi.yml,\n  openapi/frontegg-env-auth-openapi.yml, openapi/frontegg-identity-openapi.yml, openapi/frontegg-scim-openapi.yml,\n  openapi/frontegg-sso-openapi.yml, openapi/frontegg-tenants-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 877\n  by_action_class:\n    connected: 273\n    acting: 604\n  by_consequence:\n    read: 273\n    write: 26\n    safety-critical: 578\n  human_in_the_loop_required: 578\noperations:\n- path: /resources/applications/v1\n  method: get\n  operationId:\
  \ getApplications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resources/applications/v1\n  method: post\n  operationId: createApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /resources/applications/v1/default\n  method: get\n  operationId: getDefaultApplication\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resources/applications/v1/{id}\n  method: get\n  operationId: getApplicationById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /resources/applications/v1/{id}\n  method: patch\n  operationId: updateApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /resources/applications/v1/{id}\n  method: delete\n  operationId: deleteApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /resources/applications/tenant-assignments/v1\n  method: get\n  operationId: getApplicationsTenantsAssignments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /resources/applications/tenant-assignments/v1/{appId}\n  method: get\n  operationId: getApplicationTenantsAssignmentsByAppId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resources/applications/tenant-assignments/v1/{appId}\n  method: post\n  operationId: createApplicationTenantAssignment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /resources/applications/tenant-assignments/v1/{appId}/{tenantId}\n  method: put\n  operationId: editApplicationTenantAssignment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /resources/applications/tenant-assignments/v1/{appId}/{tenantId}\n  method: delete\n  operationId: deleteApplicationTenantAssignment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /resources/applications/tenant-assignments/v2\n  method: get\n  operationId: getApplicationsTenantsAssignmentsV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resources/applications/v1/credentials/{appId}\n  method: get\n  operationId: getApplicationClientCredentials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resources/applications/v1/credentials/regenerate\n  method: post\n  operationId: regenerateApplicationClientCredentials\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /resources/applications/v1/credentials/shared/regenerate\n  method: post\n  operationId: regenerateApplicationSharedSecretCredentials\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /application-clients\n  method: post\n  operationId: createApplicationClient\n  x-agentic-access:\n   \
  \ action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /application-clients/app/{appId}\n  method: get\n  operationId: getApplicationClientsByAppId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /application-clients/{id}\n  method: get\n  operationId: getApplicationClientById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /application-clients/{id}\n  method: patch\n  operationId: updateApplicationClient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n     \
  \ human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /application-clients/{id}\n  method: delete\n  operationId: deleteApplicationClient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /\n  method: get\n  operationId: AuditsController_getAudits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: post\n  operationId: AuditsController_addAudits\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /stats\n  method: get\n  operationId: AuditsController_getAuditsStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /export/csv\n  method: post\n  operationId: AuditsController_exportCsv\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /export/csv/v2\n  method: post\n  operationId: AuditsController_exportCsvToStream\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n\
  \      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /resources/audits/v2\n  method: get\n  operationId: AuditsController_V2_getAudits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resources/audits/v2/export/csv\n  method: post\n  operationId: AuditsController_V2_exportCsvToStream\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /resources/metrics/v1\n  method: get\n  operationId: MetricsController_getMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/data/e10s/features/is_entitled_to_input_feature\n  method: post\n  operationId: OpenApiPDPController_isEntitledToFeature\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/data/e10s/permissions/is_entitled_to_input_permission\n  method: post\n  operationId: OpenApiPDPController_isEntitledToPermission\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/data/e10s/routes/is_entitled_to_input_route\n  method: post\n  operationId:\
  \ OpenApiPDPController_isEntitledToRoute\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /\n  method: get\n  operationId: AuditsController_getAudits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: post\n  operationId: AuditsController_addAudits\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /stats\n  method: get\n  operationId:\
  \ AuditsController_getAuditsStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /export/csv\n  method: post\n  operationId: AuditsController_exportCsv\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /export/csv/v2\n  method: post\n  operationId: AuditsController_exportCsvToStream\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /resources/audits/v2\n\
  \  method: get\n  operationId: AuditsController_V2_getAudits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resources/audits/v2/export/csv\n  method: post\n  operationId: AuditsController_V2_exportCsvToStream\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /resources/metrics/v1\n  method: get\n  operationId: MetricsController_getMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resources/plans/v1/tenant/{tenantId}\n  method: get\n  operationId: PlansControllerV1_getTenantPlans\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resources/plans/v1\n  method: get\n  operationId: PlansControllerV1_getPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resources/plans/v1\n  method: post\n  operationId: PlansControllerV1_createPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /resources/plans/v1/{id}\n  method: get\n  operationId: PlansControllerV1_getSinglePlan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /resources/plans/v1/{id}\n  method: patch\n  operationId: PlansControllerV1_updatePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /resources/plans/v1/{id}\n  method: delete\n  operationId: PlansControllerV1_deletePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /resources/plans/v1/{id}/features\n  method: get\n  operationId: PlansControllerV1_getPlanFeatures\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resources/plans/v1/{id}/features/link\n  method: patch\n  operationId: PlansControllerV1_linkFeaturesToPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /resources/plans/v1/{id}/features/unlink\n  method: patch\n  operationId: PlansControllerV1_unlinkFeaturesFromPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /resources/routes/v1\n  method: get\n  operationId:\
  \ RoutesControllerV1_getMany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resources/routes/v1\n  method: post\n  operationId: RoutesControllerV1_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /resources/routes/v1/{id}\n  method: get\n  operationId: RoutesControllerV1_getSingle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resources/routes/v1/{id}\n  method: delete\n  operationId: RoutesControllerV1_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /resources/routes/v1/{id}\n  method: patch\n  operationId: RoutesControllerV1_update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /resources/routes/v1/import-open-api\n  method: post\n  operationId: RoutesControllerV1_importOpenApi\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /resources/routes/v1/{id}/rules\n  method: put\n  operationId: RoutesControllerV1_replaceRules\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /resources/routes/v1/configuration\n  method: get\n  operationId: RoutesConfigurationsControllerV1_getRoutesConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resources/routes/v1/configuration\n  method: patch\n  operationId: RoutesConfigurationsControllerV1_updateRoutesConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /resources/features/v1\n  method: get\n  operationId: FeaturesControllerV1_getFeatures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resources/features/v1\n  method: post\n  operationId: FeaturesControllerV1_createFeature\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /resources/features/v1/{featureId}\n  method: patch\n  operationId: FeaturesControllerV1_updateFeature\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /resources/features/v1/{featureId}\n  method: delete\n  operationId: FeaturesControllerV1_deleteFeature\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /resources/features/v2\n  method: post\n  operationId: FeaturesControllerV2_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n\
  \      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /resources/features/v2/{featureId}\n  method: patch\n  operationId: FeaturesControllerV2_update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /resources/entitlements/v2\n  method: get\n  operationId: EntitlementsControllerV2_getEntitlements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resources/entitlements/v2\n  method: post\n  operationId: EntitlementsControllerV2_createEntitlement\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /resources/entitlements/v2/batch\n  method: post\n  operationId: EntitlementsControllerV2_createBatchEntitlements\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /resources/entitlements/v2/batch\n  method: patch\n  operationId: EntitlementsControllerV2_updateBatchEntitlements\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n\
  \    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /resources/entitlements/v2/batch\n  method: delete\n  operationId: EntitlementsControllerV2_deleteBatchEntitlements\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /resources/entitlements/v2/{id}\n  method: get\n  operationId: EntitlementsControllerV2_getSingleEntitlement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resources/entitlements/v2/{id}\n  method: patch\n  operationId: EntitlementsControllerV2_updateEntitlement\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n \
  \   audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /resources/entitlements/v2/{id}\n  method: delete\n  operationId: EntitlementsControllerV2_deleteEntitlement\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /resources/feature-flags/v1\n  method: get\n  operationId: FeatureFlagsControllerV1_getFeatureFlags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resources/feature-flags/v1\n  method: post\n  operationId: FeatureFlagsControllerV1_createFeatureFlag\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /resources/feature-flags/v1/{id}\n  method: get\n  operationId: FeatureFlagsControllerV1_getSingleFeatureFlag\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resources/feature-flags/v1/{id}\n  method: patch\n  operationId: FeatureFlagsControllerV1_updateFeatureFlag\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit:\
  \ required\n- path: /resources/feature-flags/v1/{id}\n  method: delete\n  operationId: FeatureFlagsControllerV1_deleteFeatureFlag\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /resources/entity-types/v1\n  method: get\n  operationId: EntityTypesV1Controller_getEntityTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resources/entity-types/v1\n  method: post\n  operationId: EntityTypesV1Controller_createEntityType\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /resources/entity-types/v1/{key}\n  method: get\n  operationId: EntityTypesV1Controller_getEntityType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resources/entity-types/v1/{key}\n  method: patch\n  operationId: EntityTypesV1Controller_updateEntityType\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /resources/entity-types/v1/{key}\n  method: delete\n  operationId: EntityTypesV1Controller_deleteEntityType\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /resources/entity-types/v1/{key}/actions\n  method: post\n  operationId: EntityTypesActionsV1Controller_createEntityTypeActions\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /resources/entity-types/v1/{key}/actions/{actionKey}\n  method: patch\n  operationId: EntityTypesActionsV1Controller_updateEntityTypeAction\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange:\
  \ true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /resources/entity-types/v1/{key}/actions/{actionKey}\n  method: delete\n  operationId: EntityTypesActionsV1Controller_deleteEntityTypeAction\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /resources/entity-types/v1/{key}/relations\n  method: post\n  operationId: EntityTypesRelationsV1Controller_createEntityTypeRelations\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /resources/entity-types/v1/{key}/relations/{relationKey}\n  method: patch\n  operationId: EntityTypesRelationsV1Controller_updateEntityTypeRelation\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /resources/entity-types/v1/{key}/relations/{relationKey}\n  method: delete\n  operationId: EntityTypesRelationsV1Controller_deleteEntityTypeRelation\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n\
  - path: /resources/relations/v1/assignments\n  method: get\n  operationId: RelationsV1Controller_getRelationAssignments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resources/relations/v1/assign\n  method: post\n  operationId: RelationsV1Controller_createRelationAssignments\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /resources/relations/v1/unassign\n  method: post\n  operationId: RelationsV1Controller_deleteRelationAssignments\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n\
  \      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /resources/auth/v2/api-token\n  method: post\n  operationId: AuthenticationApiTokenControllerV2_authApiToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /resources/auth/v2/api-token/token/refresh\n  method: post\n  operationId: AuthenticationApiTokenControllerV2_refreshToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit:\
  \ required\n- path: /r\n\n# --- truncated at 32 KB (317 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/frontegg/refs/heads/main/agentic-access/frontegg-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/frontegg/refs/heads/main/agentic-access/frontegg-agentic-access.yml
summary_line: 877 operations · 604 acting · 578 human-in-the-loop
tags:
- Authentication
- Authorization
- Identity Management
- CIAM
- B2B SaaS
- Multi-Tenancy
- RBAC
- SSO
- SCIM
- Entitlements
- OAuth
- OpenID Connect
---
