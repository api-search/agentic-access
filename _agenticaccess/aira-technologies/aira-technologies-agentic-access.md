---
acting_count: 0
action_class_counts:
  connected: 24
api_specs:
- filename: aira-technologies-posts-api-openapi.yml
  format: yaml
  label: Aira Technologies Posts API
  slug: aira-technologies-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aira-technologies/refs/heads/main/openapi/aira-technologies-posts-api-openapi.yml
- filename: aira-technologies-pages-api-openapi.yml
  format: yaml
  label: Aira Technologies Pages API
  slug: aira-technologies-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aira-technologies/refs/heads/main/openapi/aira-technologies-pages-api-openapi.yml
- filename: aira-technologies-articles-api-openapi.yml
  format: yaml
  label: Aira Technologies Articles API
  slug: aira-technologies-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aira-technologies/refs/heads/main/openapi/aira-technologies-articles-api-openapi.yml
- filename: aira-technologies-events-api-openapi.yml
  format: yaml
  label: Aira Technologies Events API
  slug: aira-technologies-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aira-technologies/refs/heads/main/openapi/aira-technologies-events-api-openapi.yml
- filename: aira-technologies-media-api-openapi.yml
  format: yaml
  label: Aira Technologies Media API
  slug: aira-technologies-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aira-technologies/refs/heads/main/openapi/aira-technologies-media-api-openapi.yml
- filename: aira-technologies-search-api-openapi.yml
  format: yaml
  label: Aira Technologies Search API
  slug: aira-technologies-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aira-technologies/refs/heads/main/openapi/aira-technologies-search-api-openapi.yml
- filename: aira-technologies-discovery-api-openapi.yml
  format: yaml
  label: Aira Technologies Discovery API
  slug: aira-technologies-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aira-technologies/refs/heads/main/openapi/aira-technologies-discovery-api-openapi.yml
- filename: aira-technologies-categories-api-openapi.yml
  format: yaml
  label: Aira Technologies Categories API
  slug: aira-technologies-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aira-technologies/refs/heads/main/openapi/aira-technologies-categories-api-openapi.yml
- filename: aira-technologies-users-api-openapi.yml
  format: yaml
  label: Aira Technologies Users API
  slug: aira-technologies-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aira-technologies/refs/heads/main/openapi/aira-technologies-users-api-openapi.yml
- filename: aira-technologies-o-embed-api-openapi.yml
  format: yaml
  label: Aira Technologies o Embed API
  slug: aira-technologies-o-embed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aira-technologies/refs/heads/main/openapi/aira-technologies-o-embed-api-openapi.yml
consequence_counts:
  read: 24
