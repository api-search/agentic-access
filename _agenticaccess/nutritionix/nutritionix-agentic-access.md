---
acting_count: 0
action_class_counts:
  connected: 6
api_specs:
- filename: nutritionix-brands-api-openapi.yml
  format: yaml
  label: Nutritionix Brands API
  slug: nutritionix-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutritionix/refs/heads/main/openapi/nutritionix-brands-api-openapi.yml
- filename: nutritionix-item-api-openapi.yml
  format: yaml
  label: Nutritionix Item API
  slug: nutritionix-item-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutritionix/refs/heads/main/openapi/nutritionix-item-api-openapi.yml
- filename: nutritionix-natural-language-api-openapi.yml
  format: yaml
  label: Nutritionix Natural Language API
  slug: nutritionix-natural-language-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutritionix/refs/heads/main/openapi/nutritionix-natural-language-api-openapi.yml
- filename: nutritionix-search-api-openapi.yml
  format: yaml
  label: Nutritionix Search API
  slug: nutritionix-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutritionix/refs/heads/main/openapi/nutritionix-search-api-openapi.yml
consequence_counts:
  read: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Nutritionix Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Nutritionix exposes 6 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Nutritionix
provider_slug: nutritionix
slug: nutritionix-agentic-access
source_filename: nutritionix-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/nutritionix-brands-api-openapi.yml, openapi/nutritionix-item-api-openapi.yml,\n  openapi/nutritionix-natural-language-api-openapi.yml, openapi/nutritionix-search-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 6\n  by_consequence:\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /brands/search\n  method: get\n  operationId: searchBrands\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/item\n  method: get\n  operationId: searchItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /item\n  method: get\n  operationId: getItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /natural/nutrients\n  method: post\n  operationId: getNaturalNutrients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /natural/exercise\n  method: post\n  operationId: getNaturalExercise\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/instant\n  method: get\n  operationId: searchInstant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nutritionix/refs/heads/main/agentic-access/nutritionix-agentic-access.yml
summary_line: 6 operations
tags:
- Restaurant
- Health
- Nutrition
- Food
- Fitness
- Public APIs
- Food and Beverage
---
