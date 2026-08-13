---
acting_count: 0
action_class_counts:
  connected: 19
api_specs:
- filename: fabric8labs-posts-api-openapi.yml
  format: yaml
  label: Fabric8Labs Posts API
  slug: fabric8labs-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric8labs/refs/heads/main/openapi/fabric8labs-posts-api-openapi.yml
- filename: fabric8labs-pages-api-openapi.yml
  format: yaml
  label: Fabric8Labs Pages API
  slug: fabric8labs-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric8labs/refs/heads/main/openapi/fabric8labs-pages-api-openapi.yml
- filename: fabric8labs-media-api-openapi.yml
  format: yaml
  label: Fabric8Labs Media API
  slug: fabric8labs-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric8labs/refs/heads/main/openapi/fabric8labs-media-api-openapi.yml
- filename: fabric8labs-team-api-openapi.yml
  format: yaml
  label: Fabric8Labs Team API
  slug: fabric8labs-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric8labs/refs/heads/main/openapi/fabric8labs-team-api-openapi.yml
- filename: fabric8labs-taxonomy-api-openapi.yml
  format: yaml
  label: Fabric8Labs Taxonomy API
  slug: fabric8labs-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric8labs/refs/heads/main/openapi/fabric8labs-taxonomy-api-openapi.yml
- filename: fabric8labs-search-api-openapi.yml
  format: yaml
  label: Fabric8Labs Search API
  slug: fabric8labs-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric8labs/refs/heads/main/openapi/fabric8labs-search-api-openapi.yml
- filename: fabric8labs-discovery-api-openapi.yml
  format: yaml
  label: Fabric8Labs Discovery API
  slug: fabric8labs-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric8labs/refs/heads/main/openapi/fabric8labs-discovery-api-openapi.yml
consequence_counts:
  read: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Fabric8Labs Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 19
overview: 'Fabric8Labs exposes 19 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Fabric8Labs
provider_slug: fabric8labs
slug: fabric8labs-agentic-access
source_filename: fabric8labs-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: generated\nsource: openapi/fabric8labs-discovery-api-openapi.yml, openapi/fabric8labs-media-api-openapi.yml,\n  openapi/fabric8labs-pages-api-openapi.yml, openapi/fabric8labs-posts-api-openapi.yml, openapi/fabric8labs-search-api-openapi.yml,\n  openapi/fabric8labs-taxonomy-api-openapi.yml, openapi/fabric8labs-team-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 19\n  by_consequence:\n    read: 19\n  human_in_the_loop_required: 0\noperations:\n- path: /wp/v2/types\n  method: get\n  operationId: listTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /wp/v2/types/{type}\n  method: get\n  operationId: getTypesById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/taxonomies\n  method: get\n  operationId: listTaxonomies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/taxonomies/{taxonomy}\n  method: get\n  operationId: getTaxonomiesById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/statuses\n  method: get\n  operationId: listStatuses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/statuses/{status}\n  method: get\n  operationId: getStatusesById\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/media\n  method: get\n  operationId: listMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/media/{id}\n  method: get\n  operationId: getMediaById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/pages\n  method: get\n  operationId: listPages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/pages/{id}\n  method: get\n  operationId: getPagesById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/posts\n  method: get\n \
  \ operationId: listPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/posts/{id}\n  method: get\n  operationId: getPostsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/search\n  method: get\n  operationId: listSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/categories\n  method: get\n  operationId: listCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/categories/{id}\n  method: get\n  operationId: getCategoriesById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/tags\n  method: get\n  operationId: listTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/tags/{id}\n  method: get\n  operationId: getTagsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/team\n  method: get\n  operationId: listTeam\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/team/{id}\n  method: get\n  operationId: getTeamById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fabric8labs/refs/heads/main/agentic-access/fabric8labs-agentic-access.yml
summary_line: 19 operations
tags:
- Company
- Advanced Manufacturing
- Additive Manufacturing
- 3D Printing
- Metal 3D Printing
- Electrochemical Additive Manufacturing
- Thermal Management
- Liquid Cooling
- Data Centers
- Semiconductors
- Electronics
- Aerospace
- Photonics
- Power Electronics
- Hardware
- Content
---
