---
acting_count: 0
action_class_counts:
  connected: 12
api_specs:
- filename: usda-agricultural-research-service-ars--datasets-api-openapi.yml
  format: yaml
  label: USDA Agricultural Research Service (ARS) Datasets API
  slug: usda-agricultural-research-service-ars--datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usda-agricultural-research-service-ars-/refs/heads/main/openapi/usda-agricultural-research-service-ars--datasets-api-openapi.yml
- filename: usda-agricultural-research-service-ars--food-search-api-openapi.yml
  format: yaml
  label: USDA Agricultural Research Service (ARS) Food Search API
  slug: usda-agricultural-research-service-ars--food-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usda-agricultural-research-service-ars-/refs/heads/main/openapi/usda-agricultural-research-service-ars--food-search-api-openapi.yml
- filename: usda-agricultural-research-service-ars--foods-api-openapi.yml
  format: yaml
  label: USDA Agricultural Research Service (ARS) Foods API
  slug: usda-agricultural-research-service-ars--foods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usda-agricultural-research-service-ars-/refs/heads/main/openapi/usda-agricultural-research-service-ars--foods-api-openapi.yml
consequence_counts:
  read: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Usda Agricultural Research Service Ars  Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'USDA Agricultural Research Service (ARS) exposes 12 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: USDA Agricultural Research Service (ARS)
provider_slug: usda-agricultural-research-service-ars-
slug: usda-agricultural-research-service-ars--agentic-access
source_filename: usda-agricultural-research-service-ars--agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/usda-agricultural-research-service-ars--datasets-api-openapi.yml, openapi/usda-agricultural-research-service-ars--food-search-api-openapi.yml,\n  openapi/usda-agricultural-research-service-ars--foods-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 12\n  by_consequence:\n    read: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /api/action/package_search\n  method: get\n  operationId: searchDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/action/package_show\n  method: get\n  operationId: getDataset\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/action/tag_list\n  method: get\n  operationId: listTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/action/organization_list\n  method: get\n  operationId: listOrganizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/action/datastore_search\n  method: get\n  operationId: searchDatastoreResource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /foods/search\n  method: get\n  operationId: searchFoodsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /foods/search\n  method: post\n  operationId: searchFoodsPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /food/{fdcId}\n  method: get\n  operationId: getFood\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /foods\n  method: get\n  operationId: getFoodsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /foods\n  method: post\n  operationId: getFoodsPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /foods/list\n  method: get\n  operationId: getFoodsListGet\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /foods/list\n  method: post\n  operationId: getFoodsListPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usda-agricultural-research-service-ars-/refs/heads/main/agentic-access/usda-agricultural-research-service-ars--agentic-access.yml
summary_line: 12 operations
tags:
- Federal Government
- Agriculture
- Food Safety
- Nutrition
- Open Data
- Research
---
