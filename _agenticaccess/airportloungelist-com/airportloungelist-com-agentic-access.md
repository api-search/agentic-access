---
acting_count: 0
action_class_counts:
  connected: 12
api_specs:
- filename: airportloungelist-com-access-api-openapi.yml
  format: yaml
  label: Airport Lounge List Access API
  slug: airportloungelist-com-access-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airportloungelist-com/openapi/airportloungelist-com-access-api-openapi.yml
- filename: airportloungelist-com-airports-api-openapi.yml
  format: yaml
  label: Airport Lounge List Airports API
  slug: airportloungelist-com-airports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airportloungelist-com/openapi/airportloungelist-com-airports-api-openapi.yml
- filename: airportloungelist-com-lounges-api-openapi.yml
  format: yaml
  label: Airport Lounge List Lounges API
  slug: airportloungelist-com-lounges-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airportloungelist-com/openapi/airportloungelist-com-lounges-api-openapi.yml
- filename: airportloungelist-com-networks-api-openapi.yml
  format: yaml
  label: Airport Lounge List Networks API
  slug: airportloungelist-com-networks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airportloungelist-com/openapi/airportloungelist-com-networks-api-openapi.yml
consequence_counts:
  read: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Airportloungelist Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Airport Lounge List exposes 12 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Airport Lounge List
provider_slug: airportloungelist-com
slug: airportloungelist-com-agentic-access
source_filename: airportloungelist-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/airportloungelist-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 12\n  by_consequence:\n    read: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /lounges/nearby\n  method: get\n  operationId: lounges_nearby\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lounges/search\n  method: get\n  operationId: lounges_search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lounges/{id}\n  method: get\n  operationId:\
  \ lounge_show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lounges/{slug}/reviews\n  method: get\n  operationId: lounge_reviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /airports\n  method: get\n  operationId: airports_index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /airports/nearby\n  method: get\n  operationId: airports_nearby\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /airports/{iata}\n  method: get\n  operationId: airport_show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n- path: /airports/{iata}/lounges\n  method: get\n  operationId: airport_lounges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /access\n  method: get\n  operationId: access_index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /access/{method}\n  method: get\n  operationId: access_show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /networks\n  method: get\n  operationId: networks_index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /networks/{slug}\n  method: get\n  operationId: network_show\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/airportloungelist-com/agentic-access/airportloungelist-com-agentic-access.yml
summary_line: 12 operations
tags:
- Airport
- Travel
- Lounge
- Aviation
- Comparison
- Company
---
