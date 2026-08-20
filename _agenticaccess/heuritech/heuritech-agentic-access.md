---
acting_count: 0
action_class_counts:
  connected: 21
api_specs:
- filename: heuritech-posts-api-openapi.yml
  format: yaml
  label: Heuritech Posts API
  slug: heuritech-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heuritech/refs/heads/main/openapi/heuritech-posts-api-openapi.yml
- filename: heuritech-pages-api-openapi.yml
  format: yaml
  label: Heuritech Pages API
  slug: heuritech-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heuritech/refs/heads/main/openapi/heuritech-pages-api-openapi.yml
- filename: heuritech-media-api-openapi.yml
  format: yaml
  label: Heuritech Media API
  slug: heuritech-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heuritech/refs/heads/main/openapi/heuritech-media-api-openapi.yml
- filename: heuritech-comments-api-openapi.yml
  format: yaml
  label: Heuritech Comments API
  slug: heuritech-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heuritech/refs/heads/main/openapi/heuritech-comments-api-openapi.yml
- filename: heuritech-taxonomy-api-openapi.yml
  format: yaml
  label: Heuritech Taxonomy API
  slug: heuritech-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heuritech/refs/heads/main/openapi/heuritech-taxonomy-api-openapi.yml
- filename: heuritech-users-api-openapi.yml
  format: yaml
  label: Heuritech Users API
  slug: heuritech-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heuritech/refs/heads/main/openapi/heuritech-users-api-openapi.yml
- filename: heuritech-search-api-openapi.yml
  format: yaml
  label: Heuritech Search API
  slug: heuritech-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heuritech/refs/heads/main/openapi/heuritech-search-api-openapi.yml
- filename: heuritech-discovery-api-openapi.yml
  format: yaml
  label: Heuritech Discovery API
  slug: heuritech-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heuritech/refs/heads/main/openapi/heuritech-discovery-api-openapi.yml
consequence_counts:
  read: 21
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Heuritech Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 21
overview: 'Heuritech exposes 21 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Heuritech
provider_slug: heuritech
slug: heuritech-agentic-access
source_filename: heuritech-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: generated\nsource: openapi/heuritech-comments-api-openapi.yml, openapi/heuritech-discovery-api-openapi.yml,\n  openapi/heuritech-media-api-openapi.yml, openapi/heuritech-pages-api-openapi.yml, openapi/heuritech-posts-api-openapi.yml,\n  openapi/heuritech-search-api-openapi.yml, openapi/heuritech-taxonomy-api-openapi.yml, openapi/heuritech-users-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    connected: 21\n  by_consequence:\n    read: 21\n  human_in_the_loop_required: 0\noperations:\n- path: /wp/v2/comments\n  method: get\n  operationId: getComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /wp/v2/comments/{id}\n  method: get\n  operationId: getCommentsId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/types\n  method: get\n  operationId: getTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/types/{type}\n  method: get\n  operationId: getTypesType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/taxonomies\n  method: get\n  operationId: getTaxonomies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/taxonomies/{taxonomy}\n  method: get\n  operationId: getTaxonomiesTaxonomy\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/statuses\n  method: get\n  operationId: getStatuses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/statuses/{status}\n  method: get\n  operationId: getStatusesStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/media\n  method: get\n  operationId: getMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/media/{id}\n  method: get\n  operationId: getMediaId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /wp/v2/pages\n  method: get\n  operationId: getPages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/pages/{id}\n  method: get\n  operationId: getPagesId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/posts\n  method: get\n  operationId: getPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/posts/{id}\n  method: get\n  operationId: getPostsId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/search\n  method: get\n  operationId: getSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/categories\n  method: get\n  operationId: getCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/categories/{id}\n  method: get\n  operationId: getCategoriesId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/tags\n  method: get\n  operationId: getTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/tags/{id}\n  method: get\n  operationId: getTagsId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/users\n  method: get\n  operationId: getUsers\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/users/{id}\n  method: get\n  operationId: getUsersId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heuritech/refs/heads/main/agentic-access/heuritech-agentic-access.yml
summary_line: 21 operations
tags:
- Company
- Artificial Intelligence
- Computer-Vision
- Machine-Learning
- Fashion
- Trend Forecasting
- Demand Forecasting
- Retail
- Luxury
- Market Intelligence
- Consumer Insights
- Social Media Analytics
- Content
---
