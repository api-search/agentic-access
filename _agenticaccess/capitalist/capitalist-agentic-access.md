---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 4
api_specs:
- filename: capitalist-capitalist-payments-api-api-openapi.yml
  format: yaml
  label: Capitalist Payments API (v1, deprecated)
  slug: capitalist-capitalist-payments-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capitalist/refs/heads/main/openapi/capitalist-capitalist-payments-api-api-openapi.yml
- filename: capitalist-account-api-openapi.yml
  format: yaml
  label: Capitalist Account API
  slug: capitalist-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capitalist/refs/heads/main/openapi/capitalist-account-api-openapi.yml
- filename: capitalist-exchange-api-openapi.yml
  format: yaml
  label: Capitalist Exchange API
  slug: capitalist-exchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capitalist/refs/heads/main/openapi/capitalist-exchange-api-openapi.yml
- filename: capitalist-payment-api-openapi.yml
  format: yaml
  label: Capitalist Payment API
  slug: capitalist-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capitalist/refs/heads/main/openapi/capitalist-payment-api-openapi.yml
- filename: capitalist-rate-api-openapi.yml
  format: yaml
  label: Capitalist Rate API
  slug: capitalist-rate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capitalist/refs/heads/main/openapi/capitalist-rate-api-openapi.yml
consequence_counts:
  physical: 2
  read: 4
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Capitalist Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payment
operation_count: 7
overview: 'Capitalist exposes 7 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read, 1 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Capitalist
provider_slug: capitalist
slug: capitalist-agentic-access
source_filename: capitalist-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: generated\nsource: openapi/capitalist-account-api-openapi.yml, openapi/capitalist-capitalist-payments-api-api-openapi.yml,\n  openapi/capitalist-exchange-api-openapi.yml, openapi/capitalist-payment-api-openapi.yml, openapi/capitalist-rate-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 4\n    acting: 3\n  by_consequence:\n    read: 4\n    physical: 2\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/account/list\n  method: get\n  operationId: getV1AccountList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: post\n  operationId:\
  \ postRoot\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/exchange\n  method: post\n  operationId: postV1Exchange\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/payment\n  method: post\n  operationId: postV1Payment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/payment/document/{documentId}\n  method: get\n  operationId: getV1PaymentDocumentByDocumentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/payment/{userRequestId}\n  method: get\n  operationId: getV1PaymentByUserRequestId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/rate\n  method: get\n  operationId: getV1Rate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capitalist/refs/heads/main/agentic-access/capitalist-agentic-access.yml
summary_line: 7 operations · 3 acting
tags:
- Bulk Payouts
- Cryptocurrency
- Finance
- Mass Payments
- Payment Platform
- Payments
- Payouts
- Remittances
---
