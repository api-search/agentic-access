---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 8
api_specs:
- filename: sfxmint-com-generation-api-openapi.yml
  format: yaml
  label: SFXMint Generation API
  slug: sfxmint-com-generation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sfxmint-com/openapi/sfxmint-com-generation-api-openapi.yml
- filename: sfxmint-com-library-api-openapi.yml
  format: yaml
  label: SFXMint Library API
  slug: sfxmint-com-library-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sfxmint-com/openapi/sfxmint-com-library-api-openapi.yml
consequence_counts:
  physical: 1
  read: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sfxmint Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/orders
operation_count: 9
overview: 'SFXMint exposes 9 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SFXMint
provider_slug: sfxmint-com
slug: sfxmint-com-agentic-access
source_filename: sfxmint-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/sfxmint-com-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 8\n    acting: 1\n  by_consequence:\n    read: 8\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/search\n  method: get\n  operationId: searchSounds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sounds/{slug}\n  method: get\n  operationId: getSound\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/roles\n  method: get\n\
  \  operationId: listRoles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/roles/{role}\n  method: get\n  operationId: getRoleSound\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sets\n  method: get\n  operationId: listSets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sets/{id}\n  method: get\n  operationId: getSoundSet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dl/{file}\n  method: get\n  operationId: downloadSound\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/v1/orders\n  method: post\n  operationId: generateSound\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/orders/{id}\n  method: get\n  operationId: getGeneration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/sfxmint-com/agentic-access/sfxmint-com-agentic-access.yml
summary_line: 9 operations · 1 acting
tags:
- Sound Effects
- CC0
- AI Studio
- Games
- Free
---
