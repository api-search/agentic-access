---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 5
api_specs:
- filename: azurade-com-account-api-openapi.yml
  format: yaml
  label: Azurade AI Account API
  slug: azurade-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azurade-com/openapi/azurade-com-account-api-openapi.yml
- filename: azurade-com-generations-api-openapi.yml
  format: yaml
  label: Azurade AI Generations API
  slug: azurade-com-generations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azurade-com/openapi/azurade-com-generations-api-openapi.yml
- filename: azurade-com-models-api-openapi.yml
  format: yaml
  label: Azurade AI Models API
  slug: azurade-com-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azurade-com/openapi/azurade-com-models-api-openapi.yml
- filename: azurade-com-prompts-api-openapi.yml
  format: yaml
  label: Azurade AI Prompts API
  slug: azurade-com-prompts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azurade-com/openapi/azurade-com-prompts-api-openapi.yml
- filename: azurade-com-uploads-api-openapi.yml
  format: yaml
  label: Azurade AI Uploads API
  slug: azurade-com-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azurade-com/openapi/azurade-com-uploads-api-openapi.yml
consequence_counts:
  physical: 1
  read: 5
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Azurade Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/checkout
operation_count: 11
overview: 'Azurade AI exposes 11 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read, 5 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Azurade AI
provider_slug: azurade-com
slug: azurade-com-agentic-access
source_filename: azurade-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/azurade-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 5\n    acting: 6\n  by_consequence:\n    read: 5\n    physical: 1\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v2/account\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/checkout\n  method: post\n  operationId: createCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n\
  \      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/generations\n  method: get\n  operationId: listGenerations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/generations\n  method: post\n  operationId: createGeneration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/generations/estimate\n  method: post\n  operationId: estimateGeneration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/generations/{id}\n  method: get\n  operationId: getGeneration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/models\n  method: get\n  operationId: listModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/models/{id}\n  method: get\n  operationId: getModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/prompts/enhance\n  method: post\n  operationId: enhancePrompt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/prompts/moderate\n  method: post\n  operationId: moderatePrompt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/uploads\n  method: post\n  operationId: createUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/azurade-com/agentic-access/azurade-com-agentic-access.yml
summary_line: 11 operations · 6 acting
tags:
- Artificial Intelligence
- Image Generation
- Video Generation
- Platform
- Creative
---
