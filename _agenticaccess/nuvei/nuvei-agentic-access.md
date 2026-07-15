---
acting_count: 23
action_class_counts:
  acting: 23
api_specs:
- filename: nuvei-payments-api-openapi.yml
  format: yaml
  label: Nuvei Payments API
  slug: nuvei-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuvei/refs/heads/main/openapi/nuvei-payments-api-openapi.yml
- filename: nuvei-session-api-openapi.yml
  format: yaml
  label: Nuvei Session API
  slug: nuvei-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuvei/refs/heads/main/openapi/nuvei-session-api-openapi.yml
- filename: nuvei-order-api-openapi.yml
  format: yaml
  label: Nuvei Order API
  slug: nuvei-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuvei/refs/heads/main/openapi/nuvei-order-api-openapi.yml
- filename: nuvei-payouts-api-openapi.yml
  format: yaml
  label: Nuvei Payouts API
  slug: nuvei-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuvei/refs/heads/main/openapi/nuvei-payouts-api-openapi.yml
- filename: nuvei-user-payment-options-api-openapi.yml
  format: yaml
  label: Nuvei User Payment Options API
  slug: nuvei-user-payment-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuvei/refs/heads/main/openapi/nuvei-user-payment-options-api-openapi.yml
- filename: nuvei-merchant-config-api-openapi.yml
  format: yaml
  label: Nuvei Merchant Configuration API
  slug: nuvei-merchant-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuvei/refs/heads/main/openapi/nuvei-merchant-config-api-openapi.yml
- filename: nuvei-3ds-api-openapi.yml
  format: yaml
  label: Nuvei 3DS API
  slug: nuvei-3ds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuvei/refs/heads/main/openapi/nuvei-3ds-api-openapi.yml
- filename: nuvei-dcc-api-openapi.yml
  format: yaml
  label: Nuvei DCC API
  slug: nuvei-dcc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuvei/refs/heads/main/openapi/nuvei-dcc-api-openapi.yml
- filename: nuvei-dmn-asyncapi.yml
  format: yaml
  label: Nuvei Direct Merchant Notifications (DMN)
  slug: nuvei-webhooks-dmn
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuvei/refs/heads/main/asyncapi/nuvei-dmn-asyncapi.yml
consequence_counts:
  physical: 15
  safety-critical: 1
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Nuvei Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /disableUPO.do
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accountCapture.do
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /addUPOAPM.do
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /addUPOCreditCard.do
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /deleteUPO.do
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /editUPOAPM.do
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /editUPOCreditCard.do
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /enableUPO.do
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /getMerchantPaymentMethods.do
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /getPaymentStatus.do
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /getUserUPOs.do
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /openOrder.do
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment.do
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payout.do
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /refundTransaction.do
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /updateOrder.do
operation_count: 23
overview: 'Nuvei exposes 23 API operations that an AI agent could call, of which 23 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 write, 15 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Nuvei
provider_slug: nuvei
slug: nuvei-agentic-access
source_filename: nuvei-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/nuvei-3ds-api-openapi.yml, openapi/nuvei-dcc-api-openapi.yml, openapi/nuvei-merchant-config-api-openapi.yml,\n  openapi/nuvei-order-api-openapi.yml, openapi/nuvei-payments-api-openapi.yml, openapi/nuvei-payouts-api-openapi.yml,\n  openapi/nuvei-session-api-openapi.yml, openapi/nuvei-user-payment-options-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    acting: 23\n  by_consequence:\n    write: 7\n    physical: 15\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /getCard3DDetails.do\n  method: post\n  operationId: getCard3DDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /authenticate3d.do\n  method: post\n  operationId: authenticate3d\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getDccDetails.do\n  method: post\n  operationId: getDccDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getMerchantCountries.do\n  method: post\n  operationId: getMerchantCountries\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getMerchantPaymentMethods.do\n  method: post\n  operationId: getMerchantPaymentMethods\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openOrder.do\n  method: post\n  operationId: openOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /updateOrder.do\n  method: post\n  operationId: updateOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment.do\n  method: post\n  operationId: createPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settleTransaction.do\n  method: post\n  operationId: settleTransaction\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /voidTransaction.do\n  method: post\n  operationId: voidTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /refundTransaction.do\n  method: post\n  operationId: refundTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /getPaymentStatus.do\n  method: post\n  operationId: getPaymentStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payout.do\n  method: post\n  operationId: payout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accountCapture.do\n  method: post\n  operationId: accountCapture\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getSessionToken.do\n  method: post\n  operationId: getSessionToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /addUPOCreditCard.do\n  method: post\n  operationId: addUPOCreditCard\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /addUPOAPM.do\n  method:\
  \ post\n  operationId: addUPOAPM\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /editUPOCreditCard.do\n  method: post\n  operationId: editUPOCreditCard\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /editUPOAPM.do\n  method: post\n  operationId: editUPOAPM\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n    \
  \  exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deleteUPO.do\n  method: post\n  operationId: deleteUPO\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getUserUPOs.do\n  method: post\n  operationId: getUserUPOs\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /enableUPO.do\n\
  \  method: post\n  operationId: enableUPO\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /disableUPO.do\n  method: post\n  operationId: disableUPO\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nuvei/refs/heads/main/agentic-access/nuvei-agentic-access.yml
summary_line: 23 operations · 23 acting · 1 human-in-the-loop
tags:
- Payments
- Payment Processing
- Payment Gateway
- Acquiring
- Payouts
- Alternative Payment Methods
- Fraud
- Risk
- Currency Conversion
- iGaming
- eCommerce
- FinTech
---
