---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 1
api_specs:
- filename: telr-openapi.yml
  format: yaml
  label: Telr Hosted Payment Page API
  slug: telr-hosted-payment-page-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telr/refs/heads/main/openapi/telr-openapi.yml
- filename: telr-openapi.yml
  format: yaml
  label: Telr Remote API
  slug: telr-remote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telr/refs/heads/main/openapi/telr-openapi.yml
- filename: telr-openapi.yml
  format: yaml
  label: Telr Digital Wallets API
  slug: telr-digital-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telr/refs/heads/main/openapi/telr-openapi.yml
- filename: telr-openapi.yml
  format: yaml
  label: Telr Repeat Billing API
  slug: telr-repeat-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telr/refs/heads/main/openapi/telr-openapi.yml
- filename: telr-openapi.yml
  format: yaml
  label: Telr Payments REST API
  slug: telr-payments-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telr/refs/heads/main/openapi/telr-openapi.yml
- filename: telr-openapi.yml
  format: yaml
  label: Telr Mobile API and SDKs
  slug: telr-mobile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telr/refs/heads/main/openapi/telr-openapi.yml
consequence_counts:
  read: 1
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents - review and bind audience per deployment. Note - these operations move money (card/wallet charges, recurring agreements); default to human-in-the-loop for financial writes. See research/curity/agentic-access/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Telr Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Telr exposes 5 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 4 write.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Telr
provider_slug: telr
slug: telr-agentic-access
source_filename: telr-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: generated\nsource: openapi/telr-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents - review and bind\n  audience per deployment. Note - these operations move money (card/wallet charges, recurring\n  agreements); default to human-in-the-loop for financial writes. See research/curity/agentic-access/.\nsummary:\n  operations: 5\n  by_action_class:\n    acting: 4\n    connected: 1\n  by_consequence:\n    write: 4\n    read: 1\n  human_in_the_loop_required: 3\noperations:\n- path: /gateway/order.json\n  method: post\n  operationId: createHostedOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - high-value\n      - abnormal\n    audit: required\n\
  - path: /gateway/remote.json\n  method: post\n  operationId: createRemoteTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - money-movement\n      - card-data\n      - high-value\n    audit: required\n- path: /gateway/manageagreement.json\n  method: post\n  operationId: manageAgreement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - recurring-billing\n      - money-movement\n    audit: required\n- path: /api/v1/orders\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ required\n      triggers:\n      - money-movement\n      - high-value\n    audit: required\n- path: /api/v1/orders/{ref}\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telr/refs/heads/main/agentic-access/telr-agentic-access.yml
summary_line: 5 operations · 4 acting · 3 human-in-the-loop
tags:
- Payments
- Payment Gateway
- FinTech
- MENA
- UAE
---
