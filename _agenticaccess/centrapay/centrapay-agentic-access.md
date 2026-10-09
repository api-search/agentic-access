---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 8
api_specs:
- filename: centrapay-payment-requests-api-openapi.yml
  format: yaml
  label: Centrapay Payment Requests API
  slug: centrapay-payment-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centrapay/refs/heads/main/openapi/centrapay-payment-requests-api-openapi.yml
consequence_counts:
  physical: 8
  read: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Centrapay Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/payment-requests
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/payment-requests/{paymentRequestId}/conditions/{conditionId}/accept
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/payment-requests/{paymentRequestId}/conditions/{conditionId}/decline
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/payment-requests/{paymentRequestId}/confirm
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/payment-requests/{paymentRequestId}/pay
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/payment-requests/{paymentRequestId}/refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/payment-requests/{paymentRequestId}/release
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/payment-requests/{paymentRequestId}/void
operation_count: 16
overview: 'Centrapay exposes 16 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 8 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Centrapay
provider_slug: centrapay
slug: centrapay-agentic-access
source_filename: centrapay-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: generated\nsource: openapi/centrapay-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    acting: 8\n    connected: 8\n  by_consequence:\n    physical: 8\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /api/payment-requests\n  method: post\n  operationId: createPaymentRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/payment-requests/{paymentRequestId}\n  method:\
  \ get\n  operationId: getPaymentRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/payment-requests/short-code/{shortCode}\n  method: get\n  operationId: getPaymentRequestByShortCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/me/patron-code-payment-request\n  method: get\n  operationId: getPaymentRequestByPatronCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/connections/{connectionId}/latest-payment-request\n  method: get\n  operationId: getPaymentRequestByConnectionId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/payment-requests/external-ref/{externalRef}\n\
  \  method: get\n  operationId: listPaymentRequestsByExternalRef\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/payment-requests/{paymentRequestId}/summary\n  method: get\n  operationId: getPaymentRequestSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/payment-requests/{paymentRequestId}/pay\n  method: post\n  operationId: payPaymentRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/payment-requests/{paymentRequestId}/refund\n  method: post\n  operationId: refundPaymentRequest\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/payment-requests/{paymentRequestId}/void\n  method: post\n  operationId: voidPaymentRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/payment-requests/{paymentRequestId}/release\n  method: post\n  operationId: releasePaymentRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/payment-requests/{paymentRequestId}/confirm\n  method: post\n  operationId: confirmPaymentRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/payment-activities\n  method: get\n  operationId: listPaymentActivities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/payment-requests/{paymentRequestId}/activities\n  method: get\n  operationId: listPaymentRequestActivities\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/payment-requests/{paymentRequestId}/conditions/{conditionId}/accept\n  method: post\n  operationId: acceptPaymentCondition\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/payment-requests/{paymentRequestId}/conditions/{conditionId}/decline\n  method: post\n  operationId: declinePaymentCondition\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/centrapay/refs/heads/main/agentic-access/centrapay-agentic-access.yml
summary_line: 16 operations · 8 acting
tags:
- Company
- Payments
- Digital Wallets
- Open Banking
- QR Code Payments
- Loyalty
- Gift Cards
- Fintech
---
