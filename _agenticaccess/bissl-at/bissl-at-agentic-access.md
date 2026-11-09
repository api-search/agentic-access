---
acting_count: 0
action_class_counts:
  connected: 4
api_specs:
- filename: bissl-at-dishes-api-openapi.yml
  format: yaml
  label: bissl-at Dishes API
  slug: bissl-at-dishes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bissl-at/openapi/bissl-at-dishes-api-openapi.yml
- filename: bissl-at-lunch-api-openapi.yml
  format: yaml
  label: bissl-at Lunch API
  slug: bissl-at-lunch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bissl-at/openapi/bissl-at-lunch-api-openapi.yml
- filename: bissl-at-venues-api-openapi.yml
  format: yaml
  label: bissl-at Venues API
  slug: bissl-at-venues-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bissl-at/openapi/bissl-at-venues-api-openapi.yml
consequence_counts:
  read: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bissl At Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'bissl-at exposes 4 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: bissl-at
provider_slug: bissl-at
slug: bissl-at-agentic-access
source_filename: bissl-at-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/bissl-at-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    connected: 4\n  by_consequence:\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/dishes\n  method: get\n  operationId: searchDishes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/lunch\n  method: get\n  operationId: findLunch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/venues\n  method: get\n  operationId: listVenues\n  x-agentic-access:\n  \
  \  action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/venues/{slug}\n  method: get\n  operationId: getVenue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/bissl-at/agentic-access/bissl-at-agentic-access.yml
summary_line: 4 operations
tags:
- Company
---
