---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 22
api_specs:
- filename: litescrape-apple-api-openapi.yml
  format: yaml
  label: Litescrape Apple API
  slug: litescrape-apple-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litescrape/refs/heads/main/openapi/litescrape-apple-api-openapi.yml
- filename: litescrape-bing-api-openapi.yml
  format: yaml
  label: Litescrape Bing API
  slug: litescrape-bing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litescrape/refs/heads/main/openapi/litescrape-bing-api-openapi.yml
- filename: litescrape-duckduckgo-api-openapi.yml
  format: yaml
  label: Litescrape Duckduckgo API
  slug: litescrape-duckduckgo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litescrape/refs/heads/main/openapi/litescrape-duckduckgo-api-openapi.yml
- filename: litescrape-google-api-openapi.yml
  format: yaml
  label: Litescrape Google API
  slug: litescrape-google-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litescrape/refs/heads/main/openapi/litescrape-google-api-openapi.yml
- filename: litescrape-tripadvisor-api-openapi.yml
  format: yaml
  label: Litescrape Tripadvisor API
  slug: litescrape-tripadvisor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litescrape/refs/heads/main/openapi/litescrape-tripadvisor-api-openapi.yml
- filename: litescrape-yelp-api-openapi.yml
  format: yaml
  label: Litescrape Yelp API
  slug: litescrape-yelp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litescrape/refs/heads/main/openapi/litescrape-yelp-api-openapi.yml
- filename: litescrape-zeroclick-api-openapi.yml
  format: yaml
  label: Litescrape Zeroclick API
  slug: litescrape-zeroclick-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litescrape/refs/heads/main/openapi/litescrape-zeroclick-api-openapi.yml
consequence_counts:
  physical: 1
  read: 22
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Litescrape Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /zeroclick/agent/quote
operation_count: 23
overview: 'Litescrape exposes 23 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Litescrape
provider_slug: litescrape
slug: litescrape-agentic-access
source_filename: litescrape-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: generated\nsource: openapi/litescrape-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 22\n    acting: 1\n  by_consequence:\n    read: 22\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/apple/maps/places\n  method: get\n  operationId: apple_maps_places\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/apple/maps/reviews\n  method: get\n  operationId: apple_maps_reviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/bing/maps\n\
  \  method: get\n  operationId: bing_maps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/bing/search\n  method: get\n  operationId: bing_search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/duckduckgo/maps\n  method: get\n  operationId: duckduckgo_maps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/duckduckgo/search\n  method: get\n  operationId: duckduckgo_search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/google/ai-mode\n  method: get\n  operationId: google_ai_mode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/google/ai-overview\n  method: get\n  operationId: google_ai_overview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/google/contributor-reviews\n  method: get\n  operationId: google_contributor_reviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/google/maps\n  method: get\n  operationId: google_maps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/google/maps/photo-meta\n  method: get\n  operationId: google_maps_photo_meta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/google/maps/popular-times\n  method: get\n  operationId: google_maps_popular_times\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/google/maps/posts\n  method: get\n  operationId: google_maps_posts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/google/reviews\n  method: get\n  operationId: google_reviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/google/search\n  method: get\n  operationId: google_search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/google/shopping\n  method: get\n  operationId: google_shopping\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/google/shopping/product\n  method: get\n  operationId: google_shopping_product\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tripadvisor/place\n  method: get\n  operationId: tripadvisor_place\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tripadvisor/reviews\n  method: get\n  operationId: tripadvisor_reviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tripadvisor/search\n  method: get\n  operationId: tripadvisor_search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/yelp/reviews\n  method: get\n  operationId: yelp_reviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/yelp/search\n  method: get\n  operationId: yelp_search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /zeroclick/agent/quote\n  method: post\n  operationId: sellerAgentQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/litescrape/refs/heads/main/agentic-access/litescrape-agentic-access.yml
summary_line: 23 operations · 1 acting
tags:
- Company
- SERP API
- Web Scraping
- Search
- Google Maps
- Reviews
- Web Data
- MCP
---
