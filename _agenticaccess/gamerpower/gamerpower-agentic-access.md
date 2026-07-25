---
acting_count: 0
action_class_counts:
  connected: 4
api_specs:
- filename: gamerpower-filter-api-openapi.yml
  format: yaml
  label: GamerPower Filter API
  slug: gamerpower-filter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gamerpower/refs/heads/main/openapi/gamerpower-filter-api-openapi.yml
- filename: gamerpower-giveaways-api-openapi.yml
  format: yaml
  label: GamerPower Giveaways API
  slug: gamerpower-giveaways-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gamerpower/refs/heads/main/openapi/gamerpower-giveaways-api-openapi.yml
- filename: gamerpower-worth-api-openapi.yml
  format: yaml
  label: GamerPower Worth API
  slug: gamerpower-worth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gamerpower/refs/heads/main/openapi/gamerpower-worth-api-openapi.yml
consequence_counts:
  read: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Gamerpower Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'GamerPower exposes 4 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: GamerPower
provider_slug: gamerpower
slug: gamerpower-agentic-access
source_filename: gamerpower-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/gamerpower.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    connected: 4\n  by_consequence:\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /giveaways\n  method: get\n  operationId: listGiveaways\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /giveaway\n  method: get\n  operationId: getGiveaway\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /filter\n  method: get\n  operationId: filterGiveaways\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /worth\n  method: get\n  operationId: getWorth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gamerpower/refs/heads/main/agentic-access/gamerpower-agentic-access.yml
summary_line: 4 operations
tags:
- Games And Comics
- Giveaways
- Free Games
- Public APIs
---
