---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 13
api_specs:
- filename: yappy-biz-batch-api-openapi.yml
  format: yaml
  label: yappy-biz Batch API
  slug: yappy-biz-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yappy-biz/openapi/yappy-biz-batch-api-openapi.yml
- filename: yappy-biz-commerce-api-openapi.yml
  format: yaml
  label: yappy-biz Commerce API
  slug: yappy-biz-commerce-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yappy-biz/openapi/yappy-biz-commerce-api-openapi.yml
- filename: yappy-biz-discovery-api-openapi.yml
  format: yaml
  label: yappy-biz Discovery API
  slug: yappy-biz-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yappy-biz/openapi/yappy-biz-discovery-api-openapi.yml
- filename: yappy-biz-documentation-api-openapi.yml
  format: yaml
  label: yappy-biz Documentation API
  slug: yappy-biz-documentation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yappy-biz/openapi/yappy-biz-documentation-api-openapi.yml
- filename: yappy-biz-exports-api-openapi.yml
  format: yaml
  label: yappy-biz Exports API
  slug: yappy-biz-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yappy-biz/openapi/yappy-biz-exports-api-openapi.yml
- filename: yappy-biz-product-api-openapi.yml
  format: yaml
  label: yappy-biz Product API
  slug: yappy-biz-product-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yappy-biz/openapi/yappy-biz-product-api-openapi.yml
- filename: yappy-biz-releases-api-openapi.yml
  format: yaml
  label: yappy-biz Releases API
  slug: yappy-biz-releases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yappy-biz/openapi/yappy-biz-releases-api-openapi.yml
consequence_counts:
  read: 13
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Yappy Biz Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'yappy-biz exposes 15 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: yappy-biz
provider_slug: yappy-biz
slug: yappy-biz-agentic-access
source_filename: yappy-biz-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/yappy-biz-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 13\n    acting: 2\n  by_consequence:\n    read: 13\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: getServiceIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /releases\n  method: get\n  operationId: listReleases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:releases\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /releases/latest\n\
  \  method: get\n  operationId: getLatestRelease\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:releases\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /releases/{version}\n  method: get\n  operationId: getRelease\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:releases\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /docs\n  method: get\n  operationId: listDocs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:docs\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /docs/{slug}\n  method: get\n  operationId: getDoc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:docs\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /faq\n  method: get\n  operationId: listFaq\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:faq\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pricing\n  method: get\n  operationId: getPricing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:pricing\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /features\n  method: get\n  operationId: listFeatures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /requirements\n  method: get\n  operationId: getRequirements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /compatibility\n  method: get\n  operationId: checkCompatibility\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /search\n  method: get\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:docs\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /batch\n  method: post\n  operationId: createBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /exports\n  method: post\n  operationId: createExport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - export:docs\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /exports/{job_id}\n\
  \  method: get\n  operationId: getExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - export:docs\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/yappy-biz/agentic-access/yappy-biz-agentic-access.yml
summary_line: 15 operations · 2 acting
tags:
- Voice
- macOS
- Automation
- Accessibility
- Productivity
---
