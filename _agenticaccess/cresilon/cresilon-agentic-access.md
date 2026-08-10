---
acting_count: 0
action_class_counts:
  connected: 22
api_specs:
- filename: cresilon-posts-api-openapi.yml
  format: yaml
  label: Cresilon News & Press Releases API
  slug: cresilon-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cresilon/refs/heads/main/openapi/cresilon-posts-api-openapi.yml
- filename: cresilon-pages-api-openapi.yml
  format: yaml
  label: Cresilon Pages API
  slug: cresilon-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cresilon/refs/heads/main/openapi/cresilon-pages-api-openapi.yml
- filename: cresilon-media-api-openapi.yml
  format: yaml
  label: Cresilon Media API
  slug: cresilon-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cresilon/refs/heads/main/openapi/cresilon-media-api-openapi.yml
- filename: cresilon-taxonomy-api-openapi.yml
  format: yaml
  label: Cresilon Taxonomy API
  slug: cresilon-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cresilon/refs/heads/main/openapi/cresilon-taxonomy-api-openapi.yml
- filename: cresilon-search-api-openapi.yml
  format: yaml
  label: Cresilon Search API
  slug: cresilon-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cresilon/refs/heads/main/openapi/cresilon-search-api-openapi.yml
- filename: cresilon-discovery-api-openapi.yml
  format: yaml
  label: Cresilon Discovery API
  slug: cresilon-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cresilon/refs/heads/main/openapi/cresilon-discovery-api-openapi.yml
- filename: cresilon-oembed-api-openapi.yml
  format: yaml
  label: Cresilon oEmbed API
  slug: cresilon-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cresilon/refs/heads/main/openapi/cresilon-oembed-api-openapi.yml
- filename: cresilon-seo-api-openapi.yml
  format: yaml
  label: Cresilon SEO Metadata API
  slug: cresilon-seo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cresilon/refs/heads/main/openapi/cresilon-seo-api-openapi.yml
- filename: cresilon-authors-api-openapi.yml
  format: yaml
  label: Cresilon Authors API
  slug: cresilon-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cresilon/refs/heads/main/openapi/cresilon-authors-api-openapi.yml
- filename: cresilon-comments-api-openapi.yml
  format: yaml
  label: Cresilon Comments API
  slug: cresilon-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cresilon/refs/heads/main/openapi/cresilon-comments-api-openapi.yml
consequence_counts:
  read: 22
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cresilon Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'Cresilon exposes 22 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cresilon
provider_slug: cresilon
slug: cresilon-agentic-access
source_filename: cresilon-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: generated\nsource: openapi/cresilon-discovery-api-openapi.yml, openapi/cresilon-media-api-openapi.yml,\n  openapi/cresilon-oembed-api-openapi.yml, openapi/cresilon-pages-api-openapi.yml, openapi/cresilon-posts-api-openapi.yml,\n  openapi/cresilon-search-api-openapi.yml, openapi/cresilon-seo-api-openapi.yml, openapi/cresilon-taxonomy-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 22\n  by_consequence:\n    read: 22\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: getRouteIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /wp/v2/types\n  method: get\n  operationId: listTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/types/{type}\n  method: get\n  operationId: getType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/taxonomies\n  method: get\n  operationId: listTaxonomies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/taxonomies/{taxonomy}\n  method: get\n  operationId: getTaxonomy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/statuses\n  method: get\n  operationId: listStatuses\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/users/{id}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/media\n  method: get\n  operationId: listMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/media/{id}\n  method: get\n  operationId: getMediaItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oembed/1.0/embed\n  method: get\n  operationId: getOEmbed\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/pages\n  method: get\n  operationId: listPages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/pages/{id}\n  method: get\n  operationId: getPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/posts\n  method: get\n  operationId: listPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/posts/{id}\n  method: get\n  operationId: getPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/comments\n  method:\
  \ get\n  operationId: listComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/search\n  method: get\n  operationId: searchContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /yoast/v1/get_head\n  method: get\n  operationId: getYoastHead\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/categories\n  method: get\n  operationId: listCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/categories/{id}\n  method: get\n  operationId: getCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/tags\n  method: get\n  operationId: listTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/tags/{id}\n  method: get\n  operationId: getTag\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cresilon/refs/heads/main/agentic-access/cresilon-agentic-access.yml
summary_line: 22 operations
tags:
- Company
- Biotechnology
- Medical Devices
- Health
- Hemostasis
- Wound Care
- Trauma Care
- Veterinary
- Life Sciences
- Manufacturing
- Content
---
