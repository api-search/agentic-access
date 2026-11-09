---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 3
api_specs:
- filename: amnt-io-account-api-openapi.yml
  format: yaml
  label: AMNT Account API
  slug: amnt-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amnt-io/openapi/amnt-io-account-api-openapi.yml
- filename: amnt-io-agents-api-openapi.yml
  format: yaml
  label: AMNT Agents API
  slug: amnt-io-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amnt-io/openapi/amnt-io-agents-api-openapi.yml
- filename: amnt-io-runs-api-openapi.yml
  format: yaml
  label: AMNT Runs API
  slug: amnt-io-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amnt-io/openapi/amnt-io-runs-api-openapi.yml
- filename: amnt-io-svg-api-openapi.yml
  format: yaml
  label: AMNT SVG API
  slug: amnt-io-svg-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amnt-io/openapi/amnt-io-svg-api-openapi.yml
consequence_counts:
  read: 3
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Amnt Io Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'AMNT exposes 6 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AMNT
provider_slug: amnt-io
slug: amnt-io-agentic-access
source_filename: amnt-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/amnt-io-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    acting: 3\n    connected: 3\n  by_consequence:\n    write: 3\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/run\n  method: post\n  operationId: runAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agents\n  method: get\n  operationId: listAgents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agents/{handle}/{slug}\n  method: get\n  operationId: getAgent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/balance\n  method: get\n  operationId: getBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/svg/generate\n  method: post\n  operationId: svgGenerate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/svg/vectorize\n  method: post\n  operationId: svgVectorize\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/amnt-io/agentic-access/amnt-io-agentic-access.yml
summary_line: 6 operations · 3 acting
tags:
- Artificial Intelligence
- Tools
- Creators
- Developers
- Agents
---
