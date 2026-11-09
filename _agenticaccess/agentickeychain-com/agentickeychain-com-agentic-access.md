---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 5
api_specs:
- filename: agentickeychain-com-capabilities-api-openapi.yml
  format: yaml
  label: Agentic Keychain Capabilities API
  slug: agentickeychain-com-capabilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentickeychain-com/openapi/agentickeychain-com-capabilities-api-openapi.yml
- filename: agentickeychain-com-compare-api-openapi.yml
  format: yaml
  label: Agentic Keychain Compare API
  slug: agentickeychain-com-compare-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentickeychain-com/openapi/agentickeychain-com-compare-api-openapi.yml
- filename: agentickeychain-com-evaluate-api-openapi.yml
  format: yaml
  label: Agentic Keychain Evaluate API
  slug: agentickeychain-com-evaluate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentickeychain-com/openapi/agentickeychain-com-evaluate-api-openapi.yml
- filename: agentickeychain-com-outcome-api-openapi.yml
  format: yaml
  label: Agentic Keychain Outcome API
  slug: agentickeychain-com-outcome-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentickeychain-com/openapi/agentickeychain-com-outcome-api-openapi.yml
- filename: agentickeychain-com-quote-api-openapi.yml
  format: yaml
  label: Agentic Keychain Quote API
  slug: agentickeychain-com-quote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentickeychain-com/openapi/agentickeychain-com-quote-api-openapi.yml
- filename: agentickeychain-com-resolve-api-openapi.yml
  format: yaml
  label: Agentic Keychain Resolve API
  slug: agentickeychain-com-resolve-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentickeychain-com/openapi/agentickeychain-com-resolve-api-openapi.yml
- filename: agentickeychain-com-roi-api-openapi.yml
  format: yaml
  label: Agentic Keychain Roi API
  slug: agentickeychain-com-roi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentickeychain-com/openapi/agentickeychain-com-roi-api-openapi.yml
- filename: agentickeychain-com-unlock-api-openapi.yml
  format: yaml
  label: Agentic Keychain Unlock API
  slug: agentickeychain-com-unlock-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentickeychain-com/openapi/agentickeychain-com-unlock-api-openapi.yml
consequence_counts:
  physical: 1
  read: 5
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Agentickeychain Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/unlock
operation_count: 11
overview: 'Agentic Keychain exposes 11 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read, 5 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Agentic Keychain
provider_slug: agentickeychain-com
slug: agentickeychain-com-agentic-access
source_filename: agentickeychain-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/agentickeychain-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 5\n    acting: 6\n  by_consequence:\n    read: 5\n    write: 5\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/capabilities/search\n  method: get\n  operationId: search_capabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/capabilities/{capability}\n  method: get\n  operationId: get_capability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/capabilities/{capability}/benchmark\n  method: get\n  operationId: get_benchmark\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/capabilities/{capability}/provenance\n  method: get\n  operationId: get_provenance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/compare\n  method: post\n  operationId: compare_capabilities\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/evaluate\n  method: post\n  operationId: evaluate_capability\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n   \
  \ subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/outcome\n  method: post\n  operationId: report_outcome\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/quote\n  method: post\n  operationId: get_quote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/resolve\n  method: post\n  operationId: resolve_task\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/roi\n  method: post\n  operationId: estimate_roi\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/unlock\n  method: post\n  operationId: unlock_capability\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/agentickeychain-com/agentic-access/agentickeychain-com-agentic-access.yml
summary_line: 11 operations · 6 acting
tags:
- Autonomous Trading
- Blockchain
- Finance
- Solana
- Base
---
