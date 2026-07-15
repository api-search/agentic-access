---
acting_count: 0
action_class_counts:
  connected: 9
api_specs:
- filename: country-state-city-api-openapi.yml
  format: yaml
  label: Country State City API
  slug: country-state-city-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/country-state-city-api/refs/heads/main/openapi/country-state-city-api-openapi.yml
consequence_counts:
  read: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Country State City Api Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Country State City API exposes 9 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Country State City API
provider_slug: country-state-city-api
slug: country-state-city-api-agentic-access
source_filename: country-state-city-api-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/country-state-city-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 9\n  by_consequence:\n    read: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /countries\n  method: get\n  operationId: listCountries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /countries/{ciso}\n  method: get\n  operationId: getCountry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /countries/{ciso}/states\n  method: get\n  operationId:\
  \ listStatesByCountry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /countries/{ciso}/states/{siso}\n  method: get\n  operationId: getStateByCountryAndCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /countries/{ciso}/states/{siso}/cities\n  method: get\n  operationId: listCitiesByCountryAndState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /countries/{ciso}/cities\n  method: get\n  operationId: listCitiesByCountry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /states\n  method: get\n  operationId: listStates\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /states/{sid}/cities\n  method: get\n  operationId: listCitiesByState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cities\n  method: get\n  operationId: listCities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/country-state-city-api/refs/heads/main/agentic-access/country-state-city-api-agentic-access.yml
summary_line: 9 operations
tags:
- Capitals
- Cities
- Countries
- Currencies
- Geography
- Geolocation
- ISO 3166
- JSON
- Phone Codes
- Provinces
- Reference Data
- Regions
- States
- Time Zones
---
