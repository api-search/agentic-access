---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 11
api_specs:
- filename: shipshapedata-com-ai-readiness-api-openapi.yml
  format: yaml
  label: shipshapedata-com Ai Readiness API
  slug: shipshapedata-com-ai-readiness-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shipshapedata-com/openapi/shipshapedata-com-ai-readiness-api-openapi.yml
- filename: shipshapedata-com-batch-api-openapi.yml
  format: yaml
  label: shipshapedata-com Batch API
  slug: shipshapedata-com-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shipshapedata-com/openapi/shipshapedata-com-batch-api-openapi.yml
- filename: shipshapedata-com-case-studies-api-openapi.yml
  format: yaml
  label: shipshapedata-com Case Studies API
  slug: shipshapedata-com-case-studies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shipshapedata-com/openapi/shipshapedata-com-case-studies-api-openapi.yml
- filename: shipshapedata-com-contact-api-openapi.yml
  format: yaml
  label: shipshapedata-com Contact API
  slug: shipshapedata-com-contact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shipshapedata-com/openapi/shipshapedata-com-contact-api-openapi.yml
- filename: shipshapedata-com-export-api-openapi.yml
  format: yaml
  label: shipshapedata-com Export API
  slug: shipshapedata-com-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shipshapedata-com/openapi/shipshapedata-com-export-api-openapi.yml
- filename: shipshapedata-com-industries-api-openapi.yml
  format: yaml
  label: shipshapedata-com Industries API
  slug: shipshapedata-com-industries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shipshapedata-com/openapi/shipshapedata-com-industries-api-openapi.yml
- filename: shipshapedata-com-resources-api-openapi.yml
  format: yaml
  label: shipshapedata-com Resources API
  slug: shipshapedata-com-resources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shipshapedata-com/openapi/shipshapedata-com-resources-api-openapi.yml
- filename: shipshapedata-com-services-api-openapi.yml
  format: yaml
  label: shipshapedata-com Services API
  slug: shipshapedata-com-services-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shipshapedata-com/openapi/shipshapedata-com-services-api-openapi.yml
- filename: shipshapedata-com-shipshape-data-api-api-openapi.yml
  format: yaml
  label: shipshapedata-com Shipshape Data API
  slug: shipshapedata-com-shipshape-data-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shipshapedata-com/openapi/shipshapedata-com-shipshape-data-api-api-openapi.yml
consequence_counts:
  read: 11
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Shipshapedata Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'shipshapedata-com exposes 13 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: shipshapedata-com
provider_slug: shipshapedata-com
slug: shipshapedata-com-agentic-access
source_filename: shipshapedata-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/shipshapedata-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 11\n    acting: 2\n  by_consequence:\n    read: 11\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /v1\n  method: get\n  operationId: getApiIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/services\n  method: get\n  operationId: listServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/services/{slug}\n  method: get\n  operationId:\
  \ getService\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/industries\n  method: get\n  operationId: listIndustries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/case-studies\n  method: get\n  operationId: listCaseStudies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/case-studies/{slug}\n  method: get\n  operationId: getCaseStudy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/resources\n  method: get\n  operationId: searchResources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /v1/resources/categories\n  method: get\n  operationId: listResourceCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ai-readiness/questions\n  method: get\n  operationId: getAiReadinessQuestions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ai-readiness/score\n  method: post\n  operationId: scoreAiReadiness\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/batch\n  method: post\n  operationId: batchRequests\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/export\n  method: get\n  operationId: getBulkExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - export\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/contact\n  method: get\n  operationId: getContactInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/shipshapedata-com/agentic-access/shipshapedata-com-agentic-access.yml
summary_line: 13 operations · 2 acting
tags:
- Artificial Intelligence
- Data
- Consultancy
- London
---
