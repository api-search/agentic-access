---
acting_count: 10
action_class_counts:
  acting: 10
api_specs:
- filename: serper-autocomplete-api-openapi.yml
  format: yaml
  label: Serper Autocomplete API
  slug: serper-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-autocomplete-api-openapi.yml
- filename: serper-images-api-openapi.yml
  format: yaml
  label: Serper Images API
  slug: serper-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-images-api-openapi.yml
- filename: serper-lens-api-openapi.yml
  format: yaml
  label: Serper Lens API
  slug: serper-lens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-lens-api-openapi.yml
- filename: serper-locations-api-openapi.yml
  format: yaml
  label: Serper Locations API
  slug: serper-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-locations-api-openapi.yml
- filename: serper-maps-api-openapi.yml
  format: yaml
  label: Serper Maps API
  slug: serper-maps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-maps-api-openapi.yml
- filename: serper-news-api-openapi.yml
  format: yaml
  label: Serper News API
  slug: serper-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-news-api-openapi.yml
- filename: serper-patents-api-openapi.yml
  format: yaml
  label: Serper Patents API
  slug: serper-patents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-patents-api-openapi.yml
- filename: serper-places-api-openapi.yml
  format: yaml
  label: Serper Places API
  slug: serper-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-places-api-openapi.yml
- filename: serper-reviews-api-openapi.yml
  format: yaml
  label: Serper Reviews API
  slug: serper-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-reviews-api-openapi.yml
- filename: serper-scholar-api-openapi.yml
  format: yaml
  label: Serper Scholar API
  slug: serper-scholar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-scholar-api-openapi.yml
- filename: serper-search-api-openapi.yml
  format: yaml
  label: Serper Search API
  slug: serper-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-search-api-openapi.yml
- filename: serper-shopping-api-openapi.yml
  format: yaml
  label: Serper Shopping API
  slug: serper-shopping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-shopping-api-openapi.yml
- filename: serper-videos-api-openapi.yml
  format: yaml
  label: Serper Videos API
  slug: serper-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-videos-api-openapi.yml
- filename: serper-webpage-scrape-api-openapi.yml
  format: yaml
  label: Serper Webpage Scrape API
  slug: serper-webpage-scrape-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/openapi/serper-webpage-scrape-api-openapi.yml
consequence_counts:
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Serper Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'Serper exposes 10 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Serper
provider_slug: serper
slug: serper-agentic-access
source_filename: serper-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/serper-google-search-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    acting: 10\n  by_consequence:\n    write: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /search\n  method: post\n  operationId: webSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /images\n  method: post\n  operationId: imageSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /news\n  method: post\n  operationId: newsSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /maps\n  method: post\n  operationId: mapsSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /places\n  method: post\n  operationId: placesSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /videos\n  method: post\n  operationId: videoSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shopping\n  method: post\n  operationId: shoppingSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scholar\n  method: post\n  operationId: scholarSearch\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /patents\n  method: post\n  operationId: patentsSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /autocomplete\n  method: post\n  operationId: autocomplete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/serper/refs/heads/main/agentic-access/serper-agentic-access.yml
summary_line: 10 operations · 10 acting
tags:
- Search
- SERP
- Google Search
- AI
- LLM
- SEO
- Images
- News
- Maps
- Shopping
- Reviews
- Lens
- Scraping
- Locations
- SERP API
- Web Search
- Agents
- Patents
- Scholar
- Autocomplete
- Places
- Videos
---
