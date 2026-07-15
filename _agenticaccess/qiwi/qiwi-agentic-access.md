---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 9
api_specs:
- filename: qiwi-openapi.yml
  format: yaml
  label: Qiwi Payment Protocol
  slug: qiwi-payment-protocol
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qiwi/refs/heads/main/openapi/qiwi-openapi.yml
consequence_counts:
  physical: 9
  read: 9
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Qiwi Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /partner/payin/v1/sites/{siteId}/bills/{billId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /partner/payin/v1/sites/{siteId}/payments/sbp-token
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /partner/payin/v1/sites/{siteId}/payments/{paymentId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /partner/payin/v1/sites/{siteId}/payments/{paymentId}/captures/{captureId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /partner/payin/v1/sites/{siteId}/payments/{paymentId}/complete
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /partner/payin/v1/sites/{siteId}/refunds/{refundId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /partner/payin/v1/sites/{siteId}/refunds/{refundId}/decline
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /partner/payout/v1/sites/{siteId}/payouts/{payoutId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /partner/payout/v1/sites/{siteId}/payouts/{payoutId}/complete
operation_count: 21
overview: 'Qiwi exposes 21 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 3 write, and 9 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Qiwi
provider_slug: qiwi
slug: qiwi-agentic-access
source_filename: qiwi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/qiwi-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    acting: 12\n    connected: 9\n  by_consequence:\n    physical: 9\n    read: 9\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /partner/payin/v1/sites/{siteId}/bills/{billId}\n  method: put\n  operationId: createInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partner/payin/v1/sites/{siteId}/bills/{billId}\n\
  \  method: get\n  operationId: getInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /partner/payin/v1/sites/{siteId}/bills/{billId}/payments\n  method: get\n  operationId: listInvoicePayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /partner/payin/v1/sites/{siteId}/payments/{paymentId}\n  method: put\n  operationId: createPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partner/payin/v1/sites/{siteId}/payments/{paymentId}\n  method: get\n  operationId: getPayment\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /partner/payin/v1/sites/{siteId}/payments/{paymentId}/complete\n  method: post\n  operationId: completePayment3DS\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partner/payin/v1/sites/{siteId}/payments/{paymentId}/captures/{captureId}\n  method: put\n  operationId: capturePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /partner/payin/v1/sites/{siteId}/payments/{paymentId}/captures/{captureId}\n  method: get\n  operationId: getCapture\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /partner/payin/v1/sites/{siteId}/refunds/{refundId}\n  method: put\n  operationId: createRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partner/payin/v1/sites/{siteId}/refunds/{refundId}\n  method: get\n  operationId: getRefund\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /partner/payin/v1/sites/{siteId}/refunds\n  method: get\n  operationId: listRefunds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /partner/payin/v1/sites/{siteId}/refunds/{refundId}/decline\n  method: post\n  operationId: declineRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partner/payin/v1/sites/{siteId}/qr\n  method: post\n  operationId: createQrCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n     \
  \ - abnormal\n      - high-value\n    audit: required\n- path: /partner/payin/v1/sites/{siteId}/qr/{qrCodeUid}\n  method: get\n  operationId: getQrCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /partner/payin/v1/sites/{siteId}/payments/sbp-token\n  method: put\n  operationId: paySbpToken\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partner/payin/v1/sites/{siteId}/check-card\n  method: post\n  operationId: checkCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partner/payin/v1/sites/{siteId}/check-card/{checkId}\n  method: get\n  operationId: getCardCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /partner/payin/v1/sites/{siteId}/check-card/{checkId}/complete\n  method: post\n  operationId: completeCardCheck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partner/payout/v1/sites/{siteId}/payouts/{payoutId}\n  method: put\n  operationId: createPayout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n \
  \     exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partner/payout/v1/sites/{siteId}/payouts/{payoutId}\n  method: get\n  operationId: getPayout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /partner/payout/v1/sites/{siteId}/payouts/{payoutId}/complete\n  method: post\n  operationId: completePayout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qiwi/refs/heads/main/agentic-access/qiwi-agentic-access.yml
summary_line: 21 operations · 12 acting
tags:
- Payments
- Wallet
- Payouts
- Fintech
- Banking
---
