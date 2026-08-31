---
acting_count: 0
action_class_counts:
  connected: 22
api_specs:
- filename: housesigma-comments-api-openapi.yml
  format: yaml
  label: HouseSigma Comments API
  slug: housesigma-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/housesigma/refs/heads/main/openapi/housesigma-comments-api-openapi.yml
- filename: housesigma-media-api-openapi.yml
  format: yaml
  label: HouseSigma Media API
  slug: housesigma-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/housesigma/refs/heads/main/openapi/housesigma-media-api-openapi.yml
- filename: housesigma-oembed-api-openapi.yml
  format: yaml
  label: HouseSigma O Embed API
  slug: housesigma-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/housesigma/refs/heads/main/openapi/housesigma-oembed-api-openapi.yml
- filename: housesigma-pages-api-openapi.yml
  format: yaml
  label: HouseSigma Pages API
  slug: housesigma-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/housesigma/refs/heads/main/openapi/housesigma-pages-api-openapi.yml
- filename: housesigma-posts-api-openapi.yml
  format: yaml
  label: HouseSigma Posts API
  slug: housesigma-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/housesigma/refs/heads/main/openapi/housesigma-posts-api-openapi.yml
- filename: housesigma-search-api-openapi.yml
  format: yaml
  label: HouseSigma Search API
  slug: housesigma-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/housesigma/refs/heads/main/openapi/housesigma-search-api-openapi.yml
- filename: housesigma-taxonomies-api-openapi.yml
  format: yaml
  label: HouseSigma Taxonomies API
  slug: housesigma-taxonomies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/housesigma/refs/heads/main/openapi/housesigma-taxonomies-api-openapi.yml
- filename: housesigma-types-api-openapi.yml
  format: yaml
  label: HouseSigma Types API
  slug: housesigma-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/housesigma/refs/heads/main/openapi/housesigma-types-api-openapi.yml
- filename: housesigma-users-api-openapi.yml
  format: yaml
  label: HouseSigma Users API
  slug: housesigma-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/housesigma/refs/heads/main/openapi/housesigma-users-api-openapi.yml
consequence_counts:
  read: 22
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Housesigma Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'HouseSigma exposes 22 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: HouseSigma
provider_slug: housesigma
slug: housesigma-agentic-access
source_filename: housesigma-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: generated\nsource: openapi/housesigma-blog-content-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 22\n  by_consequence:\n    read: 22\n  human_in_the_loop_required: 0\noperations:\n- path: /wp/v2/posts\n  method: get\n  operationId: listPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/posts/{id}\n  method: get\n  operationId: getPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/pages\n  method: get\n  operationId: listPages\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/pages/{id}\n  method: get\n  operationId: getPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/media\n  method: get\n  operationId: listMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/media/{id}\n  method: get\n  operationId: getMediaItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/categories\n  method: get\n  operationId: listCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /wp/v2/categories/{id}\n  method: get\n  operationId: getCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/tags\n  method: get\n  operationId: listTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/tags/{id}\n  method: get\n  operationId: getTag\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/users/{id}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/comments\n  method: get\n  operationId: listComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/comments/{id}\n  method: get\n  operationId: getComment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/search\n  method: get\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/taxonomies\n  method: get\n  operationId: listTaxonomies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/taxonomies/{taxonomy}\n  method: get\n  operationId: getTaxonomy\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/types\n  method: get\n  operationId: listTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/types/{type}\n  method: get\n  operationId: getType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/statuses\n  method: get\n  operationId: listStatuses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/statuses/{status}\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oembed/1.0/embed\n\
  \  method: get\n  operationId: getOembed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/housesigma/refs/heads/main/agentic-access/housesigma-agentic-access.yml
summary_line: 22 operations
tags:
- Real-Estate
- Canada
- Property Listings
- MLS
- Valuation
- AVM
- PropTech
- Rentals
- Blog
- Content
- WordPress
- oEmbed
- Ontario
- British Columbia
- Toronto
---
