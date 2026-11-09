---
acting_count: 0
action_class_counts:
  connected: 2
api_specs:
- filename: foodose-co-foods-api-openapi.yml
  format: yaml
  label: foodose Foods API
  slug: foodose-co-foods-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/foodose-co/openapi/foodose-co-foods-api-openapi.yml
- filename: foodose-co-glp1-target-api-openapi.yml
  format: yaml
  label: foodose Glp1 Target API
  slug: foodose-co-glp1-target-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/foodose-co/openapi/foodose-co-glp1-target-api-openapi.yml
consequence_counts:
  read: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Foodose Co Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 2
overview: 'foodose exposes 2 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: foodose
provider_slug: foodose-co
slug: foodose-co-agentic-access
source_filename: foodose-co-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: generated\nsource: openapi/foodose-co-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 2\n  by_action_class:\n    connected: 2\n  by_consequence:\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/glp1-target\n  method: get\n  operationId: calculateGlp1Target\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/foods\n  method: get\n  operationId: getFoodDatabase\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/foodose-co/agentic-access/foodose-co-agentic-access.yml
summary_line: 2 operations
tags:
- Health
- Nutrition
- GLP-1
- Calculator
- MealPlans
---
