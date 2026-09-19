---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 9
api_specs:
- filename: microsoft-bing-autosuggest-api-openapi.yml
  format: yaml
  label: Microsoft Bing Autosuggest API
  slug: microsoft-bing-autosuggest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-bing/refs/heads/main/openapi/microsoft-bing-autosuggest-api-openapi.yml
- filename: microsoft-bing-custom-search-api-openapi.yml
  format: yaml
  label: Microsoft Bing Custom Search API
  slug: microsoft-bing-custom-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-bing/refs/heads/main/openapi/microsoft-bing-custom-search-api-openapi.yml
- filename: microsoft-bing-entity-search-api-openapi.yml
  format: yaml
  label: Microsoft Bing Entity Search API
  slug: microsoft-bing-entity-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-bing/refs/heads/main/openapi/microsoft-bing-entity-search-api-openapi.yml
- filename: microsoft-bing-image-search-api-openapi.yml
  format: yaml
  label: Microsoft Bing Image Search API
  slug: microsoft-bing-image-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-bing/refs/heads/main/openapi/microsoft-bing-image-search-api-openapi.yml
- filename: microsoft-bing-news-search-api-openapi.yml
  format: yaml
  label: Microsoft Bing News Search API
  slug: microsoft-bing-news-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-bing/refs/heads/main/openapi/microsoft-bing-news-search-api-openapi.yml
- filename: microsoft-bing-spell-check-api-openapi.yml
  format: yaml
  label: Microsoft Bing Spell Check API
  slug: microsoft-bing-spell-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-bing/refs/heads/main/openapi/microsoft-bing-spell-check-api-openapi.yml
- filename: microsoft-bing-video-search-api-openapi.yml
  format: yaml
  label: Microsoft Bing Video Search API
  slug: microsoft-bing-video-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-bing/refs/heads/main/openapi/microsoft-bing-video-search-api-openapi.yml
- filename: microsoft-bing-visual-search-api-openapi.yml
  format: yaml
  label: Microsoft Bing Visual search API
  slug: microsoft-bing-visual-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-bing/refs/heads/main/openapi/microsoft-bing-visual-search-api-openapi.yml
- filename: microsoft-bing-web-search-api-openapi.yml
  format: yaml
  label: Microsoft Bing Web Search API
  slug: microsoft-bing-web-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-bing/refs/heads/main/openapi/microsoft-bing-web-search-api-openapi.yml
consequence_counts:
  read: 9
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Microsoft Bing Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'Microsoft Bing exposes 10 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Microsoft Bing
provider_slug: microsoft-bing
slug: microsoft-bing-agentic-access
source_filename: microsoft-bing-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/microsoft-bing-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 9\n    acting: 1\n  by_consequence:\n    read: 9\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v7.0/search\n  method: get\n  operationId: webSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v7.0/images/search\n  method: get\n  operationId: imageSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v7.0/news/search\n  method: get\n\
  \  operationId: newsSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v7.0/news\n  method: get\n  operationId: newsTrending\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v7.0/videos/search\n  method: get\n  operationId: videoSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v7.0/entities\n  method: get\n  operationId: entitySearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v7.0/images/visualsearch\n  method: post\n  operationId: visualSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v7.0/custom/search\n  method: get\n  operationId: customSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v7.0/spellcheck\n  method: get\n  operationId: spellCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v7.0/suggestions\n  method: get\n  operationId: autosuggest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-bing/refs/heads/main/agentic-access/microsoft-bing-agentic-access.yml
summary_line: 10 operations · 1 acting
tags:
- Search
- Web Search
- Image
- Video
- News
- Azure AI
- Autosuggest
- Visual Search
---
