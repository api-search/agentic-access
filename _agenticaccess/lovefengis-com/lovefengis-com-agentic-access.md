---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 6
api_specs:
- filename: lovefengis-com-batch-api-openapi.yml
  format: yaml
  label: lovefengis-com Batch API
  slug: lovefengis-com-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lovefengis-com/openapi/lovefengis-com-batch-api-openapi.yml
- filename: lovefengis-com-catalog-api-openapi.yml
  format: yaml
  label: lovefengis-com Catalog API
  slug: lovefengis-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lovefengis-com/openapi/lovefengis-com-catalog-api-openapi.yml
- filename: lovefengis-com-jobs-api-openapi.yml
  format: yaml
  label: lovefengis-com Jobs API
  slug: lovefengis-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lovefengis-com/openapi/lovefengis-com-jobs-api-openapi.yml
consequence_counts:
  read: 6
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Lovefengis Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'lovefengis-com exposes 8 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: lovefengis-com
provider_slug: lovefengis-com
slug: lovefengis-com-agentic-access
source_filename: lovefengis-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/lovefengis-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 6\n    acting: 2\n  by_consequence:\n    read: 6\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1\n  method: get\n  operationId: getApiIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/status\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/hizmetler\n  method: get\n  operationId:\
  \ listServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/hizmetler/{id}\n  method: get\n  operationId: getService\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/fiyatlar\n  method: get\n  operationId: listPrices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/batch\n  method: post\n  operationId: batchRead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/jobs\n  method: post\n  operationId: createJob\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/jobs/{id}\n  method: get\n  operationId: getJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/lovefengis-com/agentic-access/lovefengis-com-agentic-access.yml
summary_line: 8 operations · 2 acting
tags:
- Company
- Digital Marketing
- SEO
- Advertising
- Web Services
- Turkey
---
