---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 2
api_specs:
- filename: lacuna-lacuna-music-api-api-openapi.yml
  format: yaml
  label: Lacuna Music API Events
  slug: lacuna-lacuna-music-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lacuna/refs/heads/main/openapi/lacuna-lacuna-music-api-api-openapi.yml
- filename: lacuna-music-api-openapi.yml
  format: yaml
  label: Lacuna Music API
  slug: lacuna-music-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lacuna/refs/heads/main/openapi/lacuna-music-api-openapi.yml
- filename: lacuna-account-openapi.yml
  format: yaml
  label: Lacuna Account API
  slug: lacuna-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lacuna/refs/heads/main/openapi/lacuna-account-openapi.yml
consequence_counts:
  read: 2
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Lacuna Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 3
overview: 'Lacuna exposes 3 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Lacuna
provider_slug: lacuna
slug: lacuna-agentic-access
source_filename: lacuna-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-11'\nmethod: generated\nsource: openapi/_original/lacuna-music-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 3\n  by_action_class:\n    acting: 1\n    connected: 2\n  by_consequence:\n    write: 1\n    read: 2\n  human_in_the_loop_required: 0\n  note: >-\n    getMe added 2026-09-11 from the re-harvested spec. It is the safest operation on the API — free,\n    read-only, and the documented precondition check — and it is the one an agent should be permitted\n    before any grant that allows spending.\noperations:\n- path: /v1/music/generations\n  method: post\n  operationId: createGeneration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/music/generations/{id}\n  method: get\n  operationId: getGeneration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/me\n  method: get\n  operationId: getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    audience: null\n    token:\n      max-ttl: 3600\n    audit: none\n    cost: none\n    note: >-\n      Returns the calling credential's own plan, credit balance, scopes and key expiry. Safe to allow\n      broadly and worth allowing before `createGeneration` in any policy: it is the only way an agent\n      can establish that a spend will succeed without attempting one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lacuna/refs/heads/main/agentic-access/lacuna-agentic-access.yml
summary_line: 3 operations · 1 acting
tags:
- AI Music
- Music Generation
- AI Song Generator
- AI Lyrics Generator
- Audio
- MIDI
- Songwriting
- Generative AI
- MCP Server
- AgentSkill
- A2A
- Developer Tools
- Account
- OAuth
---
