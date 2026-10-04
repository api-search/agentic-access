---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 2
api_specs:
- filename: saviynt-analytics-api-openapi.yml
  format: yaml
  label: Saviynt Analytics API
  slug: saviynt-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saviynt/refs/heads/main/openapi/saviynt-analytics-api-openapi.yml
consequence_counts:
  read: 2
  safety-critical: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 6
kind: agentic-access
layout: agentic-access
method: generated
name: Saviynt Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /fetchControlAttributes
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /fetchControlDetails
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /fetchControlDetailsES
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /fetchControlList
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /fetchControlListES
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /runAnalyticsControls
operation_count: 8
overview: 'Saviynt exposes 8 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 6 safety-critical.


  6 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Saviynt
provider_slug: saviynt
slug: saviynt-agentic-access
source_filename: saviynt-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/saviynt-analytics-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 6\n    connected: 2\n  by_consequence:\n    safety-critical: 6\n    read: 2\n  human_in_the_loop_required: 6\noperations:\n- path: /fetchControlList\n  method: post\n  operationId: fetchControlList\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /fetchControlDetails\n  method: post\n  operationId:\
  \ fetchControlDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /runAnalyticsControls\n  method: post\n  operationId: runAnalyticsControls\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /fetchRuntimeControlsData\n  method: post\n  operationId: fetchRuntimeControlsData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fetchRuntimeControlsDataV2\n\
  \  method: post\n  operationId: fetchRuntimeControlsDataV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fetchControlAttributes\n  method: post\n  operationId: fetchControlAttributes\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /fetchControlListES\n  method: post\n  operationId: fetchControlListES\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n\
  - path: /fetchControlDetailsES\n  method: post\n  operationId: fetchControlDetailsES\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/saviynt/refs/heads/main/agentic-access/saviynt-agentic-access.yml
summary_line: 8 operations · 6 acting · 6 human-in-the-loop
tags:
- Identity Governance
- Identity Administration
- Access Management
- Privileged Access Management
- Segregation of Duties
- IGA
- Security
---
