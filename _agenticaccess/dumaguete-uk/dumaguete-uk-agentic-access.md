---
acting_count: 0
action_class_counts:
  connected: 8
api_specs:
- filename: dumaguete-uk-categories-api-openapi.yml
  format: yaml
  label: Dumaguete.uk Categories API
  slug: dumaguete-uk-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dumaguete-uk/openapi/dumaguete-uk-categories-api-openapi.yml
- filename: dumaguete-uk-cities-api-openapi.yml
  format: yaml
  label: Dumaguete.uk Cities API
  slug: dumaguete-uk-cities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dumaguete-uk/openapi/dumaguete-uk-cities-api-openapi.yml
- filename: dumaguete-uk-oembed-api-openapi.yml
  format: yaml
  label: Dumaguete.uk Oembed API
  slug: dumaguete-uk-oembed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dumaguete-uk/openapi/dumaguete-uk-oembed-api-openapi.yml
- filename: dumaguete-uk-place-api-openapi.yml
  format: yaml
  label: Dumaguete.uk Place API
  slug: dumaguete-uk-place-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dumaguete-uk/openapi/dumaguete-uk-place-api-openapi.yml
- filename: dumaguete-uk-places-api-openapi.yml
  format: yaml
  label: Dumaguete.uk Places API
  slug: dumaguete-uk-places-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dumaguete-uk/openapi/dumaguete-uk-places-api-openapi.yml
- filename: dumaguete-uk-search-api-openapi.yml
  format: yaml
  label: Dumaguete.uk Search API
  slug: dumaguete-uk-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dumaguete-uk/openapi/dumaguete-uk-search-api-openapi.yml
- filename: dumaguete-uk-stats-api-openapi.yml
  format: yaml
  label: Dumaguete.uk Stats API
  slug: dumaguete-uk-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dumaguete-uk/openapi/dumaguete-uk-stats-api-openapi.yml
- filename: dumaguete-uk-status-json-api-openapi.yml
  format: yaml
  label: Dumaguete.uk Status.json API
  slug: dumaguete-uk-status-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dumaguete-uk/openapi/dumaguete-uk-status-json-api-openapi.yml
consequence_counts:
  read: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Dumaguete Uk Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Dumaguete.uk exposes 8 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Dumaguete.uk
provider_slug: dumaguete-uk
slug: dumaguete-uk-agentic-access
source_filename: dumaguete-uk-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: generated\nsource: openapi/dumaguete-uk-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 8\n  by_consequence:\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/places\n  method: get\n  operationId: listPlaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/place\n  method: get\n  operationId: getPlace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/search\n  method: get\n  operationId: searchPlaces\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/categories\n  method: get\n  operationId: listCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cities\n  method: get\n  operationId: listCities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stats\n  method: get\n  operationId: siteStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/oembed\n  method: get\n  operationId: oembed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status.json\n  method: get\n  operationId:\
  \ status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/dumaguete-uk/agentic-access/dumaguete-uk-agentic-access.yml
summary_line: 8 operations
tags:
- City Guide
- Philippines
- Relocation
- Cost of Living
- Healthcare
---
