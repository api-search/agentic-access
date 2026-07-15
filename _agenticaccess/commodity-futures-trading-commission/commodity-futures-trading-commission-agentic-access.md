---
acting_count: 0
action_class_counts:
  connected: 7
api_specs:
- filename: cftc-cot-openapi.yml
  format: yaml
  label: CFTC Commitments of Traders SODA API
  slug: cftc-cot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commodity-futures-trading-commission/refs/heads/main/openapi/cftc-cot-openapi.yml
consequence_counts:
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Commodity Futures Trading Commission Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Commodity Futures Trading Commission exposes 7 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Commodity Futures Trading Commission
provider_slug: commodity-futures-trading-commission
slug: commodity-futures-trading-commission-agentic-access
source_filename: commodity-futures-trading-commission-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/cftc-cot-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 7\n  by_consequence:\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /6dca-aqww.json\n  method: get\n  operationId: getLegacyFuturesOnly\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jun7-fc8e.json\n  method: get\n  operationId: getLegacyCombined\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /72hh-3qpy.json\n  method: get\n  operationId: getDisaggregatedFuturesOnly\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /kh3c-gbw2.json\n  method: get\n  operationId: getDisaggregatedCombined\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gpe5-46if.json\n  method: get\n  operationId: getTffFuturesOnly\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /yw9f-hn96.json\n  method: get\n  operationId: getTffCombined\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /4zgm-a668.json\n  method: get\n  operationId: getSupplementalCit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commodity-futures-trading-commission/refs/heads/main/agentic-access/commodity-futures-trading-commission-agentic-access.yml
summary_line: 7 operations
tags:
- CFTC
- Commitments of Traders
- Federal Government
- Financial
- Futures
- Open Data
- SODA
- Trading
---
