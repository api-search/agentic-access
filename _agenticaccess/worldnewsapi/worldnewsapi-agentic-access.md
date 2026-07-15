---
acting_count: 0
action_class_counts:
  connected: 8
api_specs:
- filename: worldnewsapi-openapi.yml
  format: yaml
  label: World News Search News API
  slug: worldnewsapi-search-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worldnewsapi/refs/heads/main/openapi/worldnewsapi-openapi.yml
- filename: worldnewsapi-openapi.yml
  format: yaml
  label: World News Geo Coordinates API
  slug: worldnewsapi-geo-coordinates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worldnewsapi/refs/heads/main/openapi/worldnewsapi-openapi.yml
- filename: worldnewsapi-openapi.yml
  format: yaml
  label: World News Top News API
  slug: worldnewsapi-top-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worldnewsapi/refs/heads/main/openapi/worldnewsapi-openapi.yml
- filename: worldnewsapi-openapi.yml
  format: yaml
  label: World News Extract News API
  slug: worldnewsapi-extract-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worldnewsapi/refs/heads/main/openapi/worldnewsapi-openapi.yml
- filename: worldnewsapi-openapi.yml
  format: yaml
  label: World News Retrieve News API
  slug: worldnewsapi-retrieve-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worldnewsapi/refs/heads/main/openapi/worldnewsapi-openapi.yml
- filename: worldnewsapi-openapi.yml
  format: yaml
  label: World News Sources API
  slug: worldnewsapi-news-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worldnewsapi/refs/heads/main/openapi/worldnewsapi-openapi.yml
- filename: worldnewsapi-openapi.yml
  format: yaml
  label: World News Front Pages API
  slug: worldnewsapi-front-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worldnewsapi/refs/heads/main/openapi/worldnewsapi-openapi.yml
consequence_counts:
  read: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Worldnewsapi Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'World News API exposes 8 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: World News API
provider_slug: worldnewsapi
slug: worldnewsapi-agentic-access
source_filename: worldnewsapi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/worldnewsapi-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 8\n  by_consequence:\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /search-news\n  method: get\n  operationId: searchNews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /top-news\n  method: get\n  operationId: topNews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retrieve-news\n  method: get\n  operationId: retrieveNews\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /extract-news\n  method: get\n  operationId: extractNews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /extract-news-links\n  method: get\n  operationId: extractNewsLinks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search-news-sources\n  method: get\n  operationId: searchNewsSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /retrieve-front-page\n  method: get\n  operationId: retrieveFrontPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /geo-coordinates\n  method: get\n  operationId: getGeoCoordinates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/worldnewsapi/refs/heads/main/agentic-access/worldnewsapi-agentic-access.yml
summary_line: 8 operations
tags:
- News
- Local News
- News Search
- Media Monitoring
- Geo Search
- News Data
- Sentiment Analysis
- Content Extraction
---
