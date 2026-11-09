---
acting_count: 2
action_class_counts:
  acting: 2
api_specs:
- filename: qveris-agent-lifecycle-api-openapi.yml
  format: yaml
  label: QVeris Agent Lifecycle API
  slug: qveris-agent-lifecycle-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qveris/openapi/qveris-agent-lifecycle-api-openapi.yml
consequence_counts:
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Qveris Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 2
overview: 'QVeris exposes 2 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: QVeris
provider_slug: qveris
slug: qveris-agentic-access
source_filename: qveris-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/qveris-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 2\n  by_action_class:\n    acting: 2\n  by_consequence:\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /agent/anonymous-register\n  method: post\n  operationId: agent_anonymous_register_api_v1_agent_anonymous_register_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/claim\n  method: post\n  operationId: agent_claim_start_api_v1_agent_claim_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/qveris/agentic-access/qveris-agentic-access.yml
summary_line: 2 operations · 2 acting
tags:
- Artificial Intelligence
- Data
- Platform
- Developer Tools
- MCP
---
