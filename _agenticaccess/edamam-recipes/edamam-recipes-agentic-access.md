---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 7
api_specs:
- filename: edamam-recipe-search-v2-openapi.yml
  format: yaml
  label: Edamam Recipe Search API
  slug: edamam-recipe-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edamam-recipes/refs/heads/main/openapi/edamam-recipe-search-v2-openapi.yml
- filename: edamam-nutrition-analysis-v1-openapi.yml
  format: yaml
  label: Edamam Nutrition Analysis API
  slug: edamam-nutrition-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edamam-recipes/refs/heads/main/openapi/edamam-nutrition-analysis-v1-openapi.yml
- filename: edamam-food-database-v2-openapi.yml
  format: yaml
  label: Edamam Food Database API
  slug: edamam-food-database-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edamam-recipes/refs/heads/main/openapi/edamam-food-database-v2-openapi.yml
- filename: edamam-meal-planner-v1-openapi.yml
  format: yaml
  label: Edamam Meal Planner API
  slug: edamam-meal-planner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edamam-recipes/refs/heads/main/openapi/edamam-meal-planner-v1-openapi.yml
consequence_counts:
  read: 7
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Edamam Recipes Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'Edamam exposes 14 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Edamam
provider_slug: edamam-recipes
slug: edamam-recipes-agentic-access
source_filename: edamam-recipes-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/edamam-food-database-v2-openapi.yml, openapi/edamam-meal-planner-v1-openapi.yml,\n  openapi/edamam-nutrition-analysis-v1-openapi.yml, openapi/edamam-recipe-search-v2-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 7\n    acting: 7\n  by_consequence:\n    read: 7\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /api/food-database/v2/parser\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/food-database/v2/nutrients\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/food-database/nutrients-from-image\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auto-complete\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/meal-planner/v1/{app_id}/select\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - app_id\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/daily-values/v1/values\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - app_id\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/recipes/v2/by-uri\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/shopping-list/v2\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/nutrition-details\n  method:\
  \ post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/nutrition-data\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/recipes/v2\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/recipes/v2/by-uri\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/recipes/v2/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/shopping-list/v2\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edamam-recipes/refs/heads/main/agentic-access/edamam-recipes-agentic-access.yml
summary_line: 14 operations · 7 acting
tags:
- Food And Drink
- Recipes
- Nutrition
- Diet
- Allergens
- Meal Planning
- Sustainability
- Carbon Footprint
- Public APIs
---
