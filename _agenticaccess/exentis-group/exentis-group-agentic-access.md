---
acting_count: 0
action_class_counts:
  connected: 14
api_specs:
- filename: exentis-group-posts-api-openapi.yml
  format: yaml
  label: Exentis Group Posts API
  slug: exentis-group-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exentis-group/refs/heads/main/openapi/exentis-group-posts-api-openapi.yml
- filename: exentis-group-blog-api-openapi.yml
  format: yaml
  label: Exentis Group Blog API
  slug: exentis-group-blog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exentis-group/refs/heads/main/openapi/exentis-group-blog-api-openapi.yml
- filename: exentis-group-pages-api-openapi.yml
  format: yaml
  label: Exentis Group Pages API
  slug: exentis-group-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exentis-group/refs/heads/main/openapi/exentis-group-pages-api-openapi.yml
- filename: exentis-group-media-api-openapi.yml
  format: yaml
  label: Exentis Group Media API
  slug: exentis-group-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exentis-group/refs/heads/main/openapi/exentis-group-media-api-openapi.yml
- filename: exentis-group-categories-api-openapi.yml
  format: yaml
  label: Exentis Group Categories API
  slug: exentis-group-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exentis-group/refs/heads/main/openapi/exentis-group-categories-api-openapi.yml
- filename: exentis-group-search-api-openapi.yml
  format: yaml
  label: Exentis Group Search API
  slug: exentis-group-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exentis-group/refs/heads/main/openapi/exentis-group-search-api-openapi.yml
- filename: exentis-group-languages-api-openapi.yml
  format: yaml
  label: Exentis Group Languages API
  slug: exentis-group-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exentis-group/refs/heads/main/openapi/exentis-group-languages-api-openapi.yml
- filename: exentis-group-taxonomy-api-openapi.yml
  format: yaml
  label: Exentis Group Taxonomy API
  slug: exentis-group-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exentis-group/refs/heads/main/openapi/exentis-group-taxonomy-api-openapi.yml
consequence_counts:
  read: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Exentis Group Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'Exentis Group exposes 14 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Exentis Group
provider_slug: exentis-group
slug: exentis-group-agentic-access
source_filename: exentis-group-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: generated\nsource: openapi/exentis-group-blog-api-openapi.yml, openapi/exentis-group-blog-categories-api-openapi.yml,\n  openapi/exentis-group-categories-api-openapi.yml, openapi/exentis-group-languages-api-openapi.yml,\n  openapi/exentis-group-media-api-openapi.yml, openapi/exentis-group-pages-api-openapi.yml,\n  openapi/exentis-group-posts-api-openapi.yml, openapi/exentis-group-search-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 14\n  by_consequence:\n    read: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /wp/v2/blogposts\n  method: get\n  operationId: listBlogPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/blogposts/{id}\n  method: get\n  operationId: getBlogPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/blogkategorie\n  method: get\n  operationId: listBlogCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/blogkategorie/{id}\n  method: get\n  operationId: getBlogCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/categories\n  method: get\n  operationId: listCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/categories/{id}\n\
  \  method: get\n  operationId: getCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pll/v1/languages\n  method: get\n  operationId: listLanguages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/media\n  method: get\n  operationId: listMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/media/{id}\n  method: get\n  operationId: getMediaItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/pages\n  method: get\n  operationId: listPages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /wp/v2/pages/{id}\n  method: get\n  operationId: getPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/posts\n  method: get\n  operationId: listPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/posts/{id}\n  method: get\n  operationId: getPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/search\n  method: get\n  operationId: searchSite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exentis-group/refs/heads/main/agentic-access/exentis-group-agentic-access.yml
summary_line: 14 operations
tags:
- Company
- Additive Manufacturing
- 3D Printing
- Industrial Manufacturing
- Advanced Materials
- Technical Ceramics
- Metals
- Pharmaceutical Manufacturing
- New Energy
- Switzerland
- Hardware
- Content
---
