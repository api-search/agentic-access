---
acting_count: 3
action_class_counts:
  acting: 3
api_specs:
- filename: confrere-video-openapi.yml
  format: yaml
  label: Confrere Video API
  slug: confrere-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confrere/refs/heads/main/openapi/confrere-video-openapi.yml
consequence_counts:
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Confrere Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 3
overview: 'Confrere exposes 3 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Confrere
provider_slug: confrere
slug: confrere-agentic-access
source_filename: confrere-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/confrere-video-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 3\n  by_action_class:\n    acting: 3\n  by_consequence:\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /api/token\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/room/{id}/invalidate\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/room/{id}/{userId}/invalidate\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/confrere/refs/heads/main/agentic-access/confrere-agentic-access.yml
summary_line: 3 operations · 3 acting
tags:
- Company
- Video
- Video Conferencing
- Communications
- Healthcare
- Telehealth
- Embeddable
- WebRTC
---
