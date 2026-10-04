---
acting_count: 0
action_class_counts:
  connected: 12
api_specs:
- filename: postfinder-io-nearby-api-openapi.yml
  format: yaml
  label: Postfinder Nearby API
  slug: postfinder-io-nearby-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postfinder-io/refs/heads/main/openapi/postfinder-io-nearby-api-openapi.yml
- filename: postfinder-io-places-api-openapi.yml
  format: yaml
  label: Postfinder Places API
  slug: postfinder-io-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postfinder-io/refs/heads/main/openapi/postfinder-io-places-api-openapi.yml
- filename: postfinder-io-postcodes-api-openapi.yml
  format: yaml
  label: Postfinder Postcodes API
  slug: postfinder-io-postcodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postfinder-io/refs/heads/main/openapi/postfinder-io-postcodes-api-openapi.yml
- filename: postfinder-io-reference-api-openapi.yml
  format: yaml
  label: Postfinder Reference API
  slug: postfinder-io-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postfinder-io/refs/heads/main/openapi/postfinder-io-reference-api-openapi.yml
- filename: postfinder-io-search-api-openapi.yml
  format: yaml
  label: Postfinder Search API
  slug: postfinder-io-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postfinder-io/refs/heads/main/openapi/postfinder-io-search-api-openapi.yml
consequence_counts:
  read: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Postfinder Io Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Postfinder exposes 12 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Postfinder
provider_slug: postfinder-io
slug: postfinder-io-agentic-access
source_filename: postfinder-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: generated\nsource: openapi/postfinder-io-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 12\n  by_consequence:\n    read: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/search\n  method: get\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/countries\n  method: get\n  operationId: countries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/countries/{country}\n  method: get\n  operationId: country\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/countries/{country}/regions/{region}\n  method: get\n  operationId: region\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/countries/{country}/categories/{category}\n  method: get\n  operationId: category\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/countries/{country}/postcodes\n  method: get\n  operationId: postcodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/countries/{country}/postcodes/{postcode}\n  method: get\n  operationId: postcodeDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/localities/{country}/{region}/{locality}\n  method: get\n  operationId: locality\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/places\n  method: get\n  operationId: places\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/places/{publicID}\n  method: get\n  operationId: place\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/nearby\n  method: get\n  operationId: nearby\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/openapi.json\n  method: get\n  operationId: openapi\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/postfinder-io/refs/heads/main/agentic-access/postfinder-io-agentic-access.yml
summary_line: 12 operations
tags:
- Company
- Address
- Autocomplete
- Logistics
- Australia
---