description: Recommended x-agentic-access execution contracts, classified from the OpenAPI documents in this repo. Every anonymously reachable operation on this surface is a read against a public marketing content API, so every contract classifies the same way — action-class connected, consequence read, no human in the loop, no audit requirement. There is no write, no money movement, no personal data and no irreversible action to govern here. A governance starting point for exposing this API to AI agents; review and bind audience per deployment.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Aira Technologies Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 24
overview: 'Aira Technologies exposes 24 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 24 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Aira Technologies
provider_slug: aira-technologies
slug: aira-technologies-agentic-access
source_filename: aira-technologies-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: generated\nsource: openapi/aira-technologies-articles-api-openapi.yml, openapi/aira-technologies-categories-api-openapi.yml,\n  openapi/aira-technologies-discovery-api-openapi.yml, openapi/aira-technologies-events-api-openapi.yml, openapi/aira-technologies-media-api-openapi.yml,\n  openapi/aira-technologies-oembed-api-openapi.yml, openapi/aira-technologies-pages-api-openapi.yml, openapi/aira-technologies-posts-api-openapi.yml,\n  openapi/aira-technologies-search-api-openapi.yml, openapi/aira-technologies-users-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified from the OpenAPI documents in this\n  repo. Every anonymously reachable operation on this surface is a read against a public marketing content\n  API, so every contract classifies the same way — action-class connected, consequence read, no human in the\n  loop, no audit requirement. There is no write, no money movement, no personal data and no irreversible\
  \ action\n  to govern here. A governance starting point for exposing this API to AI agents; review and bind audience\n  per deployment.\nsummary:\n  operations: 24\n  by_action_class:\n    connected: 24\n  by_consequence:\n    read: 24\n  human_in_the_loop_required: 0\n  note: 'Uniformity here is a property of the surface, not a shortcut. The anonymous surface answers `Allow:\n    GET`; an unauthenticated POST returns 401 rest_cannot_create. The only gated routes on the host — /wp/v2/settings\n    and the whole /wp-abilities/v1 namespace — return 401 and are therefore not classified.'\noperations:\n- path: /wp/v2/article\n  method: get\n  operationId: listArticles\n  spec: openapi/aira-technologies-articles-api-openapi.yml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/article/{id}\n  method: get\n  operationId: getArticle\n  spec: openapi/aira-technologies-articles-api-openapi.yml\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/categories\n  method: get\n  operationId: listCategories\n  spec: openapi/aira-technologies-categories-api-openapi.yml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/categories/{id}\n  method: get\n  operationId: getCategory\n  spec: openapi/aira-technologies-categories-api-openapi.yml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: getApiRoot\n  spec: openapi/aira-technologies-discovery-api-openapi.yml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2\n  method: get\n\
  \  operationId: getNamespaceIndex\n  spec: openapi/aira-technologies-discovery-api-openapi.yml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/types\n  method: get\n  operationId: listTypes\n  spec: openapi/aira-technologies-discovery-api-openapi.yml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/types/{type}\n  method: get\n  operationId: getType\n  spec: openapi/aira-technologies-discovery-api-openapi.yml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/taxonomies\n  method: get\n  operationId: listTaxonomies\n  spec: openapi/aira-technologies-discovery-api-openapi.yml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/taxonomies/{taxonomy}\n  method: get\n  operationId: getTaxonomy\n  spec: openapi/aira-technologies-discovery-api-openapi.yml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/statuses\n  method: get\n  operationId: listStatuses\n  spec: openapi/aira-technologies-discovery-api-openapi.yml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/statuses/{status}\n  method: get\n  operationId: getStatus\n  spec: openapi/aira-technologies-discovery-api-openapi.yml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/events\n  method: get\n  operationId: listEvents\n  spec: openapi/aira-technologies-events-api-openapi.yml\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/events/{id}\n  method: get\n  operationId: getEvent\n  spec: openapi/aira-technologies-events-api-openapi.yml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/media\n  method: get\n  operationId: listMedia\n  spec: openapi/aira-technologies-media-api-openapi.yml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/media/{id}\n  method: get\n  operationId: getAttachment\n  spec: openapi/aira-technologies-media-api-openapi.yml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oembed/1.0/embed\n  method: get\n\
  \  operationId: getOembed\n  spec: openapi/aira-technologies-oembed-api-openapi.yml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/pages\n  method: get\n  operationId: listPages\n  spec: openapi/aira-technologies-pages-api-openapi.yml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/pages/{id}\n  method: get\n  operationId: getPage\n  spec: openapi/aira-technologies-pages-api-openapi.yml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/posts\n  method: get\n  operationId: listPosts\n  spec: openapi/aira-technologies-posts-api-openapi.yml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n- path: /wp/v2/posts/{id}\n  method: get\n  operationId: getPost\n  spec: openapi/aira-technologies-posts-api-openapi.yml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/search\n  method: get\n  operationId: searchContent\n  spec: openapi/aira-technologies-search-api-openapi.yml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/users\n  method: get\n  operationId: listUsers\n  spec: openapi/aira-technologies-users-api-openapi.yml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/users/{id}\n  method: get\n  operationId: getUser\n  spec: openapi/aira-technologies-users-api-openapi.yml\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aira-technologies/refs/heads/main/agentic-access/aira-technologies-agentic-access.yml
summary_line: 24 operations
tags:
- Company
- Telecommunications
- Wireless
- Artificial Intelligence
- Machine-Learning
- 5G
- Radio Access Network
- Network Automation
- Generative AI
- Observability
- Content
---
