---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 9
api_specs:
- filename: apispec
  format: yaml
  label: USDA FoodData Central API
  slug: fooddata-central-api
  spec_type: OpenAPI
  url: https://fdc.nal.usda.gov/portal-data/external/apispec
- filename: usda-ars-ag-data-commons-openapi.yml
  format: yaml
  label: USDA Ag Data Commons CKAN API
  slug: ag-data-commons-ckan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usda-agricultural-research-service-ars-/refs/heads/main/openapi/usda-ars-ag-data-commons-openapi.yml
consequence_counts:
  read: 9
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Usda Agricultural Research Service Ars  Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'USDA Agricultural Research Service (ARS) exposes 12 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: USDA Agricultural Research Service (ARS)
provider_slug: usda-agricultural-research-service-ars-
slug: usda-agricultural-research-service-ars--agentic-access
source_filename: usda-agricultural-research-service-ars--agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/usda-ars-ag-data-commons-openapi.yml, openapi/usda-ars-fooddata-central-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 9\n    acting: 3\n  by_consequence:\n    read: 9\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /api/action/package_search\n  method: get\n  operationId: searchDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/action/package_show\n  method: get\n  operationId: getDataset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/action/tag_list\n  method: get\n  operationId: listTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/action/organization_list\n  method: get\n  operationId: listOrganizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/action/datastore_search\n  method: get\n  operationId: searchDatastoreResource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /food/{fdcId}\n  method: get\n  operationId: getFood\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /foods\n  method: get\n  operationId: getFoodsGet\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /foods\n  method: post\n  operationId: getFoodsPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /foods/list\n  method: get\n  operationId: getFoodsListGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /foods/list\n  method: post\n  operationId: getFoodsListPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /foods/search\n  method: get\n  operationId: searchFoodsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /foods/search\n  method: post\n  operationId: searchFoodsPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usda-agricultural-research-service-ars-/refs/heads/main/agentic-access/usda-agricultural-research-service-ars--agentic-access.yml
summary_line: 12 operations · 3 acting
tags:
- Federal Government
- Agriculture
- Food Safety
- Nutrition
- Open Data
- Research
---
