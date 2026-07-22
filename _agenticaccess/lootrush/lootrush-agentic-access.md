---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 3
api_specs:
- filename: lootrush-openapi-original.json
  format: json
  label: LootRush Partner API
  slug: lootrush-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lootrush/refs/heads/main/openapi/lootrush-openapi-original.json
consequence_counts:
  physical: 1
  read: 3
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Lootrush Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/crypto/{userId}/withdraw
operation_count: 5
overview: 'LootRush exposes 5 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read, 1 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: LootRush
provider_slug: lootrush
slug: lootrush-agentic-access
source_filename: lootrush-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/lootrush-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    acting: 2\n    connected: 3\n  by_consequence:\n    write: 1\n    physical: 1\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /mcp\n  method: post\n  operationId: callMcpTool\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/crypto/{userId}/withdraw\n  method: post\n  operationId: createWithdrawal\n  x-agentic-access:\n  \
  \  action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/crypto/{userId}/withdraws\n  method: get\n  operationId: listWithdrawals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/history\n  method: get\n  operationId: getUserHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/consent/{consentId}/user\n  method: get\n  operationId: getConsentUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lootrush/refs/heads/main/agentic-access/lootrush-agentic-access.yml
summary_line: 5 operations · 2 acting
tags:
- Company
- Gaming
- Crypto
- Cryptocurrency
- Payments
- Withdrawals
- MCP
- API
---
