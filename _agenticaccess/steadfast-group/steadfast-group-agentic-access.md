---
acting_count: 0
action_class_counts:
  connected: 2
api_specs:
- filename: steadfast-group-address-api-openapi.yml
  format: yaml
  label: Steadfast Group Address API
  slug: steadfast-group-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/steadfast-group/refs/heads/main/openapi/steadfast-group-address-api-openapi.yml
- filename: steadfast-group-risk-api-openapi.yml
  format: yaml
  label: Steadfast Group Risk API
  slug: steadfast-group-risk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/steadfast-group/refs/heads/main/openapi/steadfast-group-risk-api-openapi.yml
consequence_counts:
  read: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Steadfast Group Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 2
overview: 'Steadfast Group exposes 2 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Steadfast Group
provider_slug: steadfast-group
slug: steadfast-group-agentic-access
source_filename: steadfast-group-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: generated\nsource: openapi/steadfast-group-flood-risk-tracker-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 2\n  by_action_class:\n    connected: 2\n  by_consequence:\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/risk/find_address\n  method: get\n  operationId: findAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/risk/get_flood_risk\n  method: get\n  operationId: getFloodRisk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/steadfast-group/refs/heads/main/agentic-access/steadfast-group-agentic-access.yml
summary_line: 2 operations
tags:
- Insurance
- Australia
- Brokers
- Insurance Broker Network
- General Insurance
- Property and Casualty
- Underwriting Agency
- Agency Management
- ACORD
- Partner Gated
- New Zealand
---
