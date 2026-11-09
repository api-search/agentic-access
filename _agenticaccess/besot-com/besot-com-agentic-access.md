---
acting_count: 0
action_class_counts:
  connected: 8
api_specs:
- filename: besot-com-artists-api-openapi.yml
  format: yaml
  label: besot Artists API
  slug: besot-com-artists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/besot-com/openapi/besot-com-artists-api-openapi.yml
- filename: besot-com-categories-api-openapi.yml
  format: yaml
  label: besot Categories API
  slug: besot-com-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/besot-com/openapi/besot-com-categories-api-openapi.yml
- filename: besot-com-collections-api-openapi.yml
  format: yaml
  label: besot Collections API
  slug: besot-com-collections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/besot-com/openapi/besot-com-collections-api-openapi.yml
- filename: besot-com-designers-api-openapi.yml
  format: yaml
  label: besot Designers API
  slug: besot-com-designers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/besot-com/openapi/besot-com-designers-api-openapi.yml
- filename: besot-com-facets-api-openapi.yml
  format: yaml
  label: besot Facets API
  slug: besot-com-facets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/besot-com/openapi/besot-com-facets-api-openapi.yml
- filename: besot-com-networks-api-openapi.yml
  format: yaml
  label: besot Networks API
  slug: besot-com-networks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/besot-com/openapi/besot-com-networks-api-openapi.yml
- filename: besot-com-pieces-api-openapi.yml
  format: yaml
  label: besot Pieces API
  slug: besot-com-pieces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/besot-com/openapi/besot-com-pieces-api-openapi.yml
- filename: besot-com-programs-api-openapi.yml
  format: yaml
  label: besot Programs API
  slug: besot-com-programs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/besot-com/openapi/besot-com-programs-api-openapi.yml
- filename: besot-com-search-api-openapi.yml
  format: yaml
  label: besot Search API
  slug: besot-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/besot-com/openapi/besot-com-search-api-openapi.yml
- filename: besot-com-stats-api-openapi.yml
  format: yaml
  label: besot Stats API
  slug: besot-com-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/besot-com/openapi/besot-com-stats-api-openapi.yml
consequence_counts:
  read: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Besot Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'besot exposes 8 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: besot
provider_slug: besot-com
slug: besot-com-agentic-access
source_filename: besot-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/besot-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 8\n  by_consequence:\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /facets\n  method: get\n  operationId: getFacets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pieces\n  method: get\n  operationId: searchPieces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pieces/{collectionId}/{pieceId}\n  method: get\n  operationId: getPiece\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections\n  method: get\n  operationId: listCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{id}\n  method: get\n  operationId: getCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artists\n  method: get\n  operationId: listArtists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /designers\n  method: get\n  operationId: listDesigners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search\n  method:\
  \ get\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/besot-com/agentic-access/besot-com-agentic-access.yml
summary_line: 8 operations
tags:
- Company
- Fashion
- Resale
- Catalog
- Fandom
- Clothing
---
