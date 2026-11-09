---
acting_count: 0
action_class_counts:
  connected: 6
api_specs:
- filename: flight-mcp-com-flights-api-openapi.yml
  format: yaml
  label: flight-mcp-com Flights API
  slug: flight-mcp-com-flights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flight-mcp-com/openapi/flight-mcp-com-flights-api-openapi.yml
- filename: flight-mcp-com-healthz-api-openapi.yml
  format: yaml
  label: flight-mcp-com Healthz API
  slug: flight-mcp-com-healthz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flight-mcp-com/openapi/flight-mcp-com-healthz-api-openapi.yml
consequence_counts:
  read: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Flight Mcp Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'flight-mcp-com exposes 6 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: flight-mcp-com
provider_slug: flight-mcp-com
slug: flight-mcp-com-agentic-access
source_filename: flight-mcp-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/flight-mcp-com-openapi.json, openapi/flight-mcp-com-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 6\n  by_consequence:\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /healthz\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/flights/search\n  method: post\n  operationId: searchFlights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/flights/search/cached\n  method: post\n  operationId:\
  \ searchCachedFlights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /healthz\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/flights/search\n  method: post\n  operationId: searchFlights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/flights/search/cached\n  method: post\n  operationId: searchCachedFlights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/flight-mcp-com/agentic-access/flight-mcp-com-agentic-access.yml
summary_line: 6 operations
tags:
- Travel
- Flights
- MCP
- Search
---
