---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 5
api_specs:
- filename: mpesa-openapi.yml
  format: yaml
  label: M-Pesa Authorization API
  slug: mpesa-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-openapi.yml
- filename: mpesa-openapi.yml
  format: yaml
  label: M-Pesa Express (STK Push) API
  slug: mpesa-express-stk-push-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-openapi.yml
- filename: mpesa-openapi.yml
  format: yaml
  label: M-Pesa Customer To Business (C2B) API
  slug: mpesa-c2b-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-openapi.yml
- filename: mpesa-openapi.yml
  format: yaml
  label: M-Pesa Business To Customer (B2C) API
  slug: mpesa-b2c-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-openapi.yml
- filename: mpesa-openapi.yml
  format: yaml
  label: M-Pesa Business To Business (B2B) API
  slug: mpesa-b2b-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-openapi.yml
- filename: mpesa-openapi.yml
  format: yaml
  label: M-Pesa B2B Express Checkout (USSD Push) API
  slug: mpesa-b2b-express-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-openapi.yml
- filename: mpesa-openapi.yml
  format: yaml
  label: M-Pesa Transaction Status API
  slug: mpesa-transaction-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-openapi.yml
- filename: mpesa-openapi.yml
  format: yaml
  label: M-Pesa Account Balance API
  slug: mpesa-account-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-openapi.yml
- filename: mpesa-openapi.yml
  format: yaml
  label: M-Pesa Reversal API
  slug: mpesa-reversal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-openapi.yml
- filename: mpesa-openapi.yml
  format: yaml
  label: M-Pesa Dynamic QR Code API
  slug: mpesa-dynamic-qr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-openapi.yml
- filename: mpesa-openapi.yml
  format: yaml
  label: M-Pesa Tax Remittance API
  slug: mpesa-tax-remittance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-openapi.yml
- filename: mpesa-openapi.yml
  format: yaml
  label: M-Pesa Bill Manager API
  slug: mpesa-bill-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-openapi.yml
- filename: mpesa-openapi.yml
  format: yaml
  label: M-Pesa Ratiba (Standing Order) API
  slug: mpesa-ratiba-standing-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-openapi.yml
consequence_counts:
  read: 5
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. Funds-movement operations (B2C, B2B, Reversal, Tax Remittance) move real money in KES and are marked human-in-the-loop required. See research/curity/agentic-governance/.
human_in_the_loop: 4
kind: agentic-access
layout: agentic-access
method: generated
name: Mpesa Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'M-Pesa (Safaricom Daraja) exposes 14 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 9 write.


  4 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: M-Pesa (Safaricom Daraja)
provider_slug: mpesa
slug: mpesa-agentic-access
source_filename: mpesa-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: generated\nsource: openapi/mpesa-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. Funds-movement operations (B2C, B2B, Reversal, Tax Remittance) move\n  real money in KES and are marked human-in-the-loop required. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    acting: 9\n    connected: 5\n  by_consequence:\n    write: 9\n    read: 5\n  human_in_the_loop_required: 4\noperations:\n- path: /oauth/v1/generate\n  method: get\n  operationId: generateAccessToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3599\n    audit: none\n- path: /mpesa/stkpush/v1/processrequest\n  method: post\n  operationId: stkPush\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mpesa/stkpushquery/v1/query\n  method: post\n  operationId: stkPushQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 900\n    audit: none\n- path: /mpesa/c2b/v1/registerurl\n  method: post\n  operationId: c2bRegisterURL\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    audit: required\n- path: /mpesa/c2b/v1/simulate\n  method: post\n  operationId: c2bSimulate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n  \
  \  token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    audit: required\n- path: /mpesa/b2c/v3/paymentrequest\n  method: post\n  operationId: b2cPaymentRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - funds-movement\n      - high-value\n    audit: required\n- path: /mpesa/b2b/v1/paymentrequest\n  method: post\n  operationId: b2bPaymentRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - funds-movement\n      - high-value\n    audit: required\n- path: /v1/ussdpush/get-msisdn\n  method: post\n  operationId: b2bExpressCheckout\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mpesa/transactionstatus/v1/query\n  method: post\n  operationId: transactionStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 900\n    audit: none\n- path: /mpesa/accountbalance/v1/query\n  method: post\n  operationId: accountBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 900\n    audit: none\n- path: /mpesa/reversal/v1/request\n  method: post\n  operationId: reversal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n    escalation:\n      human-in-the-loop: required\n      triggers:\n\
  \      - funds-movement\n      - high-value\n    audit: required\n- path: /mpesa/qrcode/v1/generate\n  method: post\n  operationId: dynamicQR\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    audit: required\n- path: /mpesa/b2b/v1/remittax\n  method: post\n  operationId: taxRemittance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - funds-movement\n      - high-value\n    audit: required\n- path: /standingorder/v1/createStandingOrderExternal\n  method: post\n  operationId: createStandingOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/agentic-access/mpesa-agentic-access.yml
summary_line: 14 operations · 9 acting · 4 human-in-the-loop
tags:
- Mobile Money
- Payments
- Fintech
- Kenya
- Africa
- M-Pesa
---
