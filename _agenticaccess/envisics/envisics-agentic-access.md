---
acting_count: 0
action_class_counts:
  connected: 21
api_specs:
- filename: envisics-posts-api-openapi.yml
  format: yaml
  label: Envisics Posts API
  slug: envisics-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envisics/refs/heads/main/openapi/envisics-posts-api-openapi.yml
- filename: envisics-pages-api-openapi.yml
  format: yaml
  label: Envisics Pages API
  slug: envisics-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envisics/refs/heads/main/openapi/envisics-pages-api-openapi.yml
- filename: envisics-media-api-openapi.yml
  format: yaml
  label: Envisics Media API
  slug: envisics-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envisics/refs/heads/main/openapi/envisics-media-api-openapi.yml
- filename: envisics-taxonomy-api-openapi.yml
  format: yaml
  label: Envisics Taxonomy API
  slug: envisics-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envisics/refs/heads/main/openapi/envisics-taxonomy-api-openapi.yml
- filename: envisics-search-api-openapi.yml
  format: yaml
  label: Envisics Search API
  slug: envisics-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envisics/refs/heads/main/openapi/envisics-search-api-openapi.yml
- filename: envisics-discovery-api-openapi.yml
  format: yaml
  label: Envisics Discovery API
  slug: envisics-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envisics/refs/heads/main/openapi/envisics-discovery-api-openapi.yml
- filename: envisics-oembed-api-openapi.yml
  format: yaml
  label: Envisics oEmbed API
  slug: envisics-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envisics/refs/heads/main/openapi/envisics-oembed-api-openapi.yml
- filename: envisics-seo-api-openapi.yml
  format: yaml
  label: Envisics SEO Metadata API
  slug: envisics-seo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envisics/refs/heads/main/openapi/envisics-seo-api-openapi.yml
consequence_counts:
  read: 21
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Envisics Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 21
overview: 'Envisics exposes 21 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Envisics
provider_slug: envisics
slug: envisics-agentic-access
source_filename: envisics-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: generated\nsource: openapi/envisics-discovery-api-openapi.yml, openapi/envisics-media-api-openapi.yml,\n  openapi/envisics-oembed-api-openapi.yml, openapi/envisics-pages-api-openapi.yml, openapi/envisics-posts-api-openapi.yml,\n  openapi/envisics-search-api-openapi.yml, openapi/envisics-seo-api-openapi.yml, openapi/envisics-taxonomy-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    connected: 21\n  by_consequence:\n    read: 21\n  human_in_the_loop_required: 0\noperations:\n- path: /wp/v2/types\n  method: get\n  operationId: listTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /wp/v2/types/{type}\n  method: get\n  operationId: getType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/taxonomies\n  method: get\n  operationId: listTaxonomies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/taxonomies/{taxonomy}\n  method: get\n  operationId: getTaxonomy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/statuses\n  method: get\n  operationId: listStatuses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/statuses/{status}\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/users/{id}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/media\n  method: get\n  operationId: listMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/media/{id}\n  method: get\n  operationId: getMediaItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oembed/1.0/embed\n  method: get\n  operationId:\
  \ getOEmbed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/pages\n  method: get\n  operationId: listPages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/pages/{id}\n  method: get\n  operationId: getPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/posts\n  method: get\n  operationId: listPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/posts/{id}\n  method: get\n  operationId: getPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /wp/v2/search\n  method: get\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /yoast/v1/get_head\n  method: get\n  operationId: getSeoHead\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/categories\n  method: get\n  operationId: listCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/categories/{id}\n  method: get\n  operationId: getCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/tags\n  method: get\n  operationId: listTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/tags/{id}\n  method: get\n  operationId: getTag\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/envisics/refs/heads/main/agentic-access/envisics-agentic-access.yml
summary_line: 21 operations
tags:
- Company
- Automotive
- Augmented Reality
- Holography
- Head-Up Display
- Photonics
- Optics
- Deep Technology
- Hardware
- Advanced Manufacturing
- Content
---
