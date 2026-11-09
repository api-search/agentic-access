---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 3
api_specs:
- filename: cityoftrees-house-agent-api-openapi.yml
  format: yaml
  label: City of Trees House Agent API
  slug: cityoftrees-house-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cityoftrees-house/openapi/cityoftrees-house-agent-api-openapi.yml
consequence_counts:
  read: 3
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cityoftrees House Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'City of Trees House exposes 4 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: City of Trees House
provider_slug: cityoftrees-house
slug: cityoftrees-house-agentic-access
source_filename: cityoftrees-house-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/cityoftrees-house-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    connected: 3\n    acting: 1\n  by_consequence:\n    read: 3\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/agent/v1/property\n  method: get\n  operationId: getProperty\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent/v1/availability\n  method: get\n  operationId: getAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent/v1/quotes\n\
  \  method: post\n  operationId: createQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agent/v1/quotes/{quoteId}\n  method: get\n  operationId: getQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/cityoftrees-house/agentic-access/cityoftrees-house-agentic-access.yml
summary_line: 4 operations · 1 acting
tags:
- Vacation Rentals
- West Sacramento
- Family Run
- Hospitality
- Vacation Home
---
