---
acting_count: 0
action_class_counts:
  connected: 23
api_specs:
- filename: metalenz-press-releases-api-openapi.yml
  format: yaml
  label: Metalenz Press Releases API
  slug: metalenz-press-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metalenz/refs/heads/main/openapi/metalenz-press-releases-api-openapi.yml
- filename: metalenz-pages-api-openapi.yml
  format: yaml
  label: Metalenz Pages API
  slug: metalenz-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metalenz/refs/heads/main/openapi/metalenz-pages-api-openapi.yml
- filename: metalenz-media-api-openapi.yml
  format: yaml
  label: Metalenz Media API
  slug: metalenz-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metalenz/refs/heads/main/openapi/metalenz-media-api-openapi.yml
- filename: metalenz-taxonomy-api-openapi.yml
  format: yaml
  label: Metalenz Taxonomy API
  slug: metalenz-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metalenz/refs/heads/main/openapi/metalenz-taxonomy-api-openapi.yml
- filename: metalenz-search-api-openapi.yml
  format: yaml
  label: Metalenz Search API
  slug: metalenz-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metalenz/refs/heads/main/openapi/metalenz-search-api-openapi.yml
- filename: metalenz-discovery-api-openapi.yml
  format: yaml
  label: Metalenz Discovery API
  slug: metalenz-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metalenz/refs/heads/main/openapi/metalenz-discovery-api-openapi.yml
- filename: metalenz-oembed-api-openapi.yml
  format: yaml
  label: Metalenz oEmbed API
  slug: metalenz-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metalenz/refs/heads/main/openapi/metalenz-oembed-api-openapi.yml
consequence_counts:
  read: 23
description: Recommended x-agentic-access execution contracts, classified from the OpenAPI. Every operation on this surface is an anonymous read, so every contract is action-class connected / consequence read with no human-in-the-loop requirement and no audit obligation. A governance starting point for exposing this API to AI agents — review and bind audience per deployment.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Metalenz Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 23
overview: 'Metalenz exposes 23 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 23 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Metalenz
provider_slug: metalenz
slug: metalenz-agentic-access
source_filename: metalenz-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: generated\nsource: openapi/metalenz-discovery-api-openapi.yml, openapi/metalenz-media-api-openapi.yml, openapi/metalenz-oembed-api-openapi.yml,\n  openapi/metalenz-pages-api-openapi.yml, openapi/metalenz-press-releases-api-openapi.yml, openapi/metalenz-search-api-openapi.yml,\n  openapi/metalenz-taxonomy-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified from the OpenAPI. Every operation on this\n  surface is an anonymous read, so every contract is action-class connected / consequence read with no human-in-the-loop\n  requirement and no audit obligation. A governance starting point for exposing this API to AI agents — review and\n  bind audience per deployment.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 23\n  by_consequence:\n    read: 23\n  human_in_the_loop_required: 0\n  note: There is no write, no purchase, no notification and no destructive operation to classify. The write methods\n\
  \    that exist on the same WordPress routes are credential-gated with no public issuance path and are therefore\n    out of scope for an agent. listAuthors/getAuthor return personal data and are flagged below even though they\n    are reads.\noperations:\n- path: /wp/v2/posts\n  method: get\n  operationId: listPressReleases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/posts/{id}\n  method: get\n  operationId: getPressRelease\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/pages\n  method: get\n  operationId: listPages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/pages/{id}\n  method: get\n  operationId: getPage\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/media\n  method: get\n  operationId: listMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/media/{id}\n  method: get\n  operationId: getMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/categories\n  method: get\n  operationId: listCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/categories/{id}\n  method: get\n  operationId: getCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/tags\n  method:\
  \ get\n  operationId: listTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/tags/{id}\n  method: get\n  operationId: getTag\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/search\n  method: get\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: getRouteIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{namespace}\n  method: get\n  operationId: getNamespaceIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /wp/v2/types\n  method: get\n  operationId: listTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/types/{type}\n  method: get\n  operationId: getType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/taxonomies\n  method: get\n  operationId: listTaxonomies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/taxonomies/{taxonomy}\n  method: get\n  operationId: getTaxonomy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/statuses\n  method: get\n  operationId: listStatuses\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/statuses/{status}\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wp/v2/users\n  method: get\n  operationId: listAuthors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: recommended\n  x-personal-data: true\n  x-note: Returns real WordPress accounts. Reading it is permitted and anonymous, but an agent should not store,\n    republish or enrich the individuals it returns. Excluded from skills/ and mcp/.\n- path: /wp/v2/users/{id}\n  method: get\n  operationId: getAuthor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: recommended\n  x-personal-data:\
  \ true\n  x-note: Returns real WordPress accounts. Reading it is permitted and anonymous, but an agent should not store,\n    republish or enrich the individuals it returns. Excluded from skills/ and mcp/.\n- path: /wp/v2/comments\n  method: get\n  operationId: listComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oembed/1.0/embed\n  method: get\n  operationId: getOembed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metalenz/refs/heads/main/agentic-access/metalenz-agentic-access.yml
summary_line: 23 operations
tags:
- Company
- Semiconductors
- Optics
- Meta-Optics
- Metasurface
- Photonics
- Biometrics
- Face Authentication
- Polarization Imaging
- 3D Sensing
- Computer-Vision
- Consumer Electronics
- Automotive
- Robotics
- Hardware
- Content
---
