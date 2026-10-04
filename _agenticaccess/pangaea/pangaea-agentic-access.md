---
acting_count: 0
action_class_counts:
  connected: 6
api_specs:
- filename: pangaea-doi-filter-api-openapi.yml
  format: yaml
  label: PANGAEA DOI Filter API
  slug: pangaea-doi-filter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pangaea/refs/heads/main/openapi/pangaea-doi-filter-api-openapi.yml
- filename: pangaea-geo-filter-api-openapi.yml
  format: yaml
  label: PANGAEA Geo Filter API
  slug: pangaea-geo-filter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pangaea/refs/heads/main/openapi/pangaea-geo-filter-api-openapi.yml
- filename: pangaea-oai-pmh-api-openapi.yml
  format: yaml
  label: PANGAEA OAI-PMH API
  slug: pangaea-oai-pmh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pangaea/refs/heads/main/openapi/pangaea-oai-pmh-api-openapi.yml
- filename: pangaea-search-api-openapi.yml
  format: yaml
  label: PANGAEA Search API
  slug: pangaea-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pangaea/refs/heads/main/openapi/pangaea-search-api-openapi.yml
- filename: pangaea-terms-api-openapi.yml
  format: yaml
  label: PANGAEA Terms API
  slug: pangaea-terms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pangaea/refs/heads/main/openapi/pangaea-terms-api-openapi.yml
consequence_counts:
  read: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Pangaea Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'PANGAEA exposes 6 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: PANGAEA
provider_slug: pangaea
slug: pangaea-agentic-access
source_filename: pangaea-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/pangaea-doi-filter-api-openapi.yml, openapi/pangaea-geo-filter-api-openapi.yml,\n  openapi/pangaea-oai-pmh-api-openapi.yml, openapi/pangaea-search-api-openapi.yml, openapi/pangaea-terms-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 6\n  by_consequence:\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /dds-fdp/rest/panquery\n  method: get\n  operationId: queryByDOI\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dds-fgp/rest/dwhquery\n  method: get\n  operationId: queryByGeoParameters\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provider\n  method: get\n  operationId: oaiPmhRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /panmd/_search\n  method: get\n  operationId: searchDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /panmd/_search\n  method: post\n  operationId: searchDatasetsPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pangaea-terms/term/_search\n  method: post\n  operationId: searchTerms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pangaea/refs/heads/main/agentic-access/pangaea-agentic-access.yml
summary_line: 6 operations
tags:
- Earth Science
- Ocean Data
- Climate Records
- Environmental Science
- Geoscience
- Open Data
- Scientific Data
- Research Data
- OAI-PMH
- Research Repository
---
