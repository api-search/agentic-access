---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 4
api_specs:
- filename: antalyatransfers-co-fx-api-openapi.yml
  format: yaml
  label: AntalyaTransfers.co Fx API
  slug: antalyatransfers-co-fx-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antalyatransfers-co/openapi/antalyatransfers-co-fx-api-openapi.yml
- filename: antalyatransfers-co-locations-api-openapi.yml
  format: yaml
  label: AntalyaTransfers.co Locations API
  slug: antalyatransfers-co-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antalyatransfers-co/openapi/antalyatransfers-co-locations-api-openapi.yml
- filename: antalyatransfers-co-pricing-api-openapi.yml
  format: yaml
  label: AntalyaTransfers.co Pricing API
  slug: antalyatransfers-co-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antalyatransfers-co/openapi/antalyatransfers-co-pricing-api-openapi.yml
- filename: antalyatransfers-co-status-api-openapi.yml
  format: yaml
  label: AntalyaTransfers.co Status API
  slug: antalyatransfers-co-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antalyatransfers-co/openapi/antalyatransfers-co-status-api-openapi.yml
consequence_counts:
  physical: 1
  read: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Antalyatransfers Co Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/pricing/estimate
operation_count: 5
overview: 'AntalyaTransfers.co exposes 5 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AntalyaTransfers.co
provider_slug: antalyatransfers-co
slug: antalyatransfers-co-agentic-access
source_filename: antalyatransfers-co-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/antalyatransfers-co-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 4\n    acting: 1\n  by_consequence:\n    read: 4\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/status\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/pricing/estimate\n  method: post\n  operationId: estimatePrice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n  \
  \    purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/locations/popular\n  method: get\n  operationId: listPopularLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/locations/search\n  method: get\n  operationId: searchLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/fx/rates\n  method: get\n  operationId: getFxRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/antalyatransfers-co/agentic-access/antalyatransfers-co-agentic-access.yml
summary_line: 5 operations · 1 acting
tags:
- Transportation
- Travel
- Booking
- Turkey
- Taxi
---
