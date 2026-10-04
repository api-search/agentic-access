---
acting_count: 0
action_class_counts:
  connected: 10
api_specs:
- filename: nasa-cmr-capabilities-api-openapi.yml
  format: yaml
  label: NASA CMR Capabilities API
  slug: nasa-cmr-capabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-cmr/refs/heads/main/openapi/nasa-cmr-capabilities-api-openapi.yml
- filename: nasa-cmr-collections-api-openapi.yml
  format: yaml
  label: NASA CMR Collections API
  slug: nasa-cmr-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-cmr/refs/heads/main/openapi/nasa-cmr-collections-api-openapi.yml
- filename: nasa-cmr-data-api-openapi.yml
  format: yaml
  label: NASA CMR Data API
  slug: nasa-cmr-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-cmr/refs/heads/main/openapi/nasa-cmr-data-api-openapi.yml
- filename: nasa-cmr-stac-api-openapi.yml
  format: yaml
  label: NASA CMR STAC API
  slug: nasa-cmr-stac-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-cmr/refs/heads/main/openapi/nasa-cmr-stac-api-openapi.yml
consequence_counts:
  read: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Nasa Cmr Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'NASA CMR exposes 10 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: NASA CMR
provider_slug: nasa-cmr
slug: nasa-cmr-agentic-access
source_filename: nasa-cmr-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/nasa-cmr-capabilities-api-openapi.yml, openapi/nasa-cmr-collections-api-openapi.yml,\n  openapi/nasa-cmr-data-api-openapi.yml, openapi/nasa-cmr-stac-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 10\n  by_consequence:\n    read: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: getProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /docs\n  method: get\n  operationId: getConformanceDeclaration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{providerId}\n  method: get\n  operationId: getProvider\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{providerId}/collections\n  method: get\n  operationId: getCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{providerId}/collections/{collectionId}\n  method: get\n  operationId: describeCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections{response_format}\n  method: get\n  operationId: getCollections{responseFormat}\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /{providerId}/collections/{collectionId}/items\n  method: get\n  operationId: getFeatures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: '{providerId}/collections/{collectionId}/items/{featureId}'\n  method: get\n  operationId: getFeature\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{providerId}/search\n  method: get\n  operationId: getSearchSTAC\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{providerId}/search\n  method: post\n  operationId: postSearchSTAC\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nasa-cmr/refs/heads/main/agentic-access/nasa-cmr-agentic-access.yml
summary_line: 10 operations
tags:
- NASA
- Earth Science
- Satellite Data
- Remote Sensing
- Geospatial
- Open Data
- Metadata
- Collection
- Granules
---
