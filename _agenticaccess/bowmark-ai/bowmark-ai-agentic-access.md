---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 7
api_specs:
- filename: bowmark-ai-library-api-openapi.yml
  format: yaml
  label: Bowmark AI Library API
  slug: bowmark-ai-library-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bowmark-ai/openapi/bowmark-ai-library-api-openapi.yml
- filename: bowmark-ai-recipes-api-openapi.yml
  format: yaml
  label: Bowmark AI Recipes API
  slug: bowmark-ai-recipes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bowmark-ai/openapi/bowmark-ai-recipes-api-openapi.yml
- filename: bowmark-ai-run-api-openapi.yml
  format: yaml
  label: Bowmark AI Run API
  slug: bowmark-ai-run-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bowmark-ai/openapi/bowmark-ai-run-api-openapi.yml
- filename: bowmark-ai-scripts-api-openapi.yml
  format: yaml
  label: Bowmark AI Scripts API
  slug: bowmark-ai-scripts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bowmark-ai/openapi/bowmark-ai-scripts-api-openapi.yml
- filename: bowmark-ai-sites-api-openapi.yml
  format: yaml
  label: Bowmark AI Sites API
  slug: bowmark-ai-sites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bowmark-ai/openapi/bowmark-ai-sites-api-openapi.yml
consequence_counts:
  read: 7
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bowmark Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'Bowmark AI exposes 13 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bowmark AI
provider_slug: bowmark-ai
slug: bowmark-ai-agentic-access
source_filename: bowmark-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/bowmark-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 7\n    acting: 6\n  by_consequence:\n    read: 7\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/library\n  method: get\n  operationId: getLibrary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/run\n  method: post\n  operationId: run\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/recipes\n  method: get\n  operationId: listRecipes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/recipes/{id}\n  method: get\n  operationId: getRecipe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/recipes/{id}\n  method: post\n  operationId: runRecipe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/scripts\n  method: get\n  operationId: listScripts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/scripts\n  method: post\n  operationId: saveScript\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/scripts/{ref}\n  method: get\n  operationId: getScript\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/scripts/{ref}\n  method: delete\n  operationId: deleteScript\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/scripts/{ref}/run\n  method: post\n  operationId:\
  \ runScript\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sites\n  method: get\n  operationId: listSites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sites/{site}/openapi.json\n  method: get\n  operationId: getSiteSpec\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sites/{site}/{fn}\n  method: post\n  operationId: callSiteFunction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/bowmark-ai/agentic-access/bowmark-ai-agentic-access.yml
summary_line: 13 operations · 6 acting
tags:
- Artificial Intelligence
- Automation
- Web
- Data Extraction
- Platform
- Company
---
