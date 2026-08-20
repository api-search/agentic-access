---
acting_count: 0
action_class_counts:
  connected: 15
api_specs:
- filename: burger-singh-pages-api-openapi.yml
  format: yaml
  label: Burger Singh Pages API
  slug: burger-singh-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/burger-singh/refs/heads/main/openapi/burger-singh-pages-api-openapi.yml
- filename: burger-singh-media-api-openapi.yml
  format: yaml
  label: Burger Singh Media API
  slug: burger-singh-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/burger-singh/refs/heads/main/openapi/burger-singh-media-api-openapi.yml
- filename: burger-singh-taxonomy-api-openapi.yml
  format: yaml
  label: Burger Singh Taxonomy API
  slug: burger-singh-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/burger-singh/refs/heads/main/openapi/burger-singh-taxonomy-api-openapi.yml
- filename: burger-singh-search-api-openapi.yml
  format: yaml
  label: Burger Singh Search API
  slug: burger-singh-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/burger-singh/refs/heads/main/openapi/burger-singh-search-api-openapi.yml
- filename: burger-singh-discovery-api-openapi.yml
  format: yaml
  label: Burger Singh Discovery API
  slug: burger-singh-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/burger-singh/refs/heads/main/openapi/burger-singh-discovery-api-openapi.yml
- filename: burger-singh-seo-api-openapi.yml
  format: yaml
  label: Burger Singh SEO Metadata API
  slug: burger-singh-seo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/burger-singh/refs/heads/main/openapi/burger-singh-seo-api-openapi.yml
consequence_counts:
  read: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Burger Singh Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'Burger Singh exposes 15 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Burger Singh
provider_slug: burger-singh
slug: burger-singh-agentic-access
source_filename: burger-singh-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: generated\nsource: openapi/burger-singh-discovery-api-openapi.yml, openapi/burger-singh-media-api-openapi.yml,\n  openapi/burger-singh-pages-api-openapi.yml, openapi/burger-singh-search-api-openapi.yml, openapi/burger-singh-seo-api-openapi.yml,\n  openapi/burger-singh-taxonomy-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 15\n  by_consequence:\n    read: 15\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: getRootIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/types\n  method: get\n  operationId: listTypes\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/taxonomies\n  method: get\n  operationId: listTaxonomies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/statuses\n  method: get\n  operationId: listStatuses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/media\n  method: get\n  operationId: listMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /wp/v2/media/{id}\n  method: get\n  operationId: getMediaItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/pages\n  method: get\n  operationId: listPages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/pages/{id}\n  method: get\n  operationId: getPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/search\n  method: get\n  operationId: searchContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /yoast/v1/get_head\n  method: get\n  operationId: getSeoHead\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/categories\n  method: get\n  operationId: listCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/categories/{id}\n  method: get\n  operationId: getCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/tags\n  method: get\n  operationId: listTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/tags/{id}\n  method: get\n  operationId: getTag\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/burger-singh/refs/heads/main/agentic-access/burger-singh-agentic-access.yml
summary_line: 15 operations
tags:
- Company
- Restaurant
- Quick Service Restaurant
- Food and Beverage
- Franchising
- Consumer
- India
- Retail
- Content
- WordPress
---
