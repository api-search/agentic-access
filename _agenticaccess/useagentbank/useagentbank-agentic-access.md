---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 2
api_specs:
- filename: useagentbank-payouts-api-openapi.yml
  format: yaml
  label: AgentBank Payouts API
  slug: useagentbank-payouts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/useagentbank/openapi/useagentbank-payouts-api-openapi.yml
consequence_counts:
  physical: 1
  read: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Useagentbank Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/public/x402/payout
operation_count: 3
overview: 'AgentBank exposes 3 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AgentBank
provider_slug: useagentbank
slug: useagentbank-agentic-access
source_filename: useagentbank-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: generated\nsource: openapi/useagentbank-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 3\n  by_action_class:\n    acting: 1\n    connected: 2\n  by_consequence:\n    physical: 1\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/public/x402/payout\n  method: post\n  operationId: createPublicX402Payout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/public/x402/payments\n  method: get\n\
  \  operationId: listPublicX402Payouts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/public/x402/payments/{flowId}\n  method: get\n  operationId: getPublicX402Payout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/useagentbank/agentic-access/useagentbank-agentic-access.yml
summary_line: 3 operations · 1 acting
tags:
- Company
- Finance
- Artificial Intelligence
- Banking
- Cryptocurrency
- Payments
---
