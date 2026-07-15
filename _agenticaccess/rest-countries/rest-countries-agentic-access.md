---
acting_count: 0
action_class_counts:
  connected: 12
api_specs:
- filename: rest-countries-openapi.yml
  format: yaml
  label: REST Countries
  slug: rest-countries
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rest-countries/refs/heads/main/openapi/rest-countries-openapi.yml
consequence_counts:
  read: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Rest Countries Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'REST Countries exposes 12 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: REST Countries
provider_slug: rest-countries
slug: rest-countries-agentic-access
source_filename: rest-countries-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/rest-countries-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 12\n  by_consequence:\n    read: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /all\n  method: get\n  operationId: listAllCountries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /name/{name}\n  method: get\n  operationId: getCountriesByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /alpha/{code}\n  method: get\n  operationId: getCountryByAlphaCode\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /alpha\n  method: get\n  operationId: getCountriesByAlphaCodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /currency/{currency}\n  method: get\n  operationId: getCountriesByCurrency\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lang/{language}\n  method: get\n  operationId: getCountriesByLanguage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /capital/{capital}\n  method: get\n  operationId: getCountriesByCapital\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n \
  \   token:\n      max-ttl: 3600\n    audit: none\n- path: /region/{region}\n  method: get\n  operationId: getCountriesByRegion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subregion/{subregion}\n  method: get\n  operationId: getCountriesBySubregion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /translation/{translation}\n  method: get\n  operationId: getCountriesByTranslation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /demonym/{demonym}\n  method: get\n  operationId: getCountriesByDemonym\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /independent\n  method:\
  \ get\n  operationId: listIndependentCountries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rest-countries/refs/heads/main/agentic-access/rest-countries-agentic-access.yml
summary_line: 12 operations
tags:
- Countries
- Geocoding
- Geography
- ISO 3166
- Open Source
- Public APIs
- Reference Data
- Currencies
- Languages
- Capitals
- Regions
- Subregions
- Translations
---
