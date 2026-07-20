---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 4
api_specs:
- filename: capchase-pay-openapi.yml
  format: yaml
  label: Capchase Pay API
  slug: capchase-pay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capchase/refs/heads/main/openapi/capchase-pay-openapi.yml
consequence_counts:
  read: 4
  safety-critical: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 5
kind: agentic-access
layout: agentic-access
method: generated
name: Capchase Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /pay/buyers
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /pay/buyers/{id}/renew-qualification
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /pay/buyers/{id}/update-external-id
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /pay/subscriptions
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /pay/subscriptions/{key}
operation_count: 9
overview: 'Capchase exposes 9 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 5 safety-critical.


  5 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Capchase
provider_slug: capchase
slug: capchase-agentic-access
source_filename: capchase-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/capchase-pay-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    acting: 5\n    connected: 4\n  by_consequence:\n    safety-critical: 5\n    read: 4\n  human_in_the_loop_required: 5\noperations:\n- path: /pay/buyers\n  method: post\n  operationId: PayExternalController_createBuyer\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /pay/subscriptions\n  method: post\n  operationId:\
  \ PayExternalController_createSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /pay/subscriptions\n  method: get\n  operationId: PayExternalController_listSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pay/subscriptions/{key}\n  method: delete\n  operationId: PayExternalController_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit:\
  \ required\n- path: /pay/buyers/{id}\n  method: get\n  operationId: PayExternalController_getBuyer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pay/subscriptions/{key}/instalment/{instalmentKey}/receipt\n  method: get\n  operationId: PayExternalController_getInstalmentReceipt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pay/subscriptions/{id}\n  method: get\n  operationId: PayExternalController_getSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pay/buyers/{id}/update-external-id\n  method: patch\n  operationId: PayExternalController_updateBuyerExternalId\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /pay/buyers/{id}/renew-qualification\n  method: post\n  operationId: PayExternalController_updateBuyerQualification\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capchase/refs/heads/main/agentic-access/capchase-agentic-access.yml
summary_line: 9 operations · 5 acting · 5 human-in-the-loop
tags:
- Company
- Fintech
- Payments
- Embedded Finance
- Financing
- B2B SaaS
- Revenue Financing
- BNPL
- KYB
- Underwriting
---
