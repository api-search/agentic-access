---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 4
api_specs:
- filename: meld-headless-api-openapi.yml
  format: yaml
  label: Meld.io Headless API
  slug: meld-headless-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meld/openapi/meld-headless-api-openapi.yml
- filename: meld-retail-ramp-api-openapi.yml
  format: yaml
  label: Meld.io Retail Ramp API
  slug: meld-retail-ramp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meld/openapi/meld-retail-ramp-api-openapi.yml
consequence_counts:
  physical: 4
  read: 4
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Meld Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /crypto/order/headless/offramp
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /crypto/order/headless/onramp
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/crypto/quote
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/virtual-account/deposit-instructions
operation_count: 9
overview: 'Meld.io exposes 9 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read, 1 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Meld.io
provider_slug: meld
slug: meld-agentic-access
source_filename: meld-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: generated\nsource: openapi/crypto-20260203.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    acting: 5\n    connected: 4\n  by_consequence:\n    physical: 4\n    write: 1\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /payments/crypto/quote\n  method: post\n  operationId: /crypto-quote-get\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /crypto/session/widget\n  method: post\n\
  \  operationId: /crypto-session-widget-create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/transactions/{id}\n  method: get\n  operationId: /payments-transactions-get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/transactions\n  method: get\n  operationId: /payments-transactions-search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/transactions/sessions/{sessionId}\n  method: get\n  operationId: /payments-transactions-sessions-get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crypto/order/headless/offramp\n  method: post\n  operationId: /crypto-order-headless-offramp-create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/virtual-account/deposit-instructions\n  method: post\n  operationId: /payments-virtual-account-deposit-instructions-create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /crypto/order/headless/onramp\n\
  \  method: post\n  operationId: /crypto-order-headless-onramp-create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /crypto/onramp/{serviceProvider}/requirements\n  method: get\n  operationId: /crypto-onramp-verification-requirements-get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/meld/agentic-access/meld-agentic-access.yml
summary_line: 9 operations · 5 acting
tags:
- Data Integration
- Fintech
- API Platform
- Stablecoins
- Digital Assets
- Enterprise
---
