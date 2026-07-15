---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 3
api_specs:
- filename: state-farm-insurance-renters-openapi.yml
  format: yaml
  label: Renters Insurance API
  slug: renters-insurance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/state-farm-insurance/refs/heads/main/openapi/state-farm-insurance-renters-openapi.yml
consequence_counts:
  read: 3
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: State Farm Insurance Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'State Farm Insurance exposes 5 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: State Farm Insurance
provider_slug: state-farm-insurance
slug: state-farm-insurance-agentic-access
source_filename: state-farm-insurance-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/state-farm-insurance-renters-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    acting: 2\n    connected: 3\n  by_consequence:\n    write: 2\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /renters/quotes\n  method: post\n  operationId: createRentersQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - renters:policy:read\n    - renters:policy:write\n    - renters:quote\n- path: /renters/quotes/{quoteId}\n\
  \  method: get\n  operationId: getRentersQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - renters:policy:read\n    - renters:policy:write\n    - renters:quote\n- path: /renters/policies\n  method: post\n  operationId: createRentersPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - renters:policy:read\n    - renters:policy:write\n    - renters:quote\n- path: /renters/policies/{policyNumber}\n  method: get\n  operationId: getRentersPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - renters:policy:read\n\
  \    - renters:policy:write\n    - renters:quote\n- path: /renters/coverage-options\n  method: get\n  operationId: listCoverageOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - renters:policy:read\n    - renters:policy:write\n    - renters:quote\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/state-farm-insurance/refs/heads/main/agentic-access/state-farm-insurance-agentic-access.yml
summary_line: 5 operations · 2 acting
tags:
- Fortune 100
---
