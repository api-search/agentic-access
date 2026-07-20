---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 2
api_specs:
- filename: fave-favepay-omni-openapi.yml
  format: yaml
  label: FavePay Omni (FPO) API
  slug: favepay-omni-fpo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fave/refs/heads/main/openapi/fave-favepay-omni-openapi.yml
consequence_counts:
  physical: 3
  read: 2
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Fave Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/fpo/v1/{country_code}/merchant_scan
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/fpo/v1/{country_code}/qr_codes
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/fpo/v1/{country_code}/transactions
operation_count: 6
overview: 'Fave exposes 6 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read, 1 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Fave
provider_slug: fave
slug: fave-agentic-access
source_filename: fave-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/fave-favepay-omni-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    acting: 4\n    connected: 2\n  by_consequence:\n    physical: 3\n    read: 2\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/fpo/v1/{country_code}/qr_codes\n  method: post\n  operationId: createQrCode\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/fpo/v1/{country_code}/merchant_scan\n\
  \  method: post\n  operationId: merchantScan\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/fpo/v1/{country_code}/transactions\n  method: get\n  operationId: getTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/fpo/v1/{country_code}/transactions\n  method: post\n  operationId: refundTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/fpo/v1/{country_code}/transactions/{id}\n  method: post\n  operationId: acknowledgeTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/fpo/v1/{country_code}/outlets/{outlet_id}/transactions\n  method: get\n  operationId: listOutletTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fave/refs/heads/main/agentic-access/fave-agentic-access.yml
summary_line: 6 operations · 4 acting
tags:
- Company
- Payments
- Fintech
- QR Payments
- Loyalty
- Cashback
- Merchant Services
- Southeast Asia
- Webhooks
---
