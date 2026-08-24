---
acting_count: 0
action_class_counts:
  connected: 22
api_specs:
- filename: harbinger-posts-api-openapi.yml
  format: yaml
  label: Harbinger Motors Posts API
  slug: harbinger-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harbinger/refs/heads/main/openapi/harbinger-posts-api-openapi.yml
- filename: harbinger-pages-api-openapi.yml
  format: yaml
  label: Harbinger Motors Pages API
  slug: harbinger-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harbinger/refs/heads/main/openapi/harbinger-pages-api-openapi.yml
- filename: harbinger-events-api-openapi.yml
  format: yaml
  label: Harbinger Motors Events API
  slug: harbinger-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harbinger/refs/heads/main/openapi/harbinger-events-api-openapi.yml
- filename: harbinger-media-api-openapi.yml
  format: yaml
  label: Harbinger Motors Media API
  slug: harbinger-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harbinger/refs/heads/main/openapi/harbinger-media-api-openapi.yml
- filename: harbinger-taxonomy-api-openapi.yml
  format: yaml
  label: Harbinger Motors Taxonomy API
  slug: harbinger-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harbinger/refs/heads/main/openapi/harbinger-taxonomy-api-openapi.yml
- filename: harbinger-search-api-openapi.yml
  format: yaml
  label: Harbinger Motors Search API
  slug: harbinger-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harbinger/refs/heads/main/openapi/harbinger-search-api-openapi.yml
- filename: harbinger-discovery-api-openapi.yml
  format: yaml
  label: Harbinger Motors Discovery API
  slug: harbinger-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harbinger/refs/heads/main/openapi/harbinger-discovery-api-openapi.yml
- filename: harbinger-oembed-api-openapi.yml
  format: yaml
  label: Harbinger Motors oEmbed API
  slug: harbinger-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harbinger/refs/heads/main/openapi/harbinger-oembed-api-openapi.yml
- filename: harbinger-seo-api-openapi.yml
  format: yaml
  label: Harbinger Motors SEO Metadata API
  slug: harbinger-seo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harbinger/refs/heads/main/openapi/harbinger-seo-api-openapi.yml
consequence_counts:
  read: 22
description: Recommended x-agentic-access execution contracts, classified from the derived OpenAPI. Every publicly reachable operation on this surface is an anonymous read with no side effect and nothing to reverse, so the classification is uniform — that uniformity is the finding, not a shortcut. A governance starting point for exposing this API to AI agents; review and bind audience per deployment.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Harbinger Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'Harbinger exposes 22 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Harbinger
provider_slug: harbinger
slug: harbinger-agentic-access
source_filename: harbinger-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: generated\nsource: openapi/harbinger-discovery-api-openapi.yml, openapi/harbinger-events-api-openapi.yml, openapi/harbinger-media-api-openapi.yml,\n  openapi/harbinger-oembed-api-openapi.yml, openapi/harbinger-pages-api-openapi.yml, openapi/harbinger-posts-api-openapi.yml,\n  openapi/harbinger-search-api-openapi.yml, openapi/harbinger-seo-api-openapi.yml, openapi/harbinger-taxonomy-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified from the derived OpenAPI. Every publicly\n  reachable operation on this surface is an anonymous read with no side effect and nothing to reverse, so the\n  classification is uniform — that uniformity is the finding, not a shortcut. A governance starting point for\n  exposing this API to AI agents; review and bind audience per deployment.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 22\n  by_consequence:\n    read: 22\n  human_in_the_loop_required: 0\n  write_operations:\
  \ 0\n  note: No public write operation exists. Anonymous POST/PUT/PATCH/DELETE returns 401 rest_cannot_create.\noperations:\n- path: /\n  method: get\n  operationId: getApiIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    reversible: na\n- path: /wp/v2\n  method: get\n  operationId: getNamespaceIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    reversible: na\n- path: /wp/v2/types\n  method: get\n  operationId: listTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    reversible: na\n- path: /wp/v2/types/{type}\n  method: get\n  operationId: getType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n    reversible: na\n- path: /wp/v2/statuses\n  method: get\n  operationId: listStatuses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    reversible: na\n- path: /wp/v2/event\n  method: get\n  operationId: listEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    reversible: na\n- path: /wp/v2/event/{id}\n  method: get\n  operationId: getEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    reversible: na\n- path: /wp/v2/media\n  method: get\n  operationId: listMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    reversible: na\n- path: /wp/v2/media/{id}\n  method:\
  \ get\n  operationId: getMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    reversible: na\n- path: /oembed/1.0/embed\n  method: get\n  operationId: getOembed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    reversible: na\n- path: /wp/v2/pages\n  method: get\n  operationId: listPages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    reversible: na\n- path: /wp/v2/pages/{id}\n  method: get\n  operationId: getPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    reversible: na\n- path: /wp/v2/posts\n  method: get\n  operationId: listPosts\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    reversible: na\n- path: /wp/v2/posts/{id}\n  method: get\n  operationId: getPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    reversible: na\n- path: /wp/v2/search\n  method: get\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    reversible: na\n- path: /yoast/v1/get_head\n  method: get\n  operationId: getSeoHead\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    reversible: na\n- path: /wp/v2/categories\n  method: get\n  operationId: listCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n    reversible: na\n- path: /wp/v2/categories/{id}\n  method: get\n  operationId: getCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    reversible: na\n- path: /wp/v2/tags\n  method: get\n  operationId: listTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    reversible: na\n- path: /wp/v2/tags/{id}\n  method: get\n  operationId: getTag\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    reversible: na\n- path: /wp/v2/taxonomies\n  method: get\n  operationId: listTaxonomies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    reversible: na\n- path: /wp/v2/taxonomies/{taxonomy}\n\
  \  method: get\n  operationId: getTaxonomy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    reversible: na\nguardrails:\n  rate: No published limit and no runtime signal. Self-throttle to 1-2 concurrent requests. See rate-limits/harbinger-rate-limits.yml.\n  freshness: No Cache-Control, ETag or Last-Modified is returned, so an agent cannot revalidate cheaply and cannot\n    tell a stale read from a fresh one.\n  pii: Author ids appear on records but /wp/v2/users is 401-gated, so no personal data is resolvable anonymously.\n  tracking: Responses set a _fbp Meta advertising cookie. A machine client must discard cookies.\n  indexing: 'Every response carries X-Robots-Tag: noindex. Treat the data as readable-but-not-republishable-as-content.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harbinger/refs/heads/main/agentic-access/harbinger-agentic-access.yml
summary_line: 22 operations
tags:
- Company
- Automotive
- Electric Vehicles
- Commercial Vehicles
- Medium Duty Trucks
- Manufacturing
- Fleet Management
- Transportation
- Logistics
- Energy Storage
- Content
---
