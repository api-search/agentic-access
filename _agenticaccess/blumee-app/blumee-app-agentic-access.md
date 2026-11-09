---
acting_count: 0
action_class_counts:
  connected: 7
api_specs:
- filename: blumee-app-catalog-api-openapi.yml
  format: yaml
  label: Blumee Catalog API
  slug: blumee-app-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blumee-app/openapi/blumee-app-catalog-api-openapi.yml
- filename: blumee-app-search-api-openapi.yml
  format: yaml
  label: Blumee Search API
  slug: blumee-app-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blumee-app/openapi/blumee-app-search-api-openapi.yml
- filename: blumee-app-service-api-openapi.yml
  format: yaml
  label: Blumee Service API
  slug: blumee-app-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blumee-app/openapi/blumee-app-service-api-openapi.yml
consequence_counts:
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Blumee App Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Blumee exposes 7 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Blumee
provider_slug: blumee-app
slug: blumee-app-agentic-access
source_filename: blumee-app-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/blumee-app-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 7\n  by_consequence:\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/catalog\n  method: get\n  operationId: listCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/catalog/facets\n  method: get\n  operationId: getCatalogFacets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/catalog/stats\n  method: get\n  operationId: getCatalogStats\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/products/{id}\n  method: get\n  operationId: getProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/search/text\n  method: post\n  operationId: searchText\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/search/photo\n  method: post\n  operationId: searchPhoto\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/blumee-app/agentic-access/blumee-app-agentic-access.yml
summary_line: 7 operations
tags:
- Flower Delivery
- E-Commerce
- Germany
- Mobile App
- Online Shopping
---
