---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 2
api_specs:
- filename: voxplo-ai-agent-api-openapi.yml
  format: yaml
  label: Voxplo Agent API
  slug: voxplo-ai-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/voxplo-ai/openapi/voxplo-ai-agent-api-openapi.yml
consequence_counts:
  read: 2
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Voxplo Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 3
overview: 'Voxplo exposes 3 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Voxplo
provider_slug: voxplo-ai
slug: voxplo-ai-agentic-access
source_filename: voxplo-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/voxplo-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 3\n  by_action_class:\n    acting: 1\n    connected: 2\n  by_consequence:\n    write: 1\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /agent/calls\n  method: post\n  operationId: placeCall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/calls\n  method: get\n  operationId: listCalls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent/calls/{id}\n  method: get\n  operationId: getCall\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/voxplo-ai/agentic-access/voxplo-ai-agentic-access.yml
summary_line: 3 operations · 1 acting
tags:
- Company
- Artificial Intelligence
- Voice
- MCP
---
