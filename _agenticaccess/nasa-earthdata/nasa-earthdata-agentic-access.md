---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 12
api_specs:
- filename: search_api_docs.html
  format: yaml
  label: CMR Search API
  slug: cmr-search-api
  spec_type: OpenAPI
  url: https://cmr.earthdata.nasa.gov/search/site/search_api_docs.html
- filename: harmony-api-openapi.json
  format: json
  label: Harmony API
  slug: harmony-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-earthdata/refs/heads/main/openapi/harmony-api-openapi.json
consequence_counts:
  read: 12
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Nasa Earthdata Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'NASA Earthdata exposes 13 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: NASA Earthdata
provider_slug: nasa-earthdata
slug: nasa-earthdata-agentic-access
source_filename: nasa-earthdata-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/harmony-api-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 12\n    acting: 1\n  by_consequence:\n    read: 12\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: getLandingPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api\n  method: get\n  operationId: getSpecification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conformance\n  method: get\n  operationId: getRequirementsClasses\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections\n  method: get\n  operationId: describeCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collectionId}\n  method: get\n  operationId: describeCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collectionId}/coverage\n  method: get\n  operationId: getCoverageOffering\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collectionId}/coverage/description\n  method: get\n  operationId: getCoverageDescription\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collectionId}/coverage/domainset\n  method: get\n  operationId: getCoverageDomainSet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collectionId}/coverage/rangetype\n  method: get\n  operationId: getCoverageRangeType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collectionId}/coverage/metadata\n  method: get\n  operationId: getCoverageMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collectionId}/coverage/rangeset\n  method: get\n  operationId: getCoverageRangeset\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collectionId}/coverage/rangeset\n  method: post\n  operationId: postCoverageRangeset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collections/{collectionId}/coverage/all\n  method: get\n  operationId: getCoverageAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nasa-earthdata/refs/heads/main/agentic-access/nasa-earthdata-agentic-access.yml
summary_line: 13 operations · 1 acting
tags:
- Earth Observation
- Satellite Data
- Climate Data
- Remote Sensing
- Geospatial
- NASA
- Science Data
---
