---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 3
api_specs:
- filename: crawlerdata-com-custom-search-compatible-api-openapi.yml
  format: yaml
  label: crawlerdata-com Custom Search-compatible API
  slug: crawlerdata-com-custom-search-compatible-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crawlerdata-com/openapi/crawlerdata-com-custom-search-compatible-api-openapi.yml
- filename: crawlerdata-com-jobs-api-openapi.yml
  format: yaml
  label: crawlerdata-com Jobs API
  slug: crawlerdata-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crawlerdata-com/openapi/crawlerdata-com-jobs-api-openapi.yml
- filename: crawlerdata-com-open-webui-api-openapi.yml
  format: yaml
  label: crawlerdata-com Open WebUI API
  slug: crawlerdata-com-open-webui-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crawlerdata-com/openapi/crawlerdata-com-open-webui-api-openapi.yml
- filename: crawlerdata-com-serpapi-compatible-api-openapi.yml
  format: yaml
  label: crawlerdata-com Serp API Compatible API
  slug: crawlerdata-com-serpapi-compatible-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crawlerdata-com/openapi/crawlerdata-com-serpapi-compatible-api-openapi.yml
consequence_counts:
  read: 3
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Crawlerdata Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'crawlerdata-com exposes 5 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: crawlerdata-com
provider_slug: crawlerdata-com
slug: crawlerdata-com-agentic-access
source_filename: crawlerdata-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/crawlerdata-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    acting: 2\n    connected: 3\n  by_consequence:\n    write: 2\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/jobs\n  method: post\n  operationId: submitJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/jobs/{jobId}\n  method: get\n  operationId: getJob\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search.json\n  method: get\n  operationId: serpApiSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customsearch/v1\n  method: get\n  operationId: customSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/openwebui/search\n  method: post\n  operationId: openWebUiSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/crawlerdata-com/agentic-access/crawlerdata-com-agentic-access.yml
summary_line: 5 operations · 2 acting
tags:
- Search
- Google
- SERP
- Data
- E-Commerce
- SEO
---
