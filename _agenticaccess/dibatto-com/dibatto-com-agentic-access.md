---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 7
api_specs:
- filename: dibatto-com-episodes-api-openapi.yml
  format: yaml
  label: Dibatto Episodes API
  slug: dibatto-com-episodes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dibatto-com/openapi/dibatto-com-episodes-api-openapi.yml
- filename: dibatto-com-shows-api-openapi.yml
  format: yaml
  label: Dibatto Shows API
  slug: dibatto-com-shows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dibatto-com/openapi/dibatto-com-shows-api-openapi.yml
consequence_counts:
  read: 7
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Dibatto Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Dibatto exposes 9 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Dibatto
provider_slug: dibatto-com
slug: dibatto-com-agentic-access
source_filename: dibatto-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/dibatto-com-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 7\n    acting: 2\n  by_consequence:\n    read: 7\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /shows\n  method: get\n  operationId: listShows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shows/{id}\n  method: get\n  operationId: getShow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shows/{id}/rundown\n  method: get\n  operationId: getRundown\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shows/{id}/rundown\n  method: post\n  operationId: prepareRundown\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /episodes\n  method: get\n  operationId: listEpisodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /episodes\n  method: post\n  operationId: prepareEpisode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /episodes/{id}\n  method: get\n  operationId: getEpisode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /episodes/{id}/transcript\n  method: get\n  operationId: getTranscript\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /episodes/{id}/wrap\n  method: get\n  operationId: getWrapStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/dibatto-com/agentic-access/dibatto-com-agentic-access.yml
summary_line: 9 operations · 2 acting
tags:
- Company
- Podcasts
- Artificial Intelligence
- Voice
- Audio
- Content Creation
- MCP
---
