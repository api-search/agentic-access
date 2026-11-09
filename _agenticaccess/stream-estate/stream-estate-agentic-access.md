---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 10
api_specs:
- filename: stream-estate-indicators-api-openapi.yml
  format: yaml
  label: stream-estate Indicators API
  slug: stream-estate-indicators-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stream-estate/openapi/stream-estate-indicators-api-openapi.yml
- filename: stream-estate-properties-api-openapi.yml
  format: yaml
  label: stream-estate Properties API
  slug: stream-estate-properties-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stream-estate/openapi/stream-estate-properties-api-openapi.yml
- filename: stream-estate-searches-api-openapi.yml
  format: yaml
  label: stream-estate Searches API
  slug: stream-estate-searches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stream-estate/openapi/stream-estate-searches-api-openapi.yml
- filename: stream-estate-webhooks-api-openapi.yml
  format: yaml
  label: stream-estate Webhooks API
  slug: stream-estate-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stream-estate/openapi/stream-estate-webhooks-api-openapi.yml
consequence_counts:
  read: 10
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Stream Estate Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'stream-estate exposes 13 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: stream-estate
provider_slug: stream-estate
slug: stream-estate-agentic-access
source_filename: stream-estate-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/stream-estate-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 10\n    acting: 3\n  by_consequence:\n    read: 10\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /documents/properties\n  method: get\n  operationId: getProperties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/properties/{id}\n  method: get\n  operationId: getProperty\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/properties/{id}/similar-properties\n\
  \  method: get\n  operationId: getSimilarProperties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /indicators/price_per_meter\n  method: get\n  operationId: getPricePerMeter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /indicators/points_of_interest\n  method: get\n  operationId: getPointsOfInterest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/location-autocomplete\n  method: get\n  operationId: locationAutocomplete\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cities\n  method: get\n  operationId: getCities\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /searches\n  method: get\n  operationId: getSearches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /searches\n  method: post\n  operationId: createSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /searches/{id}\n  method: get\n  operationId: getSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /searches/{id}\n  method: put\n  operationId: updateSearch\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /searches/{id}\n  method: delete\n  operationId: deleteSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook-tester\n  method: get\n  operationId: simulateWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/stream-estate/agentic-access/stream-estate-agentic-access.yml
summary_line: 13 operations · 3 acting
tags:
- Real Estate
- PropTech
- Data API
- Market Analytics
- Valuation
---
