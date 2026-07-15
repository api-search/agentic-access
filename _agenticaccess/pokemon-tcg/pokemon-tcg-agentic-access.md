---
acting_count: 0
action_class_counts:
  connected: 8
api_specs:
- filename: pokemon-tcg-openapi.yml
  format: yaml
  label: Pokémon TCG Cards API
  slug: pokemon-tcg-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pokemon-tcg/refs/heads/main/openapi/pokemon-tcg-openapi.yml
- filename: pokemon-tcg-openapi.yml
  format: yaml
  label: Pokémon TCG Sets API
  slug: pokemon-tcg-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pokemon-tcg/refs/heads/main/openapi/pokemon-tcg-openapi.yml
- filename: pokemon-tcg-openapi.yml
  format: yaml
  label: Pokémon TCG Metadata API
  slug: pokemon-tcg-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pokemon-tcg/refs/heads/main/openapi/pokemon-tcg-openapi.yml
consequence_counts:
  read: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Pokemon Tcg Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Pokémon TCG API exposes 8 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Pokémon TCG API
provider_slug: pokemon-tcg
slug: pokemon-tcg-agentic-access
source_filename: pokemon-tcg-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/pokemon-tcg-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 8\n  by_consequence:\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /cards\n  method: get\n  operationId: searchCards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cards/{id}\n  method: get\n  operationId: getCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sets\n  method: get\n  operationId: searchSets\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sets/{id}\n  method: get\n  operationId: getSet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /types\n  method: get\n  operationId: getTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subtypes\n  method: get\n  operationId: getSubtypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /supertypes\n  method: get\n  operationId: getSupertypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rarities\n  method: get\n  operationId: getRarities\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pokemon-tcg/refs/heads/main/agentic-access/pokemon-tcg-agentic-access.yml
summary_line: 8 operations
tags:
- Pokemon
- Trading Cards
- TCG
- Gaming
- Card Games
- Collectibles
- Card Prices
---
