---
acting_count: 0
action_class_counts:
  connected: 8
api_specs:
- filename: openapi.yml
  format: yaml
  label: Superhero API
  slug: superhero-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superhero/refs/heads/main/openapi/openapi.yml
consequence_counts:
  read: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Superhero Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Superhero API exposes 8 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Superhero API
provider_slug: superhero
slug: superhero-agentic-access
source_filename: superhero-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 8\n  by_consequence:\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /{access-token}/{id}\n  method: get\n  operationId: getCharacterById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{access-token}/{id}/powerstats\n  method: get\n  operationId: getCharacterPowerstats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{access-token}/{id}/biography\n  method:\
  \ get\n  operationId: getCharacterBiography\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{access-token}/{id}/appearance\n  method: get\n  operationId: getCharacterAppearance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{access-token}/{id}/work\n  method: get\n  operationId: getCharacterWork\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{access-token}/{id}/connections\n  method: get\n  operationId: getCharacterConnections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{access-token}/{id}/image\n  method: get\n  operationId: getCharacterImage\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{access-token}/search/{name}\n  method: get\n  operationId: searchCharacterByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superhero/refs/heads/main/agentic-access/superhero-agentic-access.yml
summary_line: 8 operations
tags:
- Superheroes
- Comics
- Characters
- Marvel
- DC Comics
- Entertainment
- Open Data
---
