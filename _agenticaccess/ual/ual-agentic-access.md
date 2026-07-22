---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 2
api_specs:
- filename: ual-bis-cobros-online-v2-openapi.yml
  format: yaml
  label: Ualá Bis API Cobros Online v2
  slug: ualá-bis-api-cobros-online-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ual/refs/heads/main/openapi/ual-bis-cobros-online-v2-openapi.yml
- filename: ual-bis-auth-v2-openapi.yml
  format: yaml
  label: Ualá Bis Authentication API v2
  slug: ualá-bis-authentication-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ual/refs/heads/main/openapi/ual-bis-auth-v2-openapi.yml
consequence_counts:
  physical: 2
  read: 2
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ual Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/{uuid}/refund
operation_count: 5
overview: 'Ualá exposes 5 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read, 1 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Ualá
provider_slug: ual
slug: ual-agentic-access
source_filename: ual-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/ual-bis-auth-v2-openapi.yml, openapi/ual-bis-cobros-online-v2-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    acting: 3\n    connected: 2\n  by_consequence:\n    write: 1\n    physical: 2\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /auth/token\n  method: post\n  operationId: createToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /checkout\n  method: post\n  operationId: createOrder\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{uuid}\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders\n  method: get\n  operationId: listOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{uuid}/refund\n  method: post\n  operationId: refundOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n     \
  \ purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ual/refs/heads/main/agentic-access/ual-agentic-access.yml
summary_line: 5 operations · 3 acting
tags:
- Company
- Fintech
- Payments
- Banking
- Neobank
- Checkout
- Ecommerce
- Argentina
- Mexico
---
