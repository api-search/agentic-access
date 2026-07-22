---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 2
api_specs:
- filename: napkinai-openapi.yml
  format: yaml
  label: Napkin AI API
  slug: napkin-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/napkinai/refs/heads/main/openapi/napkinai-openapi.yml
consequence_counts:
  read: 2
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Napkinai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 3
overview: 'Napkin.AI exposes 3 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Napkin.AI
provider_slug: napkinai
slug: napkinai-agentic-access
source_filename: napkinai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/napkinai-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 3\n  by_action_class:\n    acting: 1\n    connected: 2\n  by_consequence:\n    write: 1\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /visual\n  method: post\n  operationId: createVisualRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /visual/{request-id}/status\n  method: get\n  operationId: getVisualRequestStatus\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /visual/{request-id}/file/{file-id}\n  method: get\n  operationId: downloadVisualFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/napkinai/refs/heads/main/agentic-access/napkinai-agentic-access.yml
summary_line: 3 operations · 1 acting
tags:
- Company
- Ai
- Visualization
- Diagrams
- Charts
- Infographics
- Presentations
- Content Generation
- Design
- Developer API
---
