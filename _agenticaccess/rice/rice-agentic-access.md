---
acting_count: 0
action_class_counts:
  connected: 5
api_specs:
- filename: rice-datasets-api-openapi.yml
  format: yaml
  label: Rice University Datasets API
  slug: rice-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rice/refs/heads/main/openapi/rice-datasets-api-openapi.yml
- filename: rice-reference-api-openapi.yml
  format: yaml
  label: Rice University Reference API
  slug: rice-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rice/refs/heads/main/openapi/rice-reference-api-openapi.yml
consequence_counts:
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Rice Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Rice University exposes 5 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Rice University
provider_slug: rice
slug: rice-agentic-access
source_filename: rice-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: generated\nsource: openapi/rice-datasets-api-openapi.yml, openapi/rice-reference-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 5\n  by_consequence:\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /datasets\n  method: get\n  operationId: listDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets/{datasetId}\n  method: get\n  operationId: getDataset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets/{datasetId}/vrde\n\
  \  method: get\n  operationId: getDatasetVrde\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/catalog\n  method: get\n  operationId: getUserCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lookups\n  method: get\n  operationId: getLookups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rice/refs/heads/main/agentic-access/rice-agentic-access.yml
summary_line: 5 operations
tags:
- University
- Higher Education
- Education
- United States
- Texas
- Private Research University
- Association of American Universities
- Research Data
- Open Data
- Research Repository
- Course Catalog
- Identity Federation
- Library
- Urban Research
---
