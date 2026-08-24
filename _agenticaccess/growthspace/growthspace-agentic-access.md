---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 6
api_specs:
- filename: growthspace-public-api-management-openapi-original.yml
  format: yaml
  label: Growthspace Public API Management
  slug: growthspace-public-api-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/growthspace/refs/heads/main/openapi/growthspace-public-api-management-openapi-original.yml
consequence_counts:
  read: 6
  safety-critical: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 6
kind: agentic-access
layout: agentic-access
method: generated
name: Growthspace Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /admin/apps
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /admin/apps/{appId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /admin/apps/{appId}/refresh
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /admin/apps/{appId}/scopes
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /admin/apps/{appId}/token
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /public/refresh
operation_count: 12
overview: 'GrowthSpace exposes 12 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 6 safety-critical.


  6 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: GrowthSpace
provider_slug: growthspace
slug: growthspace-agentic-access
source_filename: growthspace-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: generated\nsource: openapi/growthspace-public-api-management-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 6\n    acting: 6\n  by_consequence:\n    read: 6\n    safety-critical: 6\n  human_in_the_loop_required: 6\noperations:\n- path: /\n  method: get\n  operationId: AppController_microserviceInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /up-time-check\n  method: get\n  operationId: AppController_upTimeCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /_ah/warmup\n  method: get\n  operationId: AppController_warmupRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /healthz\n  method: get\n  operationId: AppController_healthz\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/scopes\n  method: get\n  operationId: AppsManagementController_getScopes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/apps\n  method: post\n  operationId: AppsManagementController_createApp\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /admin/apps\n  method: get\n  operationId: AppsManagementController_listApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/apps/{appId}/token\n  method: post\n  operationId: AppsManagementController_generateToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /admin/apps/{appId}\n  method: delete\n  operationId: AppsManagementController_revokeApp\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange:\
  \ true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /admin/apps/{appId}/scopes\n  method: put\n  operationId: AppsManagementController_updateScopes\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /admin/apps/{appId}/refresh\n  method: post\n  operationId: AppsManagementController_refreshForApp\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public/refresh\n\
  \  method: post\n  operationId: AppsManagementController_publicRefresh\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/growthspace/refs/heads/main/agentic-access/growthspace-agentic-access.yml
summary_line: 12 operations · 6 acting · 6 human-in-the-loop
tags:
- Company
- Learning and Development
- Talent Development
- Human Resources
- Coaching
- Employee Experience
- Skills
- Workforce
- Enterprise Software
- Artificial Intelligence
---
