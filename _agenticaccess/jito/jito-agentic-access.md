---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 1
api_specs:
- filename: jito-block-engine-openapi.yml
  format: yaml
  label: Jito Block Engine JSON-RPC API
  slug: jito-block-engine
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jito/refs/heads/main/openapi/jito-block-engine-openapi.yml
- filename: jito-bundles-tip-floor-openapi.yml
  format: yaml
  label: Jito Bundles Tip Floor API
  slug: jito-bundles-tip-floor
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jito/refs/heads/main/openapi/jito-bundles-tip-floor-openapi.yml
- filename: jito-streaming-asyncapi.yml
  format: yaml
  label: Jito Streaming Surfaces
  slug: jito-streaming
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/jito/refs/heads/main/asyncapi/jito-streaming-asyncapi.yml
consequence_counts:
  physical: 1
  read: 1
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Jito Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/transactions
operation_count: 3
overview: 'Jito Labs exposes 3 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read, 1 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Jito Labs
provider_slug: jito
slug: jito-agentic-access
source_filename: jito-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/jito-block-engine-openapi.yml, openapi/jito-bundles-tip-floor-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 3\n  by_action_class:\n    acting: 2\n    connected: 1\n  by_consequence:\n    write: 1\n    physical: 1\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/bundles\n  method: post\n  operationId: bundlesRpc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/transactions\n  method: post\n  operationId:\
  \ transactionsRpc\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/bundles/tip_floor\n  method: get\n  operationId: getTipFloor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jito/refs/heads/main/agentic-access/jito-agentic-access.yml
summary_line: 3 operations · 2 acting
tags:
- Solana
- MEV
- Block Engine
- Bundles
- Liquid Staking
- JitoSOL
- Restaking
- JTO
- DAO
- Validator
- Searcher
- ShredStream
- Crypto
- DeFi
---
