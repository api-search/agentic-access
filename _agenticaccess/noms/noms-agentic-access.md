---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 10
api_specs:
- filename: noms-brands-api-openapi.yml
  format: yaml
  label: Noms Brands API
  slug: noms-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noms/refs/heads/main/openapi/noms-brands-api-openapi.yml
- filename: noms-foodgroups-api-openapi.yml
  format: yaml
  label: Noms Food Groups API
  slug: noms-foodgroups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noms/refs/heads/main/openapi/noms-foodgroups-api-openapi.yml
- filename: noms-foods-api-openapi.yml
  format: yaml
  label: Noms Foods API
  slug: noms-foods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noms/refs/heads/main/openapi/noms-foods-api-openapi.yml
- filename: noms-market-api-openapi.yml
  format: yaml
  label: Noms Market API
  slug: noms-market-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noms/refs/heads/main/openapi/noms-market-api-openapi.yml
- filename: noms-nutrients-api-openapi.yml
  format: yaml
  label: Noms Nutrients API
  slug: noms-nutrients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noms/refs/heads/main/openapi/noms-nutrients-api-openapi.yml
- filename: noms-usage-api-openapi.yml
  format: yaml
  label: Noms Usage API
  slug: noms-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noms/refs/heads/main/openapi/noms-usage-api-openapi.yml
consequence_counts:
  read: 10
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Noms Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'Noms exposes 11 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Noms
provider_slug: noms
slug: noms-agentic-access
source_filename: noms-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: generated\nsource: openapi/noms-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 10\n    acting: 1\n  by_consequence:\n    read: 10\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/foods\n  method: get\n  operationId: foodsListFoods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/foods/{id}\n  method: get\n  operationId: foodsGetFood\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/nutrients\n  method: get\n  operationId:\
  \ nutrientsListNutrients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/nutrients/{id}\n  method: get\n  operationId: nutrientsGetNutrient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/food-groups\n  method: get\n  operationId: foodGroupsListFoodGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/food-groups/{id}\n  method: get\n  operationId: foodGroupsGetFoodGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/brands\n  method: get\n  operationId: brandsListBrands\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n   \
  \ subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/brands/{id}\n  method: get\n  operationId: brandsGetBrand\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/usage\n  method: get\n  operationId: usageUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/market\n  method: get\n  operationId: marketGetMarket\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/market\n  method: put\n  operationId: marketSetMarket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/noms/refs/heads/main/agentic-access/noms-agentic-access.yml
summary_line: 11 operations · 1 acting
tags:
- Company
- Nutrition
- Food
- Data
- Health
---
