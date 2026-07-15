---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 5
api_specs:
- filename: tillo-gift-card-openapi.yml
  format: yaml
  label: Tillo Gift Card API
  slug: tillo-gift-card-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tillo/refs/heads/main/openapi/tillo-gift-card-openapi.yml
- filename: tillo-gift-card-openapi.yml
  format: yaml
  label: Tillo Float Management API
  slug: tillo-float-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tillo/refs/heads/main/openapi/tillo-gift-card-openapi.yml
consequence_counts:
  physical: 4
  read: 5
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tillo Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /digital/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /digital/order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /digital/refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /float/request-payment-transfer
operation_count: 12
overview: 'Tillo exposes 12 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read, 3 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Tillo
provider_slug: tillo
slug: tillo-agentic-access
source_filename: tillo-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/tillo-gift-card-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 5\n    acting: 7\n  by_consequence:\n    read: 5\n    write: 3\n    physical: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /brands\n  method: get\n  operationId: listBrands\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /brands/{brand_identifier}\n  method: get\n  operationId: getBrand\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /digital/issue\n\
  \  method: post\n  operationId: issueDigitalCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /digital/order\n  method: post\n  operationId: orderDigitalCard\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /digital/check-balance\n  method: post\n  operationId: checkBalance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /digital/check-stock\n  method: post\n  operationId: checkStock\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /digital/cancel\n  method: post\n  operationId: cancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /digital/refund\n  method: post\n  operationId: refundOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /order-status\n  method: get\n  operationId: getOrderStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /float\n  method: get\n  operationId: getFloatBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /float/request-payment-transfer\n  method: post\n  operationId: requestPaymentTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /float/transfer-requests\n  method: get\n  operationId: listTransferRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tillo/refs/heads/main/agentic-access/tillo-agentic-access.yml
summary_line: 12 operations · 7 acting
tags:
- Finance
- Gift Cards
- Payments
- Rewards
- Incentives
---
