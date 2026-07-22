---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 12
api_specs:
- filename: topograph-openapi-original.json
  format: json
  label: Topograph API
  slug: topograph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/topograph/refs/heads/main/openapi/topograph-openapi-original.json
- filename: topograph-x402-openapi.json
  format: json
  label: Topograph x402 (agentic commerce)
  slug: topograph-x402-agentic-commerce
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/topograph/refs/heads/main/openapi/topograph-x402-openapi.json
consequence_counts:
  read: 12
  safety-critical: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 10
kind: agentic-access
layout: agentic-access
method: generated
name: Topograph Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v2/billing/notifications/config
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v2/billing/notifications/workspaces/{workspaceId}/config
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v2/billing/notifications/workspaces/{workspaceId}/config
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/company
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/monitors
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v2/monitors/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/onboarding
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/workspaces
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v2/workspaces/{name}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v2/workspaces/{name}
operation_count: 22
overview: 'Topograph exposes 22 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read and 10 safety-critical.


  10 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Topograph
provider_slug: topograph
slug: topograph-agentic-access
source_filename: topograph-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/topograph-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 12\n    acting: 10\n  by_consequence:\n    read: 12\n    safety-critical: 10\n  human_in_the_loop_required: 10\noperations:\n- path: /v2/pricing\n  method: get\n  operationId: PricingController_getPricing_v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/monitors\n  method: post\n  operationId: MonitoringController_createMonitor_v2\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/monitors\n  method: get\n  operationId: MonitoringController_listMonitors_v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/monitors/{id}\n  method: get\n  operationId: MonitoringController_getMonitor_v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/monitors/{id}\n  method: delete\n  operationId: MonitoringController_stopMonitoring_v2\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/monitors/{id}/logs\n  method: get\n  operationId: MonitoringController_getMonitorLogs_v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/search\n  method: get\n  operationId: SearchController_searchV2_v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/company\n  method: post\n  operationId: CompanyController_getCompany_v2\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/company/{requestId}\n  method: get\n\
  \  operationId: CompanyController_getCompanyRequest_v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/onboarding\n  method: post\n  operationId: CompanyOnboardingController_getOnboarding_v2\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/workspaces\n  method: get\n  operationId: WorkspaceController_listWorkspaces_v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/workspaces\n  method: post\n  operationId: WorkspaceController_createWorkspace_v2\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/workspaces/{name}\n  method: patch\n  operationId: WorkspaceController_updateWorkspace_v2\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/workspaces/{name}\n  method: delete\n  operationId: WorkspaceController_deleteWorkspace_v2\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n   \
  \   proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/workspaces/usage\n  method: get\n  operationId: WorkspaceController_getUsageReport_v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/billing/notifications/config\n  method: get\n  operationId: BillingNotificationsController_getConfig_v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/billing/notifications/config\n  method: patch\n  operationId: BillingNotificationsController_updateConfig_v2\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /v2/billing/notifications/recent\n  method: get\n  operationId: BillingNotificationsController_listRecent_v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/billing/notifications/workspaces/{workspaceId}/config\n  method: get\n  operationId: BillingNotificationsController_getWorkspaceOverride_v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/billing/notifications/workspaces/{workspaceId}/config\n  method: patch\n  operationId: BillingNotificationsController_upsertWorkspaceOverride_v2\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /v2/billing/notifications/workspaces/{workspaceId}/config\n  method: delete\n  operationId: BillingNotificationsController_deleteWorkspaceOverride_v2\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/billing/balance\n  method: get\n  operationId: BillingBalanceController_getBalance_v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/topograph/refs/heads/main/agentic-access/topograph-agentic-access.yml
summary_line: 22 operations · 10 acting · 10 human-in-the-loop
tags:
- Company
- KYB
- Company Data
- Business Registers
- Compliance
- Identity Verification
- Beneficial Ownership
- AML
- Due Diligence
- Fintech
---
