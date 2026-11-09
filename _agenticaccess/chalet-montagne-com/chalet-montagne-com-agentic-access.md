---
acting_count: 0
action_class_counts:
  connected: 7
api_specs:
- filename: chalet-montagne-com-public-front-api-openapi.yml
  format: yaml
  label: Chalet Montagne Public Front API
  slug: chalet-montagne-com-public-front-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chalet-montagne-com/openapi/chalet-montagne-com-public-front-api-openapi.yml
consequence_counts:
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Chalet Montagne Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Chalet Montagne exposes 7 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Chalet Montagne
provider_slug: chalet-montagne-com
slug: chalet-montagne-com-agentic-access
source_filename: chalet-montagne-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/chalet-montagne-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 7\n  by_consequence:\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /api/public-front/search\n  method: get\n  operationId: searchRentals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/public-front/search/filters\n  method: get\n  operationId: getSearchFilters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/public-front/destinations\n\
  \  method: get\n  operationId: getDestinations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/public-front/hostings/{hostingId}/home\n  method: get\n  operationId: getRentalDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/public-front/hostings/{hostingId}/availability\n  method: get\n  operationId: getAvailabilityCalendar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/public-front/calculate-price\n  method: get\n  operationId: calculateStayPrice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/public-front/planning-coverage\n  method: get\n\
  \  operationId: checkPlanningCoverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/chalet-montagne-com/agentic-access/chalet-montagne-com-agentic-access.yml
summary_line: 7 operations
tags:
- Vacation Rentals
- France
- Mountain
- Travel
- Accommodation
---
