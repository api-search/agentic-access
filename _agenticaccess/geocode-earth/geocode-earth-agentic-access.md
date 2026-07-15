---
acting_count: 0
action_class_counts:
  connected: 5
api_specs:
- filename: geocode-earth-openapi.yml
  format: yaml
  label: Geocode Earth Search API
  slug: search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geocode-earth/refs/heads/main/openapi/geocode-earth-openapi.yml
- filename: geocode-earth-openapi.yml
  format: yaml
  label: Geocode Earth Autocomplete API
  slug: autocomplete
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geocode-earth/refs/heads/main/openapi/geocode-earth-openapi.yml
- filename: geocode-earth-openapi.yml
  format: yaml
  label: Geocode Earth Reverse API
  slug: reverse
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geocode-earth/refs/heads/main/openapi/geocode-earth-openapi.yml
- filename: geocode-earth-openapi.yml
  format: yaml
  label: Geocode Earth Structured Search API
  slug: structured-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geocode-earth/refs/heads/main/openapi/geocode-earth-openapi.yml
- filename: geocode-earth-openapi.yml
  format: yaml
  label: Geocode Earth Place API
  slug: place
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geocode-earth/refs/heads/main/openapi/geocode-earth-openapi.yml
consequence_counts:
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Geocode Earth Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Geocode Earth exposes 5 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Geocode Earth
provider_slug: geocode-earth
slug: geocode-earth-agentic-access
source_filename: geocode-earth-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/geocode-earth-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 5\n  by_consequence:\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /search\n  method: get\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autocomplete\n  method: get\n  operationId: autocomplete\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reverse\n  method: get\n  operationId: reverse\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/structured\n  method: get\n  operationId: searchStructured\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /place\n  method: get\n  operationId: place\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geocode-earth/refs/heads/main/agentic-access/geocode-earth-agentic-access.yml
summary_line: 5 operations
tags:
- Geocoding
- Address Autocomplete
- Reverse Geocoding
- Mapping
- Pelias
- Open Data
---
