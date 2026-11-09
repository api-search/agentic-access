---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 1
api_specs:
- filename: openapi.json
  format: json
  label: Angels for Agents Discovery API
  slug: angels-for-agents-discovery-api
  spec_type: OpenAPI
  url: https://angelsforagents.com/openapi.json
consequence_counts:
  physical: 1
  read: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Angelsforagents Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /a2a/v1/message:send
operation_count: 2
overview: 'Angels for Agents exposes 2 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Angels for Agents
provider_slug: angelsforagents-com
slug: angelsforagents-com-agentic-access
source_filename: angelsforagents-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/angelsforagents-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 2\n  by_action_class:\n    acting: 1\n    connected: 1\n  by_consequence:\n    physical: 1\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /a2a/v1/message:send\n  method: post\n  operationId: sendA2AMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/opportunities\n  method: get\n  operationId:\
  \ listOpportunities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/angelsforagents-com/agentic-access/angelsforagents-com-agentic-access.yml
summary_line: 2 operations · 1 acting
tags:
- Capital
- Artificial Intelligence
- Agents
- Venture Funding
- Networks
---
