---
acting_count: 0
action_class_counts:
  connected: 4
api_specs:
- filename: aplusz-app-cities-api-openapi.yml
  format: yaml
  label: aplusz-app Cities API
  slug: aplusz-app-cities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aplusz-app/openapi/aplusz-app-cities-api-openapi.yml
- filename: aplusz-app-fare-api-openapi.yml
  format: yaml
  label: aplusz-app Fare API
  slug: aplusz-app-fare-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aplusz-app/openapi/aplusz-app-fare-api-openapi.yml
- filename: aplusz-app-health-api-openapi.yml
  format: yaml
  label: aplusz-app Health API
  slug: aplusz-app-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aplusz-app/openapi/aplusz-app-health-api-openapi.yml
- filename: aplusz-app-routes-api-openapi.yml
  format: yaml
  label: aplusz-app Routes API
  slug: aplusz-app-routes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aplusz-app/openapi/aplusz-app-routes-api-openapi.yml
consequence_counts:
  read: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Aplusz App Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'aplusz-app exposes 4 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: aplusz-app
provider_slug: aplusz-app
slug: aplusz-app-agentic-access
source_filename: aplusz-app-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/aplusz-app-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    connected: 4\n  by_consequence:\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/fare\n  method: get\n  operationId: getFare\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/routes\n  method: get\n  operationId: listRoutes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cities\n  method: get\n  operationId: listCities\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/health\n  method: get\n  operationId: health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/aplusz-app/agentic-access/aplusz-app-agentic-access.yml
summary_line: 4 operations
tags:
- Company
- Travel
- Airfare
- Search
- Free
- Booking
---
