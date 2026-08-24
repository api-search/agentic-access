---
acting_count: 0
action_class_counts:
  connected: 21
api_specs:
- filename: kateeva-posts-api-openapi.yml
  format: yaml
  label: Kateeva Posts API
  slug: kateeva-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kateeva/refs/heads/main/openapi/kateeva-posts-api-openapi.yml
- filename: kateeva-pages-api-openapi.yml
  format: yaml
  label: Kateeva Pages API
  slug: kateeva-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kateeva/refs/heads/main/openapi/kateeva-pages-api-openapi.yml
- filename: kateeva-media-api-openapi.yml
  format: yaml
  label: Kateeva Media API
  slug: kateeva-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kateeva/refs/heads/main/openapi/kateeva-media-api-openapi.yml
- filename: kateeva-taxonomy-api-openapi.yml
  format: yaml
  label: Kateeva Taxonomy API
  slug: kateeva-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kateeva/refs/heads/main/openapi/kateeva-taxonomy-api-openapi.yml
- filename: kateeva-search-api-openapi.yml
  format: yaml
  label: Kateeva Search API
  slug: kateeva-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kateeva/refs/heads/main/openapi/kateeva-search-api-openapi.yml
- filename: kateeva-discovery-api-openapi.yml
  format: yaml
  label: Kateeva Discovery API
  slug: kateeva-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kateeva/refs/heads/main/openapi/kateeva-discovery-api-openapi.yml
- filename: kateeva-oembed-api-openapi.yml
  format: yaml
  label: Kateeva oEmbed API
  slug: kateeva-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kateeva/refs/heads/main/openapi/kateeva-oembed-api-openapi.yml
- filename: kateeva-seo-api-openapi.yml
  format: yaml
  label: Kateeva SEO Metadata API
  slug: kateeva-seo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kateeva/refs/heads/main/openapi/kateeva-seo-api-openapi.yml
consequence_counts:
  read: 21
description: Recommended x-agentic-access execution contracts, classified from the OpenAPI. Every operation on this surface is an anonymous read, so every contract is action-class connected / consequence read with no human-in-the-loop requirement and no audit obligation. A governance starting point for exposing this API to AI agents — review and bind audience per deployment.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Kateeva Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 21
overview: 'Kateeva exposes 21 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Kateeva
provider_slug: kateeva
slug: kateeva-agentic-access
source_filename: kateeva-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: generated\nsource: openapi/kateeva-discovery-api-openapi.yml, openapi/kateeva-media-api-openapi.yml, openapi/kateeva-oembed-api-openapi.yml,\n  openapi/kateeva-pages-api-openapi.yml, openapi/kateeva-posts-api-openapi.yml, openapi/kateeva-search-api-openapi.yml,\n  openapi/kateeva-seo-api-openapi.yml, openapi/kateeva-taxonomy-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified from the OpenAPI. Every operation on this\n  surface is an anonymous read, so every contract is action-class connected / consequence read with no human-in-the-loop\n  requirement and no audit obligation. A governance starting point for exposing this API to AI agents — review and\n  bind audience per deployment.\nsummary:\n  operations: 21\n  by_action_class:\n    connected: 21\n  by_consequence:\n    read: 21\n  human_in_the_loop_required: 0\n  note: There is no write, no purchase, no notification and no destructive operation to classify.\
  \ The write methods\n    that exist on the same WordPress routes are credential-gated with no public issuance path and are therefore\n    out of scope for an agent.\noperations:\n- path: /\n  method: get\n  operationId: getRouteIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/types\n  method: get\n  operationId: listTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/taxonomies\n  method: get\n  operationId: listTaxonomies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/statuses\n  method: get\n  operationId: listStatuses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /wp/v2/users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/users/{id}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/comments\n  method: get\n  operationId: listComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/comments/{id}\n  method: get\n  operationId: getComment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/media\n  method: get\n  operationId: listMedia\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/media/{id}\n  method: get\n  operationId: getMediaItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oembed/1.0/embed\n  method: get\n  operationId: getOEmbed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/pages\n  method: get\n  operationId: listPages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/pages/{id}\n  method: get\n  operationId: getPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/posts\n  method: get\n  operationId: listPosts\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/posts/{id}\n  method: get\n  operationId: getPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/search\n  method: get\n  operationId: searchContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /yoast/v1/get_head\n  method: get\n  operationId: getSeoHead\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/categories\n  method: get\n  operationId: listCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/categories/{id}\n\
  \  method: get\n  operationId: getCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/tags\n  method: get\n  operationId: listTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/tags/{id}\n  method: get\n  operationId: getTag\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kateeva/refs/heads/main/agentic-access/kateeva-agentic-access.yml
summary_line: 21 operations
tags:
- Company
- Display Manufacturing
- OLED
- Semiconductor Equipment
- Capital Equipment
- Inkjet Printing
- Thin Film Encapsulation
- Advanced Manufacturing
- Materials Deposition
- Consumer Electronics
- Hardware
- Content
---
