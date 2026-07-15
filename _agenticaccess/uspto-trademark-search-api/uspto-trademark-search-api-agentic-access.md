---
acting_count: 0
action_class_counts:
  connected: 5
api_specs:
- filename: uspto-trademark-search-api-openapi.yml
  format: yaml
  label: USPTO Trademark Search API Endpoints
  slug: uspto-trademark-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-trademark-search-api/refs/heads/main/openapi/uspto-trademark-search-api-openapi.yml
consequence_counts:
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Uspto Trademark Search Api Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'USPTO Trademark Search API exposes 5 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: USPTO Trademark Search API
provider_slug: uspto-trademark-search-api
slug: uspto-trademark-search-api-agentic-access
source_filename: uspto-trademark-search-api-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/uspto-trademark-search-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 5\n  by_consequence:\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/trademarkSearch/{keyword}/{searchType}\n  method: get\n  operationId: searchTrademarks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/trademarkAvailable/{keyword}\n  method: get\n  operationId: checkTrademarkAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/trademarkBySerial/{serialNumber}\n  method: get\n  operationId: getTrademarkBySerialNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/trademarkOwner/{owner}\n  method: get\n  operationId: searchTrademarksByOwner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/databaseStatus\n  method: get\n  operationId: getDatabaseStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uspto-trademark-search-api/refs/heads/main/agentic-access/uspto-trademark-search-api-agentic-access.yml
summary_line: 5 operations
tags:
- Brand
- Brand Protection
- Business
- Data
- Government Data
- Intellectual Property
- Legal
- Search
- Trademark
- USPTO
---
