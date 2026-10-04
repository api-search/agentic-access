---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 13
api_specs:
- filename: topograph-billing-api-openapi.yml
  format: yaml
  label: Topograph Billing API
  slug: topograph-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/topograph/refs/heads/main/openapi/topograph-billing-api-openapi.yml
- filename: topograph-billing-notifications-api-openapi.yml
  format: yaml
  label: Topograph Billing Notifications API
  slug: topograph-billing-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/topograph/refs/heads/main/openapi/topograph-billing-notifications-api-openapi.yml
- filename: topograph-data-api-openapi.yml
  format: yaml
  label: Topograph Data API
  slug: topograph-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/topograph/refs/heads/main/openapi/topograph-data-api-openapi.yml
- filename: topograph-monitors-api-openapi.yml
  format: yaml
  label: Topograph Monitors API
  slug: topograph-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/topograph/refs/heads/main/openapi/topograph-monitors-api-openapi.yml
- filename: topograph-pricing-api-openapi.yml
  format: yaml
  label: Topograph Pricing API
  slug: topograph-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/topograph/refs/heads/main/openapi/topograph-pricing-api-openapi.yml
- filename: topograph-search-api-openapi.yml
  format: yaml
  label: Topograph Search API
  slug: topograph-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/topograph/refs/heads/main/openapi/topograph-search-api-openapi.yml
- filename: topograph-workspaces-api-openapi.yml
  format: yaml
  label: Topograph Workspaces API
  slug: topograph-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/topograph/refs/heads/main/openapi/topograph-workspaces-api-openapi.yml
consequence_counts:
  read: 13
  safety-critical: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 9
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
overview: 'Topograph exposes 22 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read and 9 safety-critical.


  9 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Topograph
provider_slug: topograph
slug: topograph-agentic-access
source_filename: topograph-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/topograph-billing-api-openapi.yml, openapi/topograph-billing-notifications-api-openapi.yml,\n  openapi/topograph-data-api-openapi.yml, openapi/topograph-monitors-api-openapi.yml, openapi/topograph-pricing-api-openapi.yml,\n  openapi/topograph-search-api-openapi.yml, openapi/topograph-workspaces-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 13\n    acting: 9\n  by_consequence:\n    read: 13\n    safety-critical: 9\n  human_in_the_loop_required: 9\noperations:\n- path: /v2/billing/balance\n  method: get\n  operationId: BillingBalanceController_getBalance_v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/billing/notifications/config\n  method: get\n  operationId: BillingNotificationsController_getConfig_v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/billing/notifications/config\n  method: patch\n  operationId: BillingNotificationsController_updateConfig_v2\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/billing/notifications/recent\n  method: get\n  operationId: BillingNotificationsController_listRecent_v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v2/billing/notifications/workspaces/{workspaceId}/config\n  method: get\n  operationId: BillingNotificationsController_getWorkspaceOverride_v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/billing/notifications/workspaces/{workspaceId}/config\n  method: patch\n  operationId: BillingNotificationsController_upsertWorkspaceOverride_v2\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/billing/notifications/workspaces/{workspaceId}/config\n  method: delete\n  operationId: BillingNotificationsController_deleteWorkspaceOverride_v2\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/company\n  method: post\n  operationId: CompanyController_getCompany_v2\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/company/{requestId}\n  method: get\n  operationId: CompanyController_getCompanyRequest_v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/onboarding\n  method: post\n  operationId: CompanyOnboardingController_getOnboarding_v2\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/monitors\n  method: post\n  operationId: MonitoringController_createMonitor_v2\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/monitors\n  method: get\n  operationId: MonitoringController_listMonitors_v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/monitors/{id}\n  method: get\n  operationId: MonitoringController_getMonitor_v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v2/monitors/{id}\n  method: delete\n  operationId: MonitoringController_stopMonitoring_v2\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/monitors/{id}/logs\n  method: get\n  operationId: MonitoringController_getMonitorLogs_v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/pricing\n  method: get\n  operationId: PricingController_getPricing_v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/search\n  method: get\n  operationId: SearchController_searchV2_v2\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/workspaces\n  method: get\n  operationId: WorkspaceController_listWorkspaces_v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/workspaces\n  method: post\n  operationId: WorkspaceController_createWorkspace_v2\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/workspaces/{name}\n  method: patch\n  operationId: WorkspaceController_updateWorkspace_v2\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/workspaces/{name}\n  method: delete\n  operationId: WorkspaceController_deleteWorkspace_v2\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/workspaces/usage\n  method: get\n  operationId: WorkspaceController_getUsageReport_v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/topograph/refs/heads/main/agentic-access/topograph-agentic-access.yml
summary_line: 22 operations · 9 acting · 9 human-in-the-loop
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
