---
acting_count: 0
action_class_counts:
  connected: 12
api_specs:
- filename: tinyplates-dev-health-api-openapi.yml
  format: yaml
  label: tinyplates-dev Health API
  slug: tinyplates-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tinyplates-dev/openapi/tinyplates-dev-health-api-openapi.yml
- filename: tinyplates-dev-ingredients-api-openapi.yml
  format: yaml
  label: tinyplates-dev Ingredients API
  slug: tinyplates-dev-ingredients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tinyplates-dev/openapi/tinyplates-dev-ingredients-api-openapi.yml
- filename: tinyplates-dev-pantry-api-openapi.yml
  format: yaml
  label: tinyplates-dev Pantry API
  slug: tinyplates-dev-pantry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tinyplates-dev/openapi/tinyplates-dev-pantry-api-openapi.yml
- filename: tinyplates-dev-popular-api-openapi.yml
  format: yaml
  label: tinyplates-dev Popular API
  slug: tinyplates-dev-popular-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tinyplates-dev/openapi/tinyplates-dev-popular-api-openapi.yml
- filename: tinyplates-dev-recipes-api-openapi.yml
  format: yaml
  label: tinyplates-dev Recipes API
  slug: tinyplates-dev-recipes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tinyplates-dev/openapi/tinyplates-dev-recipes-api-openapi.yml
- filename: tinyplates-dev-root-api-openapi.yml
  format: yaml
  label: tinyplates-dev Root API
  slug: tinyplates-dev-root-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tinyplates-dev/openapi/tinyplates-dev-root-api-openapi.yml
- filename: tinyplates-dev-search-api-openapi.yml
  format: yaml
  label: tinyplates-dev Search API
  slug: tinyplates-dev-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tinyplates-dev/openapi/tinyplates-dev-search-api-openapi.yml
- filename: tinyplates-dev-shoppinglist-api-openapi.yml
  format: yaml
  label: tinyplates-dev Shopping List API
  slug: tinyplates-dev-shoppinglist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tinyplates-dev/openapi/tinyplates-dev-shoppinglist-api-openapi.yml
- filename: tinyplates-dev-status-api-openapi.yml
  format: yaml
  label: tinyplates-dev Status API
  slug: tinyplates-dev-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tinyplates-dev/openapi/tinyplates-dev-status-api-openapi.yml
- filename: tinyplates-dev-substitutions-api-openapi.yml
  format: yaml
  label: tinyplates-dev Substitutions API
  slug: tinyplates-dev-substitutions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tinyplates-dev/openapi/tinyplates-dev-substitutions-api-openapi.yml
consequence_counts:
  read: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tinyplates Dev Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'tinyplates-dev exposes 12 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: tinyplates-dev
provider_slug: tinyplates-dev
slug: tinyplates-dev-agentic-access
source_filename: tinyplates-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/tinyplates-dev-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 12\n  by_consequence:\n    read: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /health\n  method: get\n  operationId: health.check\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pantry\n  method: get\n  operationId: pantry.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /popular\n  method: get\n  operationId: popular.list\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recipes\n  method: get\n  operationId: recipes.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recipes/{id}\n  method: get\n  operationId: recipes.byId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: root.index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search\n  method: get\n  operationId: search.search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shopping-list\n  method: get\n  operationId:\
  \ shoppingList.build\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ingredients\n  method: get\n  operationId: ingredients.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vocabularies\n  method: get\n  operationId: ingredients.vocabularies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status\n  method: get\n  operationId: status.read\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /substitutions\n  method: get\n  operationId: substitutions.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n  \
  \    max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/tinyplates-dev/agentic-access/tinyplates-dev-agentic-access.yml
summary_line: 12 operations
tags:
- Food
- Recipes
- Search
- Developers
---
