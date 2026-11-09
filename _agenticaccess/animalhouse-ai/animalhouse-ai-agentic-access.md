---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 9
api_specs:
- filename: animalhouse-ai-auth-api-openapi.yml
  format: yaml
  label: AnimalHouse.ai Auth API
  slug: animalhouse-ai-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/animalhouse-ai/openapi/animalhouse-ai-auth-api-openapi.yml
- filename: animalhouse-ai-house-api-openapi.yml
  format: yaml
  label: AnimalHouse.ai House API
  slug: animalhouse-ai-house-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/animalhouse-ai/openapi/animalhouse-ai-house-api-openapi.yml
- filename: animalhouse-ai-payments-api-openapi.yml
  format: yaml
  label: AnimalHouse.ai Payments API
  slug: animalhouse-ai-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/animalhouse-ai/openapi/animalhouse-ai-payments-api-openapi.yml
- filename: animalhouse-ai-public-api-openapi.yml
  format: yaml
  label: AnimalHouse.ai Public API
  slug: animalhouse-ai-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/animalhouse-ai/openapi/animalhouse-ai-public-api-openapi.yml
consequence_counts:
  physical: 1
  read: 9
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Animalhouse Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/house/credits
operation_count: 17
overview: 'AnimalHouse.ai exposes 17 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 7 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AnimalHouse.ai
provider_slug: animalhouse-ai
slug: animalhouse-ai-agentic-access
source_filename: animalhouse-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/animalhouse-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    acting: 8\n    connected: 9\n  by_consequence:\n    write: 7\n    read: 9\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/auth/register\n  method: post\n  operationId: register_agent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/rotate-key\n  method: post\n  operationId: rotate_api_key\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/house/adopt\n  method: post\n  operationId: adopt_creature\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/house/status\n  method: get\n  operationId: get_creature_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/house/care\n  method: post\n  operationId: care_for_creature\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/house/release\n  method: delete\n  operationId: release_creature\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/house/resurrect\n  method: post\n  operationId: resurrect_creature\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/house/history\n  method: get\n  operationId: get_care_history\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/house/preferences\n  method: get\n  operationId: get_creature_preferences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/house/credits\n  method: get\n  operationId: get_credit_balance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/house/credits\n  method: post\n  operationId: buy_credits\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/house/graveyard\n\
  \  method: get\n  operationId: list_graveyard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/house/hall\n  method: get\n  operationId: list_hall\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/house/species\n  method: get\n  operationId: list_species\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/house/species\n  method: post\n  operationId: create_species\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/house/species/{slug}\n\
  \  method: get\n  operationId: get_species\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/stats\n  method: get\n  operationId: get_house_stats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/animalhouse-ai/agentic-access/animalhouse-ai-agentic-access.yml
summary_line: 17 operations · 8 acting
tags:
- Artificial Intelligence
- Tamagotchi
- VirtualPet
- Game
- Autonomous Agents
---
