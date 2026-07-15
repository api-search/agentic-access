---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 4
api_specs:
- filename: edamam-nutrition-analysis-api-openapi.yml
  format: yaml
  label: Edamam Nutrition Analysis API
  slug: edamam-nutrition-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edamam/main/openapi/edamam-nutrition-analysis-api-openapi.yml
- filename: edamam-food-and-grocery-database-api-openapi.yml
  format: yaml
  label: Edamam Food and Grocery Database API
  slug: edamam-food-and-grocery-database-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edamam/main/openapi/edamam-food-and-grocery-database-api-openapi.yml
- filename: edamam-recipe-search-api-openapi.yml
  format: yaml
  label: Edamam Recipe Search API
  slug: edamam-recipe-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edamam/main/openapi/edamam-recipe-search-api-openapi.yml
- filename: edamam-meal-planner-api-openapi.yml
  format: yaml
  label: Edamam Meal Planner API
  slug: edamam-meal-planner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edamam/main/openapi/edamam-meal-planner-api-openapi.yml
consequence_counts:
  read: 4
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Edamam Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Edamam exposes 7 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Edamam
provider_slug: edamam
slug: edamam-agentic-access
source_filename: edamam-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/edamam-food-and-grocery-database-api-openapi.yml, openapi/edamam-meal-planner-api-openapi.yml,\n  openapi/edamam-nutrition-analysis-api-openapi.yml, openapi/edamam-recipe-search-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 4\n    acting: 3\n  by_consequence:\n    read: 4\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /api/food-database/v2/parser\n  method: get\n  operationId: parseFood\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/food-database/v2/nutrients\n  method: post\n  operationId: foodNutrients\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/meal-planner/v1/{app_id}/select\n  method: post\n  operationId: selectMealPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/nutrition-details\n  method: post\n  operationId: analyzeRecipe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/nutrition-data\n  method: get\n  operationId: analyzeIngredient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/recipes/v2\n  method: get\n  operationId: searchRecipes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/recipes/v2/{id}\n  method: get\n  operationId: getRecipeById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edamam/refs/heads/main/agentic-access/edamam-agentic-access.yml
summary_line: 7 operations · 3 acting
tags:
- Restaurant
- Food
- Nutrition
- UPC
---
