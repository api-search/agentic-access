---
acting_count: 0
action_class_counts:
  connected: 5
api_specs:
- filename: lrcmux-compatibility-api-openapi.yml
  format: yaml
  label: LRCMux Compatibility API
  slug: lrcmux-compatibility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lrcmux/openapi/lrcmux-compatibility-api-openapi.yml
- filename: lrcmux-lyrics-api-openapi.yml
  format: yaml
  label: LRCMux Lyrics API
  slug: lrcmux-lyrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lrcmux/openapi/lrcmux-lyrics-api-openapi.yml
- filename: lrcmux-meta-api-openapi.yml
  format: yaml
  label: LRCMux Meta API
  slug: lrcmux-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lrcmux/openapi/lrcmux-meta-api-openapi.yml
consequence_counts:
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Lrcmux Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'LRCMux exposes 5 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: LRCMux
provider_slug: lrcmux
slug: lrcmux-agentic-access
source_filename: lrcmux-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: generated\nsource: openapi/lrcmux-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 5\n  by_consequence:\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /compat/kpoe/v2/lyrics/get\n  method: get\n  operationId: kpoe-get-lyrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /compat/lrclib/api/get\n  method: get\n  operationId: lrclib-get-lyrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /compat/lrclib/api/search\n  method: get\n\
  \  operationId: lrclib-search-lyrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get\n  method: get\n  operationId: get-lyrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats\n  method: get\n  operationId: get-stats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/lrcmux/agentic-access/lrcmux-agentic-access.yml
summary_line: 5 operations
tags:
- Lyrics
- Music
- Free
- No Auth
---
