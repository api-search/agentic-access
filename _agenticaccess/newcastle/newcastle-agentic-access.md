---
acting_count: 0
action_class_counts:
  connected: 24
api_specs:
- filename: newcastle-digitised-objects-api-openapi.yml
  format: yaml
  label: Digitised Objects Repository Search and Data API
  slug: digitised-objects
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle/refs/heads/main/openapi/newcastle-digitised-objects-api-openapi.yml
- filename: newcastle-entity-api-openapi.yml
  format: yaml
  label: Urban Observatory API (Urban Sciences Building) — Entity
  slug: urban-observatory-entity
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle/refs/heads/main/openapi/newcastle-entity-api-openapi.yml
- filename: newcastle-feed-api-openapi.yml
  format: yaml
  label: Urban Observatory API (Urban Sciences Building) — Feed
  slug: urban-observatory-feed
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle/refs/heads/main/openapi/newcastle-feed-api-openapi.yml
- filename: newcastle-summary-api-openapi.yml
  format: yaml
  label: Urban Observatory API (Urban Sciences Building) — Summary
  slug: urban-observatory-summary
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle/refs/heads/main/openapi/newcastle-summary-api-openapi.yml
- filename: newcastle-api-metadata-information-api-openapi.yml
  format: yaml
  label: Newcastle University API Metadata Information API
  slug: newcastle-api-metadata-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle/refs/heads/main/openapi/newcastle-api-metadata-information-api-openapi.yml
- filename: newcastle-v1-api-openapi.yml
  format: yaml
  label: Newcastle University V1 API
  slug: newcastle-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle/refs/heads/main/openapi/newcastle-v1-api-openapi.yml
- filename: newcastle-time-series-api-openapi.yml
  format: yaml
  label: Newcastle University Time Series API
  slug: newcastle-time-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle/refs/heads/main/openapi/newcastle-time-series-api-openapi.yml
consequence_counts:
  read: 24
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Newcastle Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 24
overview: 'Newcastle University exposes 24 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 24 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Newcastle University
provider_slug: newcastle
slug: newcastle-agentic-access
source_filename: newcastle-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: generated\nsource: openapi/newcastle-api-metadata-information-api-openapi.yml, openapi/newcastle-digitised-objects-api-openapi.yml,\n  openapi/newcastle-entity-api-openapi.yml, openapi/newcastle-feed-api-openapi.yml, openapi/newcastle-summary-api-openapi.yml,\n  openapi/newcastle-time-series-api-openapi.yml, openapi/newcastle-v1-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 24\n  by_action_class:\n    connected: 24\n  by_consequence:\n    read: 24\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: getHome\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /info\n  method: get\n  operationId: getInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /info/open-api\n  method: get\n  operationId: getInfoOpenAPI\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iiif/{id}\n  method: get\n  operationId: getIIIF\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2.0a/sensors/entity\n  method: get\n  operationId: EntityController.getAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2.0a/sensors/entity/{id}\n  method: get\n  operationId: EntityController.getOne\n  x-agentic-access:\n    action-class: connected\n   \
  \ consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2.0a/sensors/feed/{id}\n  method: get\n  operationId: FeedController.getOne\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2.0a/sensors/summary\n  method: get\n  operationId: SummaryController.getSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2.0a/sensors/timeseries/{id}\n  method: get\n  operationId: TimeseriesController.getOne\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2.0a/sensors/timeseries/{id}/historic\n  method: get\n  operationId: TimeseriesController.getHistoric\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/collections\n  method: get\n  operationId: getV1CollectionsIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/collections/{id}\n  method: get\n  operationId: getV1CollectionsShow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/digitised-objects\n  method: get\n  operationId: getV1DigitisedObjectsIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/digitised-objects/search\n  method: get\n  operationId: getV1DigitisedObjectsSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/digitised-objects/search/autocomplete\n  method: get\n  operationId: getV1DigitisedObjectsSearchAutocomplete\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/digitised-objects/{id}\n  method: get\n  operationId: getV1DigitisedObjectsShow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/digitised-objects/{id}/transcript/content\n  method: get\n  operationId: getV1DigitisedObjectsTranscriptContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/items\n  method: get\n  operationId: getV1ItemsIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /v1/items/search\n  method: get\n  operationId: getV1ItemsSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/items/search/autocomplete\n  method: get\n  operationId: getV1ItemsSearchAutocomplete\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/items/{id}/{position}\n  method: get\n  operationId: getV1ItemsShow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/items/{id}/{position}/transcript/content\n  method: get\n  operationId: getV1ItemsTranscriptContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/contentdm/{collectionId}/{itemId}\n \
  \ method: get\n  operationId: getV1Contentdm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tei/{id}/content\n  method: get\n  operationId: getV1TEIContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/newcastle/refs/heads/main/agentic-access/newcastle-agentic-access.yml
summary_line: 24 operations
tags:
- University
- Higher Education
- Education
- United Kingdom
- Russell Group
- Research Data
- Open Data
- Digital Library
- Identity Federation
- Smart Cities
- Cultural Heritage
---
