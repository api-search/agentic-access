---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 22
api_specs:
- filename: profit-rhino-auth-api-openapi.yml
  format: yaml
  label: Profit Rhino Auth API
  slug: profit-rhino-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/profit-rhino/openapi/profit-rhino-auth-api-openapi.yml
- filename: profit-rhino-businessinformation-api-openapi.yml
  format: yaml
  label: Profit Rhino Business Information API
  slug: profit-rhino-businessinformation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/profit-rhino/openapi/profit-rhino-businessinformation-api-openapi.yml
- filename: profit-rhino-manufacturer-api-openapi.yml
  format: yaml
  label: Profit Rhino Manufacturer API
  slug: profit-rhino-manufacturer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/profit-rhino/openapi/profit-rhino-manufacturer-api-openapi.yml
- filename: profit-rhino-optionboard-api-openapi.yml
  format: yaml
  label: Profit Rhino Option Board API
  slug: profit-rhino-optionboard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/profit-rhino/openapi/profit-rhino-optionboard-api-openapi.yml
- filename: profit-rhino-partcategory-api-openapi.yml
  format: yaml
  label: Profit Rhino Part Category API
  slug: profit-rhino-partcategory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/profit-rhino/openapi/profit-rhino-partcategory-api-openapi.yml
- filename: profit-rhino-parts-api-openapi.yml
  format: yaml
  label: Profit Rhino Parts API
  slug: profit-rhino-parts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/profit-rhino/openapi/profit-rhino-parts-api-openapi.yml
- filename: profit-rhino-partsmarkup-api-openapi.yml
  format: yaml
  label: Profit Rhino Parts Markup API
  slug: profit-rhino-partsmarkup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/profit-rhino/openapi/profit-rhino-partsmarkup-api-openapi.yml
- filename: profit-rhino-taskcategory-api-openapi.yml
  format: yaml
  label: Profit Rhino Task Category API
  slug: profit-rhino-taskcategory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/profit-rhino/openapi/profit-rhino-taskcategory-api-openapi.yml
- filename: profit-rhino-tasks-api-openapi.yml
  format: yaml
  label: Profit Rhino Tasks API
  slug: profit-rhino-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/profit-rhino/openapi/profit-rhino-tasks-api-openapi.yml
- filename: profit-rhino-vendors-api-openapi.yml
  format: yaml
  label: Profit Rhino Vendors API
  slug: profit-rhino-vendors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/profit-rhino/openapi/profit-rhino-vendors-api-openapi.yml
consequence_counts:
  read: 22
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Profit Rhino Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 23
overview: 'Profit Rhino exposes 23 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Profit Rhino
provider_slug: profit-rhino
slug: profit-rhino-agentic-access
source_filename: profit-rhino-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: generated\nsource: openapi/profit-rhino-profitrhino-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 22\n    acting: 1\n  by_consequence:\n    read: 22\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/Brand\n  method: get\n  operationId: Manufacturer_GET_getBrand\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/OptionMask/{Id}\n  method: get\n  operationId: OptionBoard_GET_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v2/OptionMasks\n  method: get\n  operationId: OptionBoard_GET_GetAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/PartCategories\n  method: get\n  operationId: PartCategory_GET_GetAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/PartCategory/{Id}\n  method: get\n  operationId: PartCategory_GET_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/PartCategory/{Id}/ProductLines\n  method: get\n  operationId: PartCategory_GET_GetAllProducLines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/ProductLine/{Id}\n  method: get\n  operationId: PartCategory_GET_GetProducLine\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/ProductLines\n  method: get\n  operationId: PartCategory_GET_GetAllProducLine\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/TaskCategories\n  method: get\n  operationId: TaskCategory_GET_Categories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/TaskCategories/{id}\n  method: get\n  operationId: TaskCategory_GET_GetCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/TaskCategories/{id}/TaskCategories\n  method: get\n  operationId: TaskCategory_GET_GetAllSubCategories\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/TaskCategories/{id}/tasks\n  method: get\n  operationId: Tasks_GET_GetAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/Tasks\n  method: get\n  operationId: Tasks_GET_GetAllTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/Vendors\n  method: get\n  operationId: Vendors_GET_GetAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/Vendors/{Id}\n  method: get\n  operationId: Vendors_GET_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v2/auth\n  method: post\n  operationId: Auth_POST_Login\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/businessinformation/{id}\n  method: get\n  operationId: BusinessInformation_GET_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/manufacturer\n  method: get\n  operationId: Manufacturer_GET_getManufacturer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/part/{Id}\n  method: get\n  operationId: Parts_GET_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v2/part/{id}/tasks\n  method: get\n  operationId: Parts_GET_GetPartTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/part/{id}/vendors\n  method: get\n  operationId: Parts_GET_GetPartVendors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partsmarkup\n  method: get\n  operationId: PartsMarkup_GET_GetAllMarkups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/productline/{Id}/parts\n  method: get\n  operationId: Parts_GET_Partbyproductline\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/profit-rhino/agentic-access/profit-rhino-agentic-access.yml
summary_line: 23 operations · 1 acting
tags:
- Company
- Flat Rate
- Contractor
- HVAC
- Software
- sales-tool
---
