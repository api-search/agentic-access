---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 1
api_specs:
- filename: paytabs-openapi.yml
  format: yaml
  label: PayTabs Hosted Payment Page API
  slug: paytabs-hosted-payment-page-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paytabs/refs/heads/main/openapi/paytabs-openapi.yml
- filename: paytabs-openapi.yml
  format: yaml
  label: PayTabs Managed Form API
  slug: paytabs-managed-form-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paytabs/refs/heads/main/openapi/paytabs-openapi.yml
- filename: paytabs-openapi.yml
  format: yaml
  label: PayTabs Own Form API
  slug: paytabs-own-form-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paytabs/refs/heads/main/openapi/paytabs-openapi.yml
- filename: paytabs-openapi.yml
  format: yaml
  label: PayTabs Transaction Management API
  slug: paytabs-transaction-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paytabs/refs/heads/main/openapi/paytabs-openapi.yml
- filename: paytabs-openapi.yml
  format: yaml
  label: PayTabs Token & Recurring Billing API
  slug: paytabs-token-recurring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paytabs/refs/heads/main/openapi/paytabs-openapi.yml
- filename: paytabs-openapi.yml
  format: yaml
  label: PayTabs Invoices API
  slug: paytabs-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paytabs/refs/heads/main/openapi/paytabs-openapi.yml
consequence_counts:
  read: 1
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents - review and bind audience per deployment. Payment operations move real money; write actions default to human-in-the-loop required. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Paytabs Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 2
overview: 'PayTabs exposes 2 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 1 write.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: PayTabs
provider_slug: paytabs
slug: paytabs-agentic-access
source_filename: paytabs-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: generated\nsource: openapi/paytabs-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents - review and bind\n  audience per deployment. Payment operations move real money; write actions default to\n  human-in-the-loop required. See research/curity/agentic-governance/.\nsummary:\n  operations: 2\n  by_action_class:\n    acting: 1\n    connected: 1\n  by_consequence:\n    write: 1\n    read: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /payment/request\n  method: post\n  operationId: createPaymentRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - always\n      - high-value\n      - abnormal\n    audit: required\n    notes: >-\n\
  \      Moves money - creates sales/authorizations and performs capture, void,\n      release and refund via tran_type. Treat as a high-consequence financial\n      write; require human approval and full audit. Refund/void especially\n      should never be fully autonomous.\n- path: /payment/query\n  method: post\n  operationId: queryTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 900\n    audit: required\n    notes: >-\n      Read-only transaction lookup, but returns cardholder/customer PII and\n      payment details; keep audit on and restrict audience.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paytabs/refs/heads/main/agentic-access/paytabs-agentic-access.yml
summary_line: 2 operations · 1 acting · 1 human-in-the-loop
tags:
- Payments
- Payment Gateway
- Fintech
- MENA
- Saudi Arabia
- Cards
- mada
---
