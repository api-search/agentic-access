---
acting_count: 0
action_class_counts:
  connected: 8
api_specs:
- filename: dabyte-ai-aiv-csv-api-openapi.yml
  format: yaml
  label: DABYTE Aiv.csv API
  slug: dabyte-ai-aiv-csv-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dabyte-ai/openapi/dabyte-ai-aiv-csv-api-openapi.yml
- filename: dabyte-ai-aiv-json-api-openapi.yml
  format: yaml
  label: DABYTE Aiv.json API
  slug: dabyte-ai-aiv-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dabyte-ai/openapi/dabyte-ai-aiv-json-api-openapi.yml
- filename: dabyte-ai-brands-api-openapi.yml
  format: yaml
  label: DABYTE Brands API
  slug: dabyte-ai-brands-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dabyte-ai/openapi/dabyte-ai-brands-api-openapi.yml
- filename: dabyte-ai-brands-json-api-openapi.yml
  format: yaml
  label: DABYTE Brands.json API
  slug: dabyte-ai-brands-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dabyte-ai/openapi/dabyte-ai-brands-json-api-openapi.yml
- filename: dabyte-ai-history-json-api-openapi.yml
  format: yaml
  label: DABYTE History.json API
  slug: dabyte-ai-history-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dabyte-ai/openapi/dabyte-ai-history-json-api-openapi.yml
- filename: dabyte-ai-index-md-api-openapi.yml
  format: yaml
  label: DABYTE Index.md API
  slug: dabyte-ai-index-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dabyte-ai/openapi/dabyte-ai-index-md-api-openapi.yml
- filename: dabyte-ai-measurement-status-json-api-openapi.yml
  format: yaml
  label: DABYTE Measurement Status.json API
  slug: dabyte-ai-measurement-status-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dabyte-ai/openapi/dabyte-ai-measurement-status-json-api-openapi.yml
- filename: dabyte-ai-methodology-json-api-openapi.yml
  format: yaml
  label: DABYTE Methodology.json API
  slug: dabyte-ai-methodology-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dabyte-ai/openapi/dabyte-ai-methodology-json-api-openapi.yml
consequence_counts:
  read: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Dabyte Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'DABYTE exposes 8 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: DABYTE
provider_slug: dabyte-ai
slug: dabyte-ai-agentic-access
source_filename: dabyte-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/dabyte-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 8\n  by_consequence:\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /api/aiv.json\n  method: get\n  operationId: getVisibilityIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/history.json\n  method: get\n  operationId: getHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/brands.json\n  method: get\n  operationId: listTrackedBrands\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/brands/{slug}.json\n  method: get\n  operationId: getBrandVisibility\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/methodology.json\n  method: get\n  operationId: getMethodology\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/measurement-status.json\n  method: get\n  operationId: getMeasurementStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /aiv.csv\n  method: get\n  operationId: getIndexCsv\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /index.md\n  method: get\n  operationId: getIndexMarkdown\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/dabyte-ai/agentic-access/dabyte-ai-agentic-access.yml
summary_line: 8 operations
tags:
- Software-as-a-Service
- AI Tools
- Visibility Index
- Open Data
- CC-BY
---
