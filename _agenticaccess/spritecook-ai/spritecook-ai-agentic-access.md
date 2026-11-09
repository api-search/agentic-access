---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 8
api_specs:
- filename: spritecook-ai-account-api-openapi.yml
  format: yaml
  label: spritecook-ai Account API
  slug: spritecook-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spritecook-ai/openapi/spritecook-ai-account-api-openapi.yml
- filename: spritecook-ai-animation-api-openapi.yml
  format: yaml
  label: spritecook-ai Animation API
  slug: spritecook-ai-animation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spritecook-ai/openapi/spritecook-ai-animation-api-openapi.yml
- filename: spritecook-ai-assets-api-openapi.yml
  format: yaml
  label: spritecook-ai Assets API
  slug: spritecook-ai-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spritecook-ai/openapi/spritecook-ai-assets-api-openapi.yml
- filename: spritecook-ai-catalog-api-openapi.yml
  format: yaml
  label: spritecook-ai Catalog API
  slug: spritecook-ai-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spritecook-ai/openapi/spritecook-ai-catalog-api-openapi.yml
- filename: spritecook-ai-generation-api-openapi.yml
  format: yaml
  label: spritecook-ai Generation API
  slug: spritecook-ai-generation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spritecook-ai/openapi/spritecook-ai-generation-api-openapi.yml
- filename: spritecook-ai-jobs-api-openapi.yml
  format: yaml
  label: spritecook-ai Jobs API
  slug: spritecook-ai-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spritecook-ai/openapi/spritecook-ai-jobs-api-openapi.yml
consequence_counts:
  physical: 1
  read: 8
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Spritecook Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/api/assets/{asset_id}/alpha-cutoff
operation_count: 21
overview: 'spritecook-ai exposes 21 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 12 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: spritecook-ai
provider_slug: spritecook-ai
slug: spritecook-ai-agentic-access
source_filename: spritecook-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/spritecook-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    connected: 8\n    acting: 13\n  by_consequence:\n    read: 8\n    write: 12\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/api/models\n  method: get\n  operationId: getModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - generate\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/character-workflows\n  method: get\n  operationId: getCharacterWorkflows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - generate\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/characters\n  method: post\n  operationId: generateCharacter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - generate\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api/characters/{character_id}/animations\n  method: post\n  operationId: generateCharacterAnimations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - generate\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api/character-animation-runs/{run_id}\n  method: get\n  operationId: getCharacterAnimationRun\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    scope:\n    - generate\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/generate\n  method: post\n  operationId: generate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - generate\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api/tilesets/options\n  method: get\n  operationId: getTilesetOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - generate\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/tilesets\n  method: post\n  operationId: generateTileset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - generate\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api/animate\n  method: post\n  operationId: animate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - generate\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api/remove-background\n  method: post\n  operationId: removeBackground\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - generate\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api/assets/import\n  method: post\n  operationId: importAsset\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    scope:\n    - generate\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api/assets/{asset_id}/auto-slice\n  method: post\n  operationId: autoSliceAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - generate\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api/jobs/{job_id}\n  method: get\n  operationId: getJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read_assets\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/jobs/{job_id}/cancel\n  method: post\n  operationId: cancelJob\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - generate\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api/assets/recent\n  method: get\n  operationId: getRecentAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read_assets\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/assets/{asset_id}/alpha-cutoff\n  method: put\n  operationId: setAssetAlphaCutoff\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - generate\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/api/assets/{asset_id}\n  method: get\n  operationId: getAssetMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read_assets\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/credits\n  method: get\n  operationId: getCredits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read_credits\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/generate-sync\n  method: post\n  operationId: generateSync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - generate\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api/tilesets-sync\n  method: post\n  operationId: generateTilesetSync\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    scope:\n    - generate\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api/animate-sync\n  method: post\n  operationId: animateSync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - generate\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/spritecook-ai/agentic-access/spritecook-ai-agentic-access.yml
summary_line: 21 operations · 13 acting
tags:
- Artificial Intelligence
- Pixel Art
- Game Development
- Software-as-a-Service
- Graphics
---
