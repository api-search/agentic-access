---
acting_count: 0
action_class_counts:
  connected: 5
api_specs:
- filename: 1forge-forex-data-api.yml
  format: yaml
  label: 1Forge Forex Data API
  slug: 1forge-forex-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1forge/refs/heads/main/openapi/1forge-forex-data-api.yml
- filename: 1forge-forex-stream-asyncapi.yml
  format: yaml
  label: 1Forge Forex Stream
  slug: 1forge-forex-stream
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/1forge/refs/heads/main/asyncapi/1forge-forex-stream-asyncapi.yml
consequence_counts:
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: 1Forge Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: '1Forge exposes 5 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: 1Forge
provider_slug: 1forge
slug: 1forge-agentic-access
source_filename: 1forge-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/1forge-forex-data-api.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 5\n  by_consequence:\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /quotes\n  method: get\n  operationId: getQuotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /convert\n  method: get\n  operationId: convertCurrency\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /symbols\n  method: get\n  operationId: getSymbols\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /market_status\n  method: get\n  operationId: getMarketStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /quota\n  method: get\n  operationId: getQuota\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1forge/refs/heads/main/agentic-access/1forge-agentic-access.yml
summary_line: 5 operations
tags:
- Currency Exchange
- Forex
- Cryptocurrency
- Market Data
- Financial Data
- Real-Time Data
---
