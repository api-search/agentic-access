---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 2
api_specs:
- filename: civic-pass-customer-api.yaml
  format: yaml
  label: Civic Pass API
  slug: civic-pass-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/civic/refs/heads/main/openapi/civic-pass-customer-api.yaml
consequence_counts:
  read: 2
  safety-critical: 1
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Civic Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /pass/{chain}/{chainNetwork}/{wallet}
operation_count: 7
overview: 'Civic exposes 7 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read, 4 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Civic
provider_slug: civic
slug: civic-agentic-access
source_filename: civic-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/civic-pass-customer-api.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    acting: 5\n    connected: 2\n  by_consequence:\n    write: 4\n    read: 2\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /pass\n  method: post\n  operationId: listPass\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - read:token\n    - write:token\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pass/{chain}/{chainNetwork}\n  method: post\n  operationId:\
  \ issuePass\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - read:token\n    - write:token\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pass/{chain}/{chainNetwork}/{wallet}\n  method: get\n  operationId: getPass\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:token\n    - write:token\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pass/{chain}/{chainNetwork}/{wallet}\n  method: patch\n  operationId: patchPass\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - read:token\n    - write:token\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    \
  \  - high-value\n    audit: required\n- path: /pass/{chain}/{chainNetwork}/{wallet}\n  method: delete\n  operationId: deletePass\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - read:token\n    - write:token\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /piirequest/{scopeRequestId}\n  method: get\n  operationId: getPii\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /piirequest/{scopeRequestId}/status\n  method: put\n  operationId: updatePiiReceipt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/civic/refs/heads/main/agentic-access/civic-agentic-access.yml
summary_line: 7 operations · 5 acting · 1 human-in-the-loop
tags:
- AI Agents
- Authentication
- Digital Identity
- Identity Verification
- KYC
- MCP
- OAuth
- Security
- Solana
- Web3
- Wallets
---
