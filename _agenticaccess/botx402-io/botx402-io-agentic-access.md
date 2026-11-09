---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 2
api_specs:
- filename: botx402-io-agent-api-openapi.yml
  format: yaml
  label: BotX402 Agent API
  slug: botx402-io-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botx402-io/openapi/botx402-io-agent-api-openapi.yml
- filename: botx402-io-base-address-balance-api-openapi.yml
  format: yaml
  label: BotX402 Base Address Balance API
  slug: botx402-io-base-address-balance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botx402-io/openapi/botx402-io-base-address-balance-api-openapi.yml
- filename: botx402-io-well-known-api-openapi.yml
  format: yaml
  label: BotX402 .well Known API
  slug: botx402-io-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botx402-io/openapi/botx402-io-well-known-api-openapi.yml
consequence_counts:
  read: 2
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Botx402 Io Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 3
overview: 'BotX402 exposes 3 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BotX402
provider_slug: botx402-io
slug: botx402-io-agentic-access
source_filename: botx402-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/botx402-io-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 3\n  by_action_class:\n    connected: 2\n    acting: 1\n  by_consequence:\n    read: 2\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /.well-known/x402\n  method: get\n  operationId: x402Manifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agent/bots\n  method: get\n  operationId: listBots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /base-address-balance\n  method:\
  \ post\n  operationId: base_address_balance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/botx402-io/agentic-access/botx402-io-agentic-access.yml
summary_line: 3 operations · 1 acting
tags:
- Company
- Pay-Per-Use
- Bots
- Business
- Automation
- SaaS-alternative
---
