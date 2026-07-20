---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 4
api_specs:
- filename: allowance-openapi-original.json
  format: json
  label: Allowance API
  slug: allowance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allowance/refs/heads/main/openapi/allowance-openapi-original.json
consequence_counts:
  physical: 1
  read: 4
  safety-critical: 1
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Allowance Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /mandates/{id}/revoke
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /mandates/{id}/credential-requests
operation_count: 7
overview: 'Allowance exposes 7 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read, 1 write, 1 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Allowance
provider_slug: allowance
slug: allowance-agentic-access
source_filename: allowance-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: generated\nsource: openapi/allowance-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    acting: 3\n    connected: 4\n  by_consequence:\n    write: 1\n    read: 4\n    safety-critical: 1\n    physical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /mandates\n  method: post\n  operationId: createMandate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mandates/{id}\n  method: get\n  operationId: getMandate\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mandates/{id}/revoke\n  method: post\n  operationId: revokeMandate\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /mandates/{id}/credential-requests\n  method: post\n  operationId: requestCredential\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mandates/{id}/credential-requests/{cr_id}\n  method:\
  \ get\n  operationId: getCredentialRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pricing\n  method: get\n  operationId: getPricing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allowance/refs/heads/main/agentic-access/allowance-agentic-access.yml
summary_line: 7 operations · 3 acting · 1 human-in-the-loop
tags:
- Company
- Payments
- Agentic Payments
- AI Agents
- Virtual Cards
- Fintech
- Model Context Protocol
- Consumer Trust
- Spending Controls
- AP2
---
