---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 11
api_specs:
- filename: zenserp-batch-api-openapi.yml
  format: yaml
  label: Zenserp Batch API
  slug: zenserp-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenserp/refs/heads/main/openapi/zenserp-batch-api-openapi.yml
- filename: zenserp-lists-api-openapi.yml
  format: yaml
  label: Zenserp Lists API
  slug: zenserp-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenserp/refs/heads/main/openapi/zenserp-lists-api-openapi.yml
- filename: zenserp-search-api-openapi.yml
  format: yaml
  label: Zenserp Search API
  slug: zenserp-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenserp/refs/heads/main/openapi/zenserp-search-api-openapi.yml
- filename: zenserp-shopping-api-openapi.yml
  format: yaml
  label: Zenserp Shopping Product Page API
  slug: zenserp-shopping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenserp/refs/heads/main/openapi/zenserp-shopping-api-openapi.yml
- filename: zenserp-trends-api-openapi.yml
  format: yaml
  label: Zenserp Trends API
  slug: zenserp-trends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenserp/refs/heads/main/openapi/zenserp-trends-api-openapi.yml
consequence_counts:
  read: 11
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Zenserp Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'Zenserp exposes 13 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Zenserp
provider_slug: zenserp
slug: zenserp-agentic-access
source_filename: zenserp-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: generated\nsource: openapi/zenserp-batch-api-openapi.yml, openapi/zenserp-lists-api-openapi.yml, openapi/zenserp-search-api-openapi.yml,\n  openapi/zenserp-shopping-api-openapi.yml, openapi/zenserp-trends-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 11\n    acting: 2\n  by_consequence:\n    read: 11\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /batches\n  method: get\n  operationId: listBatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /batches\n  method: post\n  operationId: submitBatch\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /batches/{id}\n  method: get\n  operationId: getBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hl\n  method: get\n  operationId: listLanguages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gl\n  method: get\n  operationId: listCountries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locations\n  method: get\n  operationId: listLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search_engines\n  method: get\n  operationId: listEngines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search\n  method: get\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status\n  method: post\n  operationId: getStatusPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /shopping\n  method: get\n  operationId: shoppingProductPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trends\n  method: get\n  operationId: trendsSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trends/trending\n  method: get\n  operationId: trendsTrending\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zenserp/refs/heads/main/agentic-access/zenserp-agentic-access.yml
summary_line: 13 operations · 2 acting
tags:
- SERP
- Search Engine Results
- Google Search
- Web Scraping
- SEO
- Image Search
- News Search
- Shopping Search
- Maps
- YouTube Search
- Bing
- Yandex
- DuckDuckGo
- Geolocation
- Keyword Research
---
