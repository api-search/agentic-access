---
acting_count: 0
action_class_counts:
  connected: 17
api_specs:
- filename: mindmaze-discovery-api-openapi.yml
  format: yaml
  label: MindMaze Discovery API
  slug: mindmaze-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindmaze/refs/heads/main/openapi/mindmaze-discovery-api-openapi.yml
- filename: mindmaze-media-api-openapi.yml
  format: yaml
  label: MindMaze Media API
  slug: mindmaze-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindmaze/refs/heads/main/openapi/mindmaze-media-api-openapi.yml
- filename: mindmaze-oembed-api-openapi.yml
  format: yaml
  label: MindMaze O Embed API
  slug: mindmaze-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindmaze/refs/heads/main/openapi/mindmaze-oembed-api-openapi.yml
- filename: mindmaze-pages-api-openapi.yml
  format: yaml
  label: MindMaze Pages API
  slug: mindmaze-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindmaze/refs/heads/main/openapi/mindmaze-pages-api-openapi.yml
- filename: mindmaze-posts-api-openapi.yml
  format: yaml
  label: MindMaze Posts API
  slug: mindmaze-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindmaze/refs/heads/main/openapi/mindmaze-posts-api-openapi.yml
- filename: mindmaze-search-api-openapi.yml
  format: yaml
  label: MindMaze Search API
  slug: mindmaze-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindmaze/refs/heads/main/openapi/mindmaze-search-api-openapi.yml
- filename: mindmaze-taxonomy-api-openapi.yml
  format: yaml
  label: MindMaze Taxonomy API
  slug: mindmaze-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mindmaze/refs/heads/main/openapi/mindmaze-taxonomy-api-openapi.yml
consequence_counts:
  read: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Mindmaze Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'MindMaze exposes 17 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: MindMaze
provider_slug: mindmaze
slug: mindmaze-agentic-access
source_filename: mindmaze-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: generated\nsource: openapi/mindmaze-content-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 17\n  by_consequence:\n    read: 17\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: getApiIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2\n  method: get\n  operationId: getNamespaceIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/posts\n  method: get\n  operationId: listPosts\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/posts/{id}\n  method: get\n  operationId: getPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/pages\n  method: get\n  operationId: listPages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/pages/{id}\n  method: get\n  operationId: getPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/media\n  method: get\n  operationId: listMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/media/{id}\n  method:\
  \ get\n  operationId: getMediaItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/categories\n  method: get\n  operationId: listCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/categories/{id}\n  method: get\n  operationId: getCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/tags\n  method: get\n  operationId: listTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/tags/{id}\n  method: get\n  operationId: getTag\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /wp/v2/taxonomies\n  method: get\n  operationId: listTaxonomies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/types\n  method: get\n  operationId: listContentTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/statuses\n  method: get\n  operationId: listStatuses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/search\n  method: get\n  operationId: searchContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oembed/1.0/embed\n  method: get\n  operationId: getOEmbed\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mindmaze/refs/heads/main/agentic-access/mindmaze-agentic-access.yml
summary_line: 17 operations
tags:
- Company
- Digital Therapeutics
- Neurotechnology
- Neurorehabilitation
- Medical Devices
- Health
- Artificial Intelligence
- Stroke
- Parkinsons Disease
- Switzerland
---
