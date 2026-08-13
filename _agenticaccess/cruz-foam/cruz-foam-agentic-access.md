---
acting_count: 0
action_class_counts:
  connected: 23
api_specs:
- filename: cruz-foam-posts-api-openapi.yml
  format: yaml
  label: Cruz Foam Posts API
  slug: cruz-foam-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cruz-foam/refs/heads/main/openapi/cruz-foam-posts-api-openapi.yml
- filename: cruz-foam-pages-api-openapi.yml
  format: yaml
  label: Cruz Foam Pages API
  slug: cruz-foam-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cruz-foam/refs/heads/main/openapi/cruz-foam-pages-api-openapi.yml
- filename: cruz-foam-customers-api-openapi.yml
  format: yaml
  label: Cruz Foam Customers API
  slug: cruz-foam-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cruz-foam/refs/heads/main/openapi/cruz-foam-customers-api-openapi.yml
- filename: cruz-foam-media-api-openapi.yml
  format: yaml
  label: Cruz Foam Media API
  slug: cruz-foam-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cruz-foam/refs/heads/main/openapi/cruz-foam-media-api-openapi.yml
- filename: cruz-foam-taxonomy-api-openapi.yml
  format: yaml
  label: Cruz Foam Taxonomy API
  slug: cruz-foam-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cruz-foam/refs/heads/main/openapi/cruz-foam-taxonomy-api-openapi.yml
- filename: cruz-foam-search-api-openapi.yml
  format: yaml
  label: Cruz Foam Search API
  slug: cruz-foam-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cruz-foam/refs/heads/main/openapi/cruz-foam-search-api-openapi.yml
- filename: cruz-foam-discovery-api-openapi.yml
  format: yaml
  label: Cruz Foam Discovery API
  slug: cruz-foam-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cruz-foam/refs/heads/main/openapi/cruz-foam-discovery-api-openapi.yml
- filename: cruz-foam-oembed-api-openapi.yml
  format: yaml
  label: Cruz Foam oEmbed API
  slug: cruz-foam-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cruz-foam/refs/heads/main/openapi/cruz-foam-oembed-api-openapi.yml
- filename: cruz-foam-seo-api-openapi.yml
  format: yaml
  label: Cruz Foam SEO Metadata API
  slug: cruz-foam-seo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cruz-foam/refs/heads/main/openapi/cruz-foam-seo-api-openapi.yml
consequence_counts:
  read: 23
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cruz Foam Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 23
overview: 'Cruz Foam exposes 23 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 23 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cruz Foam
provider_slug: cruz-foam
slug: cruz-foam-agentic-access
source_filename: cruz-foam-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: generated\nsource: openapi/cruz-foam-customers-api-openapi.yml, openapi/cruz-foam-discovery-api-openapi.yml,\n  openapi/cruz-foam-media-api-openapi.yml, openapi/cruz-foam-oembed-api-openapi.yml, openapi/cruz-foam-pages-api-openapi.yml,\n  openapi/cruz-foam-posts-api-openapi.yml, openapi/cruz-foam-search-api-openapi.yml, openapi/cruz-foam-seo-api-openapi.yml,\n  openapi/cruz-foam-taxonomy-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 23\n  by_consequence:\n    read: 23\n  human_in_the_loop_required: 0\noperations:\n- path: /wp/v2/customers\n  method: get\n  operationId: listCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/customers/{id}\n  method: get\n  operationId: getCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/users/{id}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: getRouteIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/statuses\n  method: get\n  operationId: listStatuses\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/types\n  method: get\n  operationId: listTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/taxonomies\n  method: get\n  operationId: listTaxonomies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/media\n  method: get\n  operationId: listMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/media/{id}\n  method: get\n  operationId: getMediaItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oembed/1.0/embed\n\
  \  method: get\n  operationId: getOembed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/pages\n  method: get\n  operationId: listPages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/pages/{id}\n  method: get\n  operationId: getPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/posts\n  method: get\n  operationId: listPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/posts/{id}\n  method: get\n  operationId: getPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /wp/v2/search\n  method: get\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /yoast/v1/get_head\n  method: get\n  operationId: getSeoHead\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/categories\n  method: get\n  operationId: listCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/categories/{id}\n  method: get\n  operationId: getCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/tags\n  method: get\n  operationId: listTags\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/tags/{id}\n  method: get\n  operationId: getTag\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/portfolio-categories\n  method: get\n  operationId: listPortfolioCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/portfolio-categories/{id}\n  method: get\n  operationId: getPortfolioCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cruz-foam/refs/heads/main/agentic-access/cruz-foam-agentic-access.yml
summary_line: 23 operations
tags:
- Company
- Materials Science
- Sustainable Packaging
- Compostable Materials
- Biomaterials
- Circular Economy
- Manufacturing
- Consumer Packaged Goods
- Cold Chain
- Sustainability
- Content
---
