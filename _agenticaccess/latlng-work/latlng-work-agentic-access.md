---
acting_count: 0
action_class_counts:
  connected: 4
api_specs:
- filename: latlng-work-geocoding-api-openapi.yml
  format: yaml
  label: latlng-work Geocoding API
  slug: latlng-work-geocoding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/latlng-work/openapi/latlng-work-geocoding-api-openapi.yml
- filename: latlng-work-places-api-openapi.yml
  format: yaml
  label: latlng-work Places API
  slug: latlng-work-places-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/latlng-work/openapi/latlng-work-places-api-openapi.yml
consequence_counts:
  read: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Latlng Work Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'latlng-work exposes 4 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: latlng-work
provider_slug: latlng-work
slug: latlng-work-agentic-access
source_filename: latlng-work-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/latlng-work-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    connected: 4\n  by_consequence:\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /api\n  method: get\n  operationId: forwardGeocode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reverse\n  method: get\n  operationId: reverseGeocode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/places/nearby\n  method: get\n  operationId: placesNearby\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/places/search\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/latlng-work/agentic-access/latlng-work-agentic-access.yml
summary_line: 4 operations
tags:
- Company
- Geocoding
- Mapping
- Location
---
