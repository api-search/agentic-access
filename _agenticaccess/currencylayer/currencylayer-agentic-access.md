---
acting_count: 0
action_class_counts:
  connected: 6
api_specs:
- filename: currencylayer-openapi.yml
  format: yaml
  label: Currencylayer API
  slug: currencylayer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/currencylayer/refs/heads/main/openapi/currencylayer-openapi.yml
consequence_counts:
  read: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Currencylayer Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Currencylayer exposes 6 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Currencylayer
provider_slug: currencylayer
slug: currencylayer-agentic-access
source_filename: currencylayer-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/currencylayer-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 6\n  by_consequence:\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /list\n  method: get\n  operationId: listCurrencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /live\n  method: get\n  operationId: getLive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /historical\n  method: get\n  operationId: getHistorical\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /convert\n  method: get\n  operationId: convertCurrency\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /timeframe\n  method: get\n  operationId: getTimeFrame\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /change\n  method: get\n  operationId: getChange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/currencylayer/refs/heads/main/agentic-access/currencylayer-agentic-access.yml
summary_line: 6 operations
tags:
- Currency Exchange
- Foreign Exchange
- FX
- Forex
- Conversion
- Historical Rates
- Time Frame
- Change Report
- Precious Metals
- APILayer
- Public APIs
---
