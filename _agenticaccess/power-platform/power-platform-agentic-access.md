---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 8
api_specs:
- filename: v1
  format: yaml
  label: Power Apps API
  slug: power-apps-api
  spec_type: OpenAPI
  url: https://api.powerapps.com/openapi/v1
- filename: v1
  format: yaml
  label: Power Automate API
  slug: power-automate-api
  spec_type: OpenAPI
  url: https://api.flow.microsoft.com/openapi/v1
- filename: swagger.json
  format: json
  label: Power BI REST API
  slug: power-bi-rest-api
  spec_type: OpenAPI
  url: https://api.powerbi.com/v1.0/myorg/swagger.json
- filename: power-platform-api-openapi.json
  format: json
  label: Power Platform Unified API
  slug: power-platform-unified-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/power-platform/refs/heads/main/openapi/power-platform-api-openapi.json
consequence_counts:
  read: 8
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Power Platform Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'Microsoft Power Platform APIs exposes 13 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Microsoft Power Platform APIs
provider_slug: power-platform
slug: power-platform-agentic-access
source_filename: power-platform-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/power-platform-api-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 8\n    acting: 5\n  by_consequence:\n    read: 8\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /providers/Microsoft.BusinessAppPlatform/scopes/admin/environments\n  method: get\n  operationId: listEnvironments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /providers/Microsoft.BusinessAppPlatform/scopes/admin/environments/{environmentId}\n  method: get\n  operationId: getEnvironment\n  x-agentic-access:\n    action-class: connected\n   \
  \ consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /providers/Microsoft.BusinessAppPlatform/scopes/admin/environments/{environmentId}\n  method: delete\n  operationId: deleteEnvironment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /appmanagement/environments/{environmentId}/applicationPackages\n  method: get\n  operationId: getEnvironmentApplicationPackages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /appmanagement/environments/{environmentId}/applicationPackages/{applicationPackageId}/install\n  method: post\n  operationId: installApplicationPackage\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /appmanagement/environments/{environmentId}/operations/{operationId}\n  method: get\n  operationId: getApplicationPackageInstallStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /appmanagement/applicationPackages\n  method: get\n  operationId: getTenantApplicationPackages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /powerautomate/environments/{environmentId}/flowRuns\n  method: get\n  operationId: listFlowRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n- path: /licensing/billingPolicies\n  method: get\n  operationId: listBillingPolicies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /licensing/billingPolicies\n  method: post\n  operationId: createBillingPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /licensing/billingPolicies/{billingPolicyId}\n  method: get\n  operationId: getBillingPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /licensing/billingPolicies/{billingPolicyId}\n  method: patch\n  operationId: updateBillingPolicy\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /licensing/billingPolicies/{billingPolicyId}\n  method: delete\n  operationId: deleteBillingPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/power-platform/refs/heads/main/agentic-access/power-platform-agentic-access.yml
summary_line: 13 operations · 5 acting
tags:
- Business Applications
- Copilot Studio
- Dataverse
- Low-Code
- Microsoft
- No-Code
- Power Pages
- Power Platform
---
