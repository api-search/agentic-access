---
acting_count: 0
action_class_counts:
  connected: 3
api_specs:
- filename: polygon-io-asyncapi.yml
  format: yaml
  label: Polygon.io Stocks API
  slug: stocks-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon-io/refs/heads/main/asyncapi/polygon-io-asyncapi.yml
- filename: polygon-io-asyncapi.yml
  format: yaml
  label: Polygon.io Options API
  slug: options-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon-io/refs/heads/main/asyncapi/polygon-io-asyncapi.yml
- filename: polygon-io-asyncapi.yml
  format: yaml
  label: Polygon.io Indices API
  slug: indices-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon-io/refs/heads/main/asyncapi/polygon-io-asyncapi.yml
- filename: polygon-io-asyncapi.yml
  format: yaml
  label: Polygon.io Forex API
  slug: forex-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon-io/refs/heads/main/asyncapi/polygon-io-asyncapi.yml
- filename: polygon-io-asyncapi.yml
  format: yaml
  label: Polygon.io Crypto API
  slug: crypto-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon-io/refs/heads/main/asyncapi/polygon-io-asyncapi.yml
- filename: polygon-io-asyncapi.yml
  format: yaml
  label: Polygon.io Futures API
  slug: futures-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon-io/refs/heads/main/asyncapi/polygon-io-asyncapi.yml
consequence_counts:
  read: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Polygon Io Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 3
overview: 'Polygon.io exposes 3 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Polygon.io
provider_slug: polygon-io
slug: polygon-io-agentic-access
source_filename: polygon-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/polygon-io-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 3\n  by_action_class:\n    connected: 3\n  by_consequence:\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/aggs/ticker/{stocksTicker}/range/{multiplier}/{timespan}/{from}/{to}\n  method: get\n  operationId: getAggregateBars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/reference/tickers\n  method: get\n  operationId: listTickers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v3/reference/tickers/{ticker}\n  method: get\n  operationId: getTickerDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polygon-io/refs/heads/main/agentic-access/polygon-io-agentic-access.yml
summary_line: 3 operations
tags:
- Fintech
- Market Data
- Stocks
- Options
- Forex
- Crypto
- Indices
- Futures
- WebSockets
- Real-time
- Historical
---
