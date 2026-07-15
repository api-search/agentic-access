---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 18
api_specs:
- filename: klarna-payments-api-openapi.yml
  format: yaml
  label: Klarna Payments API
  slug: klarna-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-payments-api-openapi.yml
- filename: klarna-customer-token-api-openapi.yml
  format: yaml
  label: Klarna Customer Token API
  slug: klarna-customer-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-customer-token-api-openapi.yml
- filename: klarna-settlements-api-openapi.yml
  format: yaml
  label: Klarna Settlements API
  slug: klarna-settlements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/openapi/klarna-settlements-api-openapi.yml
- filename: klarna-push-notifications-asyncapi.yml
  format: yaml
  label: Klarna Push Notifications
  slug: klarna-push-notifications
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/asyncapi/klarna-push-notifications-asyncapi.yml
consequence_counts:
  physical: 14
  read: 18
  safety-critical: 1
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Klarna Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /hpp/v1/sessions/{session_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /merchantcard/v3/orders/{order_id}/cancel-request
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ordermanagement/v1/orders/{order_id}/acknowledge
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /ordermanagement/v1/orders/{order_id}/authorization
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ordermanagement/v1/orders/{order_id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ordermanagement/v1/orders/{order_id}/captures
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /ordermanagement/v1/orders/{order_id}/captures/{capture_id}/extend-due-date
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ordermanagement/v1/orders/{order_id}/captures/{capture_id}/shipping-info
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ordermanagement/v1/orders/{order_id}/captures/{capture_id}/trigger-send-out
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /ordermanagement/v1/orders/{order_id}/customer-details
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ordermanagement/v1/orders/{order_id}/extend-authorization-time
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /ordermanagement/v1/orders/{order_id}/merchant-references
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ordermanagement/v1/orders/{order_id}/refunds
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ordermanagement/v1/orders/{order_id}/release-remaining-authorization
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ordermanagement/v1/orders/{order_id}/shipping-info
operation_count: 37
overview: 'Klarna exposes 37 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read, 4 write, 14 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Klarna
provider_slug: klarna
slug: klarna-agentic-access
source_filename: klarna-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/hosted-payment-page-api-openapi.yml, openapi/klarna-settlements-api-openapi.yml,\n  openapi/merchant-card-service-api-openapi.yml, openapi/order-management-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 37\n  by_action_class:\n    acting: 19\n    connected: 18\n  by_consequence:\n    write: 4\n    read: 18\n    safety-critical: 1\n    physical: 14\n  human_in_the_loop_required: 1\noperations:\n- path: /hpp/v1/sessions\n  method: post\n  operationId: createHppSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hpp/v1/sessions/{session_id}\n  method: get\n  operationId: getSessionById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hpp/v1/sessions/{session_id}\n  method: delete\n  operationId: disableHppSession\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /hpp/v1/sessions/{session_id}/distribution\n  method: post\n  operationId: distributeHppSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payouts/summary\n  method: get\n  operationId: getPayoutSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payouts/{payment_reference}\n  method: get\n  operationId: getPayout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payouts\n  method: get\n  operationId: getPayouts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/payout-with-transactions\n  method: get\n  operationId: getPayoutReportWithTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /reports/payout\n  method: get\n  operationId: payout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions\n  method: get\n  operationId: getTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/payouts-summary-with-transactions\n  method: get\n  operationId: getPayoutsSummaryReportWithTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/payouts-summary\n  method: get\n  operationId: payoutsSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchantcard/v3/promises\n  method: post\n  operationId: createPromise\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /merchantcard/v3/promises/{promise_id}\n  method: get\n  operationId: readPromise\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchantcard/v3/settlements\n  method: post\n  operationId: settlePromise\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /merchantcard/v3/settlements/{settlement_id}\n  method: get\n  operationId: readSettlement\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchantcard/v3/settlements/order/{order_id}\n  method: get\n  operationId: readSettlementByOrderId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchantcard/v3/orders/{order_id}/cancel-request\n  method: post\n  operationId: postcancelorder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /merchantcard/v3/orders/{order_id}/cancel-request\n  method: get\n  operationId: getcancelorder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /ordermanagement/v1/orders/{order_id}\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ordermanagement/v1/orders/{order_id}/acknowledge\n  method: post\n  operationId: acknowledgeOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ordermanagement/v1/orders/{order_id}/authorization\n  method: patch\n  operationId: updateAuthorization\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n  \
  \    purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ordermanagement/v1/orders/{order_id}/captures\n  method: post\n  operationId: captureOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ordermanagement/v1/orders/{order_id}/captures\n  method: get\n  operationId: getCaptures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ordermanagement/v1/orders/{order_id}/captures/{capture_id}\n  method: get\n  operationId: getCapture\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ordermanagement/v1/orders/{order_id}/captures/{capture_id}/extend-due-date\n  method: patch\n  operationId: extendDueDate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ordermanagement/v1/orders/{order_id}/captures/{capture_id}/extend-due-date-options\n  method: get\n  operationId: getOptionsForExtendDueDate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ordermanagement/v1/orders/{order_id}/captures/{capture_id}/shipping-info\n  method: post\n  operationId: appendShippingInfo\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ordermanagement/v1/orders/{order_id}/captures/{capture_id}/trigger-send-out\n  method: post\n  operationId: triggerSendOut\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ordermanagement/v1/orders/{order_id}/customer-details\n  method: patch\n  operationId: updateConsumerDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ordermanagement/v1/orders/{order_id}/extend-authorization-time\n  method: post\n  operationId: extendAuthorizationTime\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ordermanagement/v1/orders/{order_id}/merchant-references\n  method: patch\n  operationId: updateMerchantReferences\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ordermanagement/v1/orders/{order_id}/refunds\n  method: post\n  operationId: refundOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ordermanagement/v1/orders/{order_id}/refunds/{refund_id}\n  method: get\n  operationId: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ordermanagement/v1/orders/{order_id}/release-remaining-authorization\n  method: post\n  operationId: releaseRemainingAuthorization\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ordermanagement/v1/orders/{order_id}/shipping-info\n  method: post\n  operationId: appendOrderShippingInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ordermanagement/v1/orders/{order_id}/cancel\n  method: post\n  operationId: cancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n\
  \      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/klarna/refs/heads/main/agentic-access/klarna-agentic-access.yml
summary_line: 37 operations · 19 acting · 1 human-in-the-loop
tags:
- Fintech
- BNPL
- Payments
- Cards
- Shopping
---
