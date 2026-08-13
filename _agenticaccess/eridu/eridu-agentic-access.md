---
acting_count: 0
action_class_counts:
  connected: 20
api_specs:
- filename: eridu-content-api-openapi.yml
  format: yaml
  label: Eridu Content API
  slug: eridu-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eridu/refs/heads/main/openapi/eridu-content-api-openapi.yml
- filename: eridu-pages-api-openapi.yml
  format: yaml
  label: Eridu Pages API
  slug: eridu-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eridu/refs/heads/main/openapi/eridu-pages-api-openapi.yml
- filename: eridu-media-api-openapi.yml
  format: yaml
  label: Eridu Media API
  slug: eridu-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eridu/refs/heads/main/openapi/eridu-media-api-openapi.yml
- filename: eridu-taxonomy-api-openapi.yml
  format: yaml
  label: Eridu Taxonomy API
  slug: eridu-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eridu/refs/heads/main/openapi/eridu-taxonomy-api-openapi.yml
- filename: eridu-search-api-openapi.yml
  format: yaml
  label: Eridu Search API
  slug: eridu-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eridu/refs/heads/main/openapi/eridu-search-api-openapi.yml
- filename: eridu-discovery-api-openapi.yml
  format: yaml
  label: Eridu Discovery API
  slug: eridu-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eridu/refs/heads/main/openapi/eridu-discovery-api-openapi.yml
- filename: eridu-oembed-api-openapi.yml
  format: yaml
  label: Eridu oEmbed API
  slug: eridu-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eridu/refs/heads/main/openapi/eridu-oembed-api-openapi.yml
consequence_counts:
  read: 20
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Eridu Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 20
overview: 'Eridu exposes 20 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Eridu
provider_slug: eridu
slug: eridu-agentic-access
source_filename: eridu-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: generated\nsource: openapi/eridu-content-api-openapi.yml, openapi/eridu-discovery-api-openapi.yml, openapi/eridu-media-api-openapi.yml,\n  openapi/eridu-oembed-api-openapi.yml, openapi/eridu-pages-api-openapi.yml, openapi/eridu-search-api-openapi.yml,\n  openapi/eridu-taxonomy-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    connected: 20\n  by_consequence:\n    read: 20\n  human_in_the_loop_required: 0\noperations:\n- path: /wp/v2/posts\n  method: get\n  operationId: listPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/posts/{id}\n  method: get\n  operationId:\
  \ getPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: getApiIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/types\n  method: get\n  operationId: listTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/types/{type}\n  method: get\n  operationId: getType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/taxonomies\n  method: get\n  operationId: listTaxonomies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /wp/v2/taxonomies/{taxonomy}\n  method: get\n  operationId: getTaxonomy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/statuses\n  method: get\n  operationId: listStatuses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/users/{id}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/media\n  method: get\n  operationId: listMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/media/{id}\n  method: get\n  operationId: getMediaItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oembed/1.0/embed\n  method: get\n  operationId: getOembed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/pages\n  method: get\n  operationId: listPages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/pages/{id}\n  method: get\n  operationId: getPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/search\n  method: get\n  operationId: search\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/categories\n  method: get\n  operationId: listCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/categories/{id}\n  method: get\n  operationId: getCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/tags\n  method: get\n  operationId: listTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/tags/{id}\n  method: get\n  operationId: getTag\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eridu/refs/heads/main/agentic-access/eridu-agentic-access.yml
summary_line: 20 operations
tags:
- Company
- Artificial Intelligence
- AI Infrastructure
- Networking
- Semiconductors
- Data Centers
- Silicon
- Network Switching
- Interconnect
- Hardware
- Content
---
