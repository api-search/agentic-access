---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 6
api_specs:
- filename: food-info-apiv1-api-openapi.yml
  format: yaml
  label: Food Info API V1 API
  slug: food-info-apiv1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/food-info/refs/heads/main/openapi/food-info-apiv1-api-openapi.yml
- filename: food-info-recipesapi-api-openapi.yml
  format: yaml
  label: Food Info Recipes API API
  slug: food-info-recipesapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/food-info/refs/heads/main/openapi/food-info-recipesapi-api-openapi.yml
consequence_counts:
  read: 6
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Food Info Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Food Info exposes 8 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Food Info
provider_slug: food-info
slug: food-info-agentic-access
source_filename: food-info-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: generated\nsource: openapi/food-info-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 6\n    acting: 2\n  by_consequence:\n    read: 6\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/nutrients\n  method: get\n  operationId: listNutrients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/foods/search\n  method: get\n  operationId: searchFoods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/foods/{id}\n  method:\
  \ get\n  operationId: getFood\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/foods/{id}/panel\n  method: get\n  operationId: getFoodNutrientPanel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/nutrients/{nutrientId}/top-foods\n  method: get\n  operationId: listTopFoodsByNutrient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/nutrients/{nutrientId}/bottom-foods\n  method: get\n  operationId: listBottomFoodsByNutrient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/recipes/parse\n  method: post\n  operationId: parseRecipeIngredients\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/recipes/analyze\n  method: post\n  operationId: analyzeRecipeNutrition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/food-info/refs/heads/main/agentic-access/food-info-agentic-access.yml
summary_line: 8 operations · 2 acting
tags:
- Nutrition
- Food
- food-composition
- Nutrients
- Data
- Open Data
- Dietetics
- Recipes
- Health
- Research
---
