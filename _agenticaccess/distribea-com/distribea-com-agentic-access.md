---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 5
api_specs:
- filename: distribea-com-account-api-openapi.yml
  format: yaml
  label: Distribea Account API
  slug: distribea-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/distribea-com/openapi/distribea-com-account-api-openapi.yml
- filename: distribea-com-catalog-api-openapi.yml
  format: yaml
  label: Distribea Catalog API
  slug: distribea-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/distribea-com/openapi/distribea-com-catalog-api-openapi.yml
- filename: distribea-com-generation-api-openapi.yml
  format: yaml
  label: Distribea Generation API
  slug: distribea-com-generation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/distribea-com/openapi/distribea-com-generation-api-openapi.yml
- filename: distribea-com-models-api-openapi.yml
  format: yaml
  label: Distribea Models API
  slug: distribea-com-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/distribea-com/openapi/distribea-com-models-api-openapi.yml
consequence_counts:
  read: 5
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Distribea Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Distribea exposes 9 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Distribea
provider_slug: distribea-com
slug: distribea-com-agentic-access
source_filename: distribea-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/distribea-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 5\n    acting: 4\n  by_consequence:\n    read: 5\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1\n  method: get\n  operationId: getApiIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/catalog/search\n  method: get\n  operationId: searchCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/catalog/items/{slug}\n\
  \  method: get\n  operationId: getCatalogItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/models\n  method: get\n  operationId: listModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/account\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/generate/image\n  method: post\n  operationId: generateImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/generate/video\n\
  \  method: post\n  operationId: generateVideo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/generate/music\n  method: post\n  operationId: generateMusic\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/generate/voice\n  method: post\n  operationId: generateVoice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/distribea-com/agentic-access/distribea-com-agentic-access.yml
summary_line: 9 operations · 4 acting
tags:
- Artificial Intelligence
- Video
- Media
- Software-as-a-Service
- Platform
---
