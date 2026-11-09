---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 7
api_specs:
- filename: creativefabrica-generations-api-openapi.yml
  format: yaml
  label: Creative Fabrica Generations API
  slug: creativefabrica-generations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creativefabrica/openapi/creativefabrica-generations-api-openapi.yml
- filename: creativefabrica-models-api-openapi.yml
  format: yaml
  label: Creative Fabrica Models API
  slug: creativefabrica-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creativefabrica/openapi/creativefabrica-models-api-openapi.yml
- filename: creativefabrica-presets-api-openapi.yml
  format: yaml
  label: Creative Fabrica Presets API
  slug: creativefabrica-presets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creativefabrica/openapi/creativefabrica-presets-api-openapi.yml
- filename: creativefabrica-voices-api-openapi.yml
  format: yaml
  label: Creative Fabrica Voices API
  slug: creativefabrica-voices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creativefabrica/openapi/creativefabrica-voices-api-openapi.yml
consequence_counts:
  read: 7
  safety-critical: 1
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Creativefabrica Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/presets/{presetId}/generations
operation_count: 10
overview: 'Creative Fabrica exposes 10 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read, 2 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Creative Fabrica
provider_slug: creativefabrica
slug: creativefabrica-agentic-access
source_filename: creativefabrica-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/creativefabrica-idea-ai-genai-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    acting: 3\n    connected: 7\n  by_consequence:\n    write: 2\n    read: 7\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /v1/generations\n  method: post\n  operationId: createGeneration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/generations\n  method: get\n  operationId: listGenerations\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/generations/{generationId}\n  method: get\n  operationId: getGeneration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/voices/{voiceCatalog}\n  method: get\n  operationId: listVoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/models\n  method: get\n  operationId: listModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/models/{model}\n  method: get\n  operationId: getModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/models/{model}/cost\n  method: post\n  operationId: calculateModelCost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/presets\n  method: get\n  operationId: listPresets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/presets/{presetId}\n  method: get\n  operationId: getPreset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/presets/{presetId}/generations\n  method: post\n  operationId: createPresetGeneration\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/creativefabrica/agentic-access/creativefabrica-agentic-access.yml
summary_line: 10 operations · 3 acting · 1 human-in-the-loop
tags:
- Company
- Creative Marketplace
- Digital Assets
- Fonts
- Graphics
- Print on Demand
- Embroidery
- Design Tools
- Subscription Service
- Amsterdam
---
