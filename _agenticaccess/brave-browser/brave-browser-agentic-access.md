---
acting_count: 0
action_class_counts:
  connected: 9
api_specs:
- filename: brave-browser-images-api-openapi.yml
  format: yaml
  label: Brave Images API
  slug: brave-browser-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brave-browser/refs/heads/main/openapi/brave-browser-images-api-openapi.yml
- filename: brave-browser-local-api-openapi.yml
  format: yaml
  label: Brave Local API
  slug: brave-browser-local-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brave-browser/refs/heads/main/openapi/brave-browser-local-api-openapi.yml
- filename: brave-browser-news-api-openapi.yml
  format: yaml
  label: Brave News API
  slug: brave-browser-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brave-browser/refs/heads/main/openapi/brave-browser-news-api-openapi.yml
- filename: brave-browser-spellcheck-api-openapi.yml
  format: yaml
  label: Brave Spellcheck API
  slug: brave-browser-spellcheck-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brave-browser/refs/heads/main/openapi/brave-browser-spellcheck-api-openapi.yml
- filename: brave-browser-suggest-api-openapi.yml
  format: yaml
  label: Brave Suggest API
  slug: brave-browser-suggest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brave-browser/refs/heads/main/openapi/brave-browser-suggest-api-openapi.yml
- filename: brave-browser-summarizer-api-openapi.yml
  format: yaml
  label: Brave Summarizer API
  slug: brave-browser-summarizer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brave-browser/refs/heads/main/openapi/brave-browser-summarizer-api-openapi.yml
- filename: brave-browser-videos-api-openapi.yml
  format: yaml
  label: Brave Videos API
  slug: brave-browser-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brave-browser/refs/heads/main/openapi/brave-browser-videos-api-openapi.yml
- filename: brave-browser-web-api-openapi.yml
  format: yaml
  label: Brave Web API
  slug: brave-browser-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brave-browser/refs/heads/main/openapi/brave-browser-web-api-openapi.yml
consequence_counts:
  read: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Brave Browser Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Brave exposes 9 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Brave
provider_slug: brave-browser
slug: brave-browser-agentic-access
source_filename: brave-browser-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/brave-browser-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 9\n  by_consequence:\n    read: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /web/search\n  method: get\n  operationId: webSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /news/search\n  method: get\n  operationId: newsSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /images/search\n  method: get\n  operationId: imageSearch\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /videos/search\n  method: get\n  operationId: videoSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /suggest/search\n  method: get\n  operationId: suggestSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spellcheck/search\n  method: get\n  operationId: spellcheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /summarizer/search\n  method: get\n  operationId: summarizer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /local/pois\n\
  \  method: get\n  operationId: localPois\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /local/descriptions\n  method: get\n  operationId: localDescriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brave-browser/refs/heads/main/agentic-access/brave-browser-agentic-access.yml
summary_line: 9 operations
tags:
- Browser
- Search
- Privacy
- Chromium
- Web3
- AI
- Advertising
---
