---
acting_count: 0
action_class_counts:
  connected: 10
api_specs:
- filename: jelly-belly-openapi.yml
  format: yaml
  label: Jelly Belly Wiki API
  slug: jelly-belly-wiki-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jelly-belly/refs/heads/main/openapi/jelly-belly-openapi.yml
consequence_counts:
  read: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Jelly Belly Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'Jelly Belly exposes 10 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Jelly Belly
provider_slug: jelly-belly
slug: jelly-belly-agentic-access
source_filename: jelly-belly-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/jelly-belly-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 10\n  by_consequence:\n    read: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /api/Beans\n  method: get\n  operationId: listBeans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Beans/{id}\n  method: get\n  operationId: getBean\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Combinations\n  method: get\n  operationId: listCombinations\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Combinations/{id}\n  method: get\n  operationId: getCombination\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Facts\n  method: get\n  operationId: listFacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Facts/{id}\n  method: get\n  operationId: getFact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/MileStones\n  method: get\n  operationId: listMilestones\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/MileStones/{id}\n\
  \  method: get\n  operationId: getMilestone\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Recipes\n  method: get\n  operationId: listRecipes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Recipes/{id}\n  method: get\n  operationId: getRecipe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jelly-belly/refs/heads/main/agentic-access/jelly-belly-agentic-access.yml
summary_line: 10 operations
tags:
- Beans
- Candy
- Confectionery
- Food
- Jelly Beans
- Recipes
---
