---
acting_count: 0
action_class_counts:
  connected: 10
api_specs:
- filename: constellation-brands-bottleshots-api-openapi.yml
  format: yaml
  label: Constellation Brands BottleShots API
  slug: constellation-brands-bottleshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constellation-brands/refs/heads/main/openapi/constellation-brands-bottleshots-api-openapi.yml
- filename: constellation-brands-hotsheets-api-openapi.yml
  format: yaml
  label: Constellation Brands HotSheets API
  slug: constellation-brands-hotsheets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constellation-brands/refs/heads/main/openapi/constellation-brands-hotsheets-api-openapi.yml
- filename: constellation-brands-items-api-openapi.yml
  format: yaml
  label: Constellation Brands Items API
  slug: constellation-brands-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constellation-brands/refs/heads/main/openapi/constellation-brands-items-api-openapi.yml
- filename: constellation-brands-neckhangers-api-openapi.yml
  format: yaml
  label: Constellation Brands NeckHangers API
  slug: constellation-brands-neckhangers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constellation-brands/refs/heads/main/openapi/constellation-brands-neckhangers-api-openapi.yml
- filename: constellation-brands-recipes-api-openapi.yml
  format: yaml
  label: Constellation Brands Recipes API
  slug: constellation-brands-recipes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constellation-brands/refs/heads/main/openapi/constellation-brands-recipes-api-openapi.yml
- filename: constellation-brands-shelftalkers-api-openapi.yml
  format: yaml
  label: Constellation Brands ShelfTalkers API
  slug: constellation-brands-shelftalkers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constellation-brands/refs/heads/main/openapi/constellation-brands-shelftalkers-api-openapi.yml
- filename: constellation-brands-tastingnotes-api-openapi.yml
  format: yaml
  label: Constellation Brands TastingNotes API
  slug: constellation-brands-tastingnotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constellation-brands/refs/heads/main/openapi/constellation-brands-tastingnotes-api-openapi.yml
consequence_counts:
  read: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Constellation Brands Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'Constellation Brands exposes 10 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Constellation Brands
provider_slug: constellation-brands
slug: constellation-brands-agentic-access
source_filename: constellation-brands-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/constellation-brands-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 10\n  by_consequence:\n    read: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /api/1.0/bottleShots\n  method: get\n  operationId: listBottleShots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/1.0/bottleShots/{gtin}\n  method: get\n  operationId: getBottleShot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/1.0/tastingNotes\n  method:\
  \ get\n  operationId: listTastingNotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/1.0/hotSheets\n  method: get\n  operationId: listHotSheets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/1.0/shelfTalkers\n  method: get\n  operationId: listShelfTalkers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/1.0/neckHangers\n  method: get\n  operationId: listNeckHangers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/1.0/recipes\n  method: get\n  operationId: listRecipes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/items\n  method: get\n  operationId: listItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/items/{itemId}\n  method: get\n  operationId: getItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/items/{itemId}/digitalAssets\n  method: get\n  operationId: getItemDigitalAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/constellation-brands/refs/heads/main/agentic-access/constellation-brands-agentic-access.yml
summary_line: 10 operations
tags:
- Alcohol
- Beer
- Beverages
- Digital Assets
- Fortune 500
- Spirits
- Wine
---
