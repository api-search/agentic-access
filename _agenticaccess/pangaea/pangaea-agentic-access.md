---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 4
api_specs:
- filename: _search
  format: yaml
  label: PANGAEA Elasticsearch Search API
  slug: pangaea-elasticsearch-search-api
  spec_type: OpenAPI
  url: https://ws.pangaea.de/es/pangaea/panmd/_search
- filename: provider
  format: yaml
  label: PANGAEA OAI-PMH Metadata Harvesting API
  slug: pangaea-oai-pmh-metadata-harvesting-api
  spec_type: OpenAPI
  url: https://ws.pangaea.de/oai/provider?verb=Identify
consequence_counts:
  read: 4
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Pangaea Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'PANGAEA exposes 6 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: PANGAEA
provider_slug: pangaea
slug: pangaea-agentic-access
source_filename: pangaea-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/pangaea-data-download-api.yml, openapi/pangaea-oai-pmh-api.yml, openapi/pangaea-search-api.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 4\n    acting: 2\n  by_consequence:\n    read: 4\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /dds-fdp/rest/panquery\n  method: get\n  operationId: queryByDOI\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dds-fgp/rest/dwhquery\n  method: get\n  operationId: queryByGeoParameters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /provider\n  method: get\n  operationId: oaiPmhRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /panmd/_search\n  method: get\n  operationId: searchDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /panmd/_search\n  method: post\n  operationId: searchDatasetsPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pangaea-terms/term/_search\n  method: post\n  operationId: searchTerms\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pangaea/refs/heads/main/agentic-access/pangaea-agentic-access.yml
summary_line: 6 operations · 2 acting
tags:
- Earth Science
- Ocean Data
- Climate Records
- Environmental Science
- Geoscience
- Open Data
- Scientific Data
---
