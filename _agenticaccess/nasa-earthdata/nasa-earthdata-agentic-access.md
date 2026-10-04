---
acting_count: 0
action_class_counts:
  connected: 13
api_specs:
- filename: nasa-earthdata-capabilities-api-openapi.yml
  format: yaml
  label: NASA Earthdata Capabilities API
  slug: nasa-earthdata-capabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-earthdata/refs/heads/main/openapi/nasa-earthdata-capabilities-api-openapi.yml
- filename: nasa-earthdata-coverage-api-openapi.yml
  format: yaml
  label: NASA Earthdata Coverage API
  slug: nasa-earthdata-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-earthdata/refs/heads/main/openapi/nasa-earthdata-coverage-api-openapi.yml
- filename: nasa-earthdata-open-api-api-openapi.yml
  format: yaml
  label: NASA Earthdata Open API
  slug: nasa-earthdata-open-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-earthdata/refs/heads/main/openapi/nasa-earthdata-open-api-api-openapi.yml
consequence_counts:
  read: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Nasa Earthdata Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'NASA Earthdata exposes 13 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: NASA Earthdata
provider_slug: nasa-earthdata
slug: nasa-earthdata-agentic-access
source_filename: nasa-earthdata-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/nasa-earthdata-capabilities-api-openapi.yml, openapi/nasa-earthdata-coverage-api-openapi.yml,\n  openapi/nasa-earthdata-open-api-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 13\n  by_consequence:\n    read: 13\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: getLandingPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conformance\n  method: get\n  operationId: getRequirementsClasses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections\n  method: get\n  operationId: describeCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collectionId}\n  method: get\n  operationId: describeCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collectionId}/coverage\n  method: get\n  operationId: getCoverageOffering\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collectionId}/coverage/description\n  method: get\n  operationId: getCoverageDescription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /collections/{collectionId}/coverage/domainset\n  method: get\n  operationId: getCoverageDomainSet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collectionId}/coverage/rangetype\n  method: get\n  operationId: getCoverageRangeType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collectionId}/coverage/metadata\n  method: get\n  operationId: getCoverageMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collectionId}/coverage/rangeset\n  method: get\n  operationId: getCoverageRangeset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /collections/{collectionId}/coverage/rangeset\n  method: post\n  operationId: postCoverageRangeset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collectionId}/coverage/all\n  method: get\n  operationId: getCoverageAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api\n  method: get\n  operationId: getSpecification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nasa-earthdata/refs/heads/main/agentic-access/nasa-earthdata-agentic-access.yml
summary_line: 13 operations
tags:
- Earth Observation
- Satellite Data
- Climate Data
- Remote Sensing
- Geospatial
- NASA
- Science Data
---
