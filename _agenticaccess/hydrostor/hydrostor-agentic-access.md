---
acting_count: 0
action_class_counts:
  connected: 26
api_specs:
- filename: hydrostor-projects-api-openapi.yml
  format: yaml
  label: Hydrostor Projects API
  slug: hydrostor-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hydrostor/refs/heads/main/openapi/hydrostor-projects-api-openapi.yml
- filename: hydrostor-posts-api-openapi.yml
  format: yaml
  label: Hydrostor Posts API
  slug: hydrostor-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hydrostor/refs/heads/main/openapi/hydrostor-posts-api-openapi.yml
- filename: hydrostor-pages-api-openapi.yml
  format: yaml
  label: Hydrostor Pages API
  slug: hydrostor-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hydrostor/refs/heads/main/openapi/hydrostor-pages-api-openapi.yml
- filename: hydrostor-media-api-openapi.yml
  format: yaml
  label: Hydrostor Media API
  slug: hydrostor-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hydrostor/refs/heads/main/openapi/hydrostor-media-api-openapi.yml
- filename: hydrostor-taxonomy-api-openapi.yml
  format: yaml
  label: Hydrostor Taxonomy API
  slug: hydrostor-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hydrostor/refs/heads/main/openapi/hydrostor-taxonomy-api-openapi.yml
- filename: hydrostor-search-api-openapi.yml
  format: yaml
  label: Hydrostor Search API
  slug: hydrostor-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hydrostor/refs/heads/main/openapi/hydrostor-search-api-openapi.yml
- filename: hydrostor-discovery-api-openapi.yml
  format: yaml
  label: Hydrostor Discovery API
  slug: hydrostor-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hydrostor/refs/heads/main/openapi/hydrostor-discovery-api-openapi.yml
- filename: hydrostor-oembed-api-openapi.yml
  format: yaml
  label: Hydrostor oEmbed API
  slug: hydrostor-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hydrostor/refs/heads/main/openapi/hydrostor-oembed-api-openapi.yml
- filename: hydrostor-seo-api-openapi.yml
  format: yaml
  label: Hydrostor SEO Metadata API
  slug: hydrostor-seo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hydrostor/refs/heads/main/openapi/hydrostor-seo-api-openapi.yml
consequence_counts:
  read: 26
description: Recommended x-agentic-access execution contracts, classified from the derived OpenAPI. Every publicly reachable operation on this surface is an anonymous read, so every classification below is `connected` / `read` with no human-in-the-loop requirement — there is nothing an agent can do here that changes state. The write methods declared on the same routes are excluded because they require a WordPress application password with no public issuance path and are therefore not part of the public contract.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Hydrostor Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 26
overview: 'Hydrostor exposes 26 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 26 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Hydrostor
provider_slug: hydrostor
slug: hydrostor-agentic-access
source_filename: hydrostor-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: generated\nsource: openapi/hydrostor-discovery-api-openapi.yml, openapi/hydrostor-media-api-openapi.yml, openapi/hydrostor-oembed-api-openapi.yml,\n  openapi/hydrostor-pages-api-openapi.yml, openapi/hydrostor-posts-api-openapi.yml, openapi/hydrostor-projects-api-openapi.yml,\n  openapi/hydrostor-search-api-openapi.yml, openapi/hydrostor-seo-api-openapi.yml, openapi/hydrostor-taxonomy-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified from the derived OpenAPI. Every publicly\n  reachable operation on this surface is an anonymous read, so every classification below is `connected` / `read`\n  with no human-in-the-loop requirement — there is nothing an agent can do here that changes state. The write\n  methods declared on the same routes are excluded because they require a WordPress application password with\n  no public issuance path and are therefore not part of the public contract.\nsummary:\n  operations:\
  \ 26\n  by_action_class:\n    connected: 26\n  by_consequence:\n    read: 26\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: getApiIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/types\n  method: get\n  operationId: listContentTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/types/{type}\n  method: get\n  operationId: getContentType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/taxonomies\n  method: get\n  operationId: listTaxonomyDefinitions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/statuses\n\
  \  method: get\n  operationId: listPostStatuses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/users\n  method: get\n  operationId: listAuthors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/users/{id}\n  method: get\n  operationId: getAuthor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/media\n  method: get\n  operationId: listMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/media/{id}\n  method: get\n  operationId: getMediaItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /oembed/1.0/embed\n  method: get\n  operationId: getOembed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/pages\n  method: get\n  operationId: listPages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/pages/{id}\n  method: get\n  operationId: getPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/posts\n  method: get\n  operationId: listPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/posts/{id}\n  method: get\n  operationId: getPost\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/project\n  method: get\n  operationId: listProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/project/{id}\n  method: get\n  operationId: getProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/search\n  method: get\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /yoast/v1/get_head\n  method: get\n  operationId: getSeoHead\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/categories\n  method: get\n  operationId:\
  \ listCategoryTerms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/categories/{id}\n  method: get\n  operationId: getCategoryTerm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/tags\n  method: get\n  operationId: listTagTerms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/tags/{id}\n  method: get\n  operationId: getTagTerm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/project_category\n  method: get\n  operationId: listProjectCategoryTerms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/project_category/{id}\n  method: get\n  operationId: getProjectCategoryTerm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/project_tag\n  method: get\n  operationId: listProjectTagTerms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/project_tag/{id}\n  method: get\n  operationId: getProjectTagTerm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hydrostor/refs/heads/main/agentic-access/hydrostor-agentic-access.yml
summary_line: 26 operations
tags:
- Company
- Energy
- Energy Storage
- Long Duration Energy Storage
- Compressed Air Energy Storage
- Grid Infrastructure
- Renewable Energy
- Clean Energy
- Utilities
- Climate Tech
- Canada
- Content
---
