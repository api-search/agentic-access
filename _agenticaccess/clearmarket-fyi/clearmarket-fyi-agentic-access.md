---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 11
api_specs:
- filename: clearmarket-fyi-catalysts-api-openapi.yml
  format: yaml
  label: ClearMarket Catalysts API
  slug: clearmarket-fyi-catalysts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearmarket-fyi/openapi/clearmarket-fyi-catalysts-api-openapi.yml
- filename: clearmarket-fyi-clearmarket-api-api-openapi.yml
  format: yaml
  label: ClearMarket ClearMarket API
  slug: clearmarket-fyi-clearmarket-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearmarket-fyi/openapi/clearmarket-fyi-clearmarket-api-api-openapi.yml
- filename: clearmarket-fyi-events-api-openapi.yml
  format: yaml
  label: ClearMarket Events API
  slug: clearmarket-fyi-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearmarket-fyi/openapi/clearmarket-fyi-events-api-openapi.yml
- filename: clearmarket-fyi-keys-api-openapi.yml
  format: yaml
  label: ClearMarket Keys API
  slug: clearmarket-fyi-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearmarket-fyi/openapi/clearmarket-fyi-keys-api-openapi.yml
- filename: clearmarket-fyi-markets-api-openapi.yml
  format: yaml
  label: ClearMarket Markets API
  slug: clearmarket-fyi-markets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearmarket-fyi/openapi/clearmarket-fyi-markets-api-openapi.yml
- filename: clearmarket-fyi-marks-api-openapi.yml
  format: yaml
  label: ClearMarket Marks API
  slug: clearmarket-fyi-marks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearmarket-fyi/openapi/clearmarket-fyi-marks-api-openapi.yml
- filename: clearmarket-fyi-signals-api-openapi.yml
  format: yaml
  label: ClearMarket Signals API
  slug: clearmarket-fyi-signals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearmarket-fyi/openapi/clearmarket-fyi-signals-api-openapi.yml
- filename: clearmarket-fyi-spot-api-openapi.yml
  format: yaml
  label: ClearMarket Spot API
  slug: clearmarket-fyi-spot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearmarket-fyi/openapi/clearmarket-fyi-spot-api-openapi.yml
- filename: clearmarket-fyi-status-api-openapi.yml
  format: yaml
  label: ClearMarket Status API
  slug: clearmarket-fyi-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearmarket-fyi/openapi/clearmarket-fyi-status-api-openapi.yml
consequence_counts:
  read: 11
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Clearmarket Fyi Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'ClearMarket exposes 12 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ClearMarket
provider_slug: clearmarket-fyi
slug: clearmarket-fyi-agentic-access
source_filename: clearmarket-fyi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/clearmarket-fyi-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 11\n    acting: 1\n  by_consequence:\n    read: 11\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: serviceInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/events\n  method: get\n  operationId: listEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/events/{slug}\n  method: get\n  operationId:\
  \ getEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/markets/{id}\n  method: get\n  operationId: getMarket\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/marks\n  method: get\n  operationId: listMarks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/status\n  method: get\n  operationId: feedStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/markets/movers\n  method: get\n  operationId: listMovers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/catalysts/upcoming\n  method: get\n  operationId: listUpcomingCatalysts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/signals\n  method: get\n  operationId: listSignals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/signals/{slug}\n  method: get\n  operationId: getSignal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/spot\n  method: get\n  operationId: getSpot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/keys\n  method: post\n  operationId: createKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/clearmarket-fyi/agentic-access/clearmarket-fyi-agentic-access.yml
summary_line: 12 operations · 1 acting
tags:
- Prediction Markets
- Market Data API
- Signal Feed
- Daily Wire
- Market Intelligence
---
