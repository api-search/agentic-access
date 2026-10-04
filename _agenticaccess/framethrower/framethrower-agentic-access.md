---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 10
api_specs:
- filename: framethrower-discovery-api-openapi.yml
  format: yaml
  label: FrameThrower Discovery API
  slug: framethrower-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/framethrower/refs/heads/main/openapi/framethrower-discovery-api-openapi.yml
- filename: framethrower-films-api-openapi.yml
  format: yaml
  label: FrameThrower Films API
  slug: framethrower-films-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/framethrower/refs/heads/main/openapi/framethrower-films-api-openapi.yml
- filename: framethrower-frames-api-openapi.yml
  format: yaml
  label: FrameThrower Frames API
  slug: framethrower-frames-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/framethrower/refs/heads/main/openapi/framethrower-frames-api-openapi.yml
- filename: framethrower-search-api-openapi.yml
  format: yaml
  label: FrameThrower Search API
  slug: framethrower-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/framethrower/refs/heads/main/openapi/framethrower-search-api-openapi.yml
consequence_counts:
  read: 10
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Framethrower Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'FrameThrower exposes 11 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: FrameThrower
provider_slug: framethrower
slug: framethrower-agentic-access
source_filename: framethrower-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: generated\nsource: openapi/framethrower-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 10\n    acting: 1\n  by_consequence:\n    read: 10\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /search\n  method: post\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/image\n  method: post\n  operationId: searchByImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/color\n  method: post\n  operationId:\
  \ searchByColor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /browse\n  method: post\n  operationId: browse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /similar\n  method: post\n  operationId: findSimilar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /frames\n  method: get\n  operationId: getFrame\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /frames/random\n  method: get\n  operationId: randomFrames\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /suggest\n  method: get\n  operationId: suggest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /films\n  method: get\n  operationId: listFilms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /films/{slug}\n  method: get\n  operationId: getFilm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /films/frames\n  method: get\n  operationId: listFilmFrames\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/framethrower/refs/heads/main/agentic-access/framethrower-agentic-access.yml
summary_line: 11 operations · 1 acting
tags:
- Film
- Cinematography
- Visual Reference
- Image Search
- Media
- Creative Tools
- MCP
- Agent-Native
---
