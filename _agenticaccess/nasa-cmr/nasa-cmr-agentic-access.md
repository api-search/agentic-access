---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 9
api_specs:
- filename: api.html
  format: yaml
  label: CMR Search API
  slug: cmr-search
  spec_type: OpenAPI
  url: https://cmr.earthdata.nasa.gov/search/site/docs/search/api.html
consequence_counts:
  read: 9
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Nasa Cmr Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'NASA CMR exposes 10 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: NASA CMR
provider_slug: nasa-cmr
slug: nasa-cmr-agentic-access
source_filename: nasa-cmr-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/nasa-cmr-search-openapi.json, openapi/nasa-cmr-stac-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 9\n    acting: 1\n  by_consequence:\n    read: 9\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /collections{response_format}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: getProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /docs\n  method: get\n\
  \  operationId: getConformanceDeclaration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{providerId}\n  method: get\n  operationId: getProvider\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{providerId}/collections\n  method: get\n  operationId: getCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{providerId}/collections/{collectionId}\n  method: get\n  operationId: describeCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{providerId}/collections/{collectionId}/items\n  method: get\n  operationId: getFeatures\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: '{providerId}/collections/{collectionId}/items/{featureId}'\n  method: get\n  operationId: getFeature\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{providerId}/search\n  method: get\n  operationId: getSearchSTAC\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{providerId}/search\n  method: post\n  operationId: postSearchSTAC\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nasa-cmr/refs/heads/main/agentic-access/nasa-cmr-agentic-access.yml
summary_line: 10 operations · 1 acting
tags:
- NASA
- Earth Science
- Satellite Data
- Remote Sensing
- Geospatial
- Open Data
- Metadata
- Collections
- Granules
---
