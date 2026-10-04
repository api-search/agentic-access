---
acting_count: 0
action_class_counts:
  connected: 13
api_specs:
- filename: dlr-capabilities-api-openapi.yml
  format: yaml
  label: DLR Capabilities API
  slug: dlr-capabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dlr/refs/heads/main/openapi/dlr-capabilities-api-openapi.yml
- filename: dlr-data-api-openapi.yml
  format: yaml
  label: DLR Data API
  slug: dlr-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dlr/refs/heads/main/openapi/dlr-data-api-openapi.yml
- filename: dlr-stac-api-openapi.yml
  format: yaml
  label: DLR STAC API
  slug: dlr-stac-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dlr/refs/heads/main/openapi/dlr-stac-api-openapi.yml
consequence_counts:
  read: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Dlr Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'DLR exposes 13 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: DLR
provider_slug: dlr
slug: dlr-agentic-access
source_filename: dlr-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/dlr-capabilities-api-openapi.yml, openapi/dlr-data-api-openapi.yml, openapi/dlr-stac-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 13\n  by_consequence:\n    read: 13\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: getLandingPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conformance\n  method: get\n  operationId: getConformanceDeclaration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /filter-capabilities\n  method: get\n  operationId: getFilterCapabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/queryables\n  method: get\n  operationId: getSearchQueryables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/sortables\n  method: get\n  operationId: getSearchSortables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections\n  method: get\n  operationId: getCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collectionId}\n  method: get\n  operationId: describeCollection\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collectionId}/queryables\n  method: get\n  operationId: getQueryables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collectionId}/sortables\n  method: get\n  operationId: getSortables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collectionId}/items\n  method: get\n  operationId: getFeatures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collectionId}/items/{featureId}\n  method: get\n  operationId: getFeature\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search\n  method: get\n  operationId: getSearchSTAC\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search\n  method: post\n  operationId: postSearchSTAC\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dlr/refs/heads/main/agentic-access/dlr-agentic-access.yml
summary_line: 13 operations
tags:
- Earth Observation
- Remote Sensing
- Satellite Data
- Geospatial
- Aerospace
- Open Data
- OGC
- STAC
- Atmospheric Science
- Digital Elevation Models
---
