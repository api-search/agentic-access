---
acting_count: 0
action_class_counts:
  connected: 7
api_specs:
- filename: deadends-dev-countries-json-api-openapi.yml
  format: yaml
  label: deadends.dev Countries.json API
  slug: deadends-dev-countries-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deadends-dev/openapi/deadends-dev-countries-json-api-openapi.yml
- filename: deadends-dev-country-api-openapi.yml
  format: yaml
  label: deadends.dev Country API
  slug: deadends-dev-country-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deadends-dev/openapi/deadends-dev-country-api-openapi.yml
- filename: deadends-dev-deadends-dev-api-api-openapi.yml
  format: yaml
  label: deadends.dev Deadends.dev API
  slug: deadends-dev-deadends-dev-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deadends-dev/openapi/deadends-dev-deadends-dev-api-api-openapi.yml
- filename: deadends-dev-errors-ndjson-api-openapi.yml
  format: yaml
  label: deadends.dev Errors.ndjson API
  slug: deadends-dev-errors-ndjson-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deadends-dev/openapi/deadends-dev-errors-ndjson-api-openapi.yml
- filename: deadends-dev-index-json-api-openapi.yml
  format: yaml
  label: deadends.dev Index.json API
  slug: deadends-dev-index-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deadends-dev/openapi/deadends-dev-index-json-api-openapi.yml
- filename: deadends-dev-match-json-api-openapi.yml
  format: yaml
  label: deadends.dev Match.json API
  slug: deadends-dev-match-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deadends-dev/openapi/deadends-dev-match-json-api-openapi.yml
- filename: deadends-dev-stats-json-api-openapi.yml
  format: yaml
  label: deadends.dev Stats.json API
  slug: deadends-dev-stats-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deadends-dev/openapi/deadends-dev-stats-json-api-openapi.yml
consequence_counts:
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Deadends Dev Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'deadends.dev exposes 7 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: deadends.dev
provider_slug: deadends-dev
slug: deadends-dev-agentic-access
source_filename: deadends-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/deadends-dev-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 7\n  by_consequence:\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /index.json\n  method: get\n  operationId: listErrors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /match.json\n  method: get\n  operationId: matchErrors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats.json\n  method: get\n  operationId: getStats\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /errors.ndjson\n  method: get\n  operationId: streamErrors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{domain}/{slug}/{env}.json\n  method: get\n  operationId: getErrorCanon\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/countries.json\n  method: get\n  operationId: listCountries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/country/{country}.json\n  method: get\n  operationId: getCountryAggregate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/deadends-dev/agentic-access/deadends-dev-agentic-access.yml
summary_line: 7 operations
tags:
- Error Database
- Debugging
- Open Source
---
