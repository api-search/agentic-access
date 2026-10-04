---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 4
api_specs:
- filename: mpesa-account-balance-api-openapi.yml
  format: yaml
  label: M-Pesa (Safaricom Daraja) Account Balance API
  slug: mpesa-account-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-account-balance-api-openapi.yml
- filename: mpesa-authorization-api-openapi.yml
  format: yaml
  label: M-Pesa (Safaricom Daraja) Authorization API
  slug: mpesa-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-authorization-api-openapi.yml
- filename: mpesa-b2c-api-openapi.yml
  format: yaml
  label: M-Pesa (Safaricom Daraja) B2C API
  slug: mpesa-b2c-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-b2c-api-openapi.yml
- filename: mpesa-c2b-api-openapi.yml
  format: yaml
  label: M-Pesa (Safaricom Daraja) C2B API
  slug: mpesa-c2b-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-c2b-api-openapi.yml
- filename: mpesa-dynamic-qr-api-openapi.yml
  format: yaml
  label: M-Pesa (Safaricom Daraja) Dynamic QR API
  slug: mpesa-dynamic-qr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-dynamic-qr-api-openapi.yml
- filename: mpesa-m-pesa-express-api-openapi.yml
  format: yaml
  label: M-Pesa (Safaricom Daraja) M-Pesa Express API
  slug: mpesa-m-pesa-express-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-m-pesa-express-api-openapi.yml
- filename: mpesa-reversal-api-openapi.yml
  format: yaml
  label: M-Pesa (Safaricom Daraja) Reversal API
  slug: mpesa-reversal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-reversal-api-openapi.yml
- filename: mpesa-standing-order-api-openapi.yml
  format: yaml
  label: M-Pesa (Safaricom Daraja) Standing Order API
  slug: mpesa-standing-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-standing-order-api-openapi.yml
- filename: mpesa-tax-remittance-api-openapi.yml
  format: yaml
  label: M-Pesa (Safaricom Daraja) Tax Remittance API
  slug: mpesa-tax-remittance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-tax-remittance-api-openapi.yml
- filename: mpesa-transaction-status-api-openapi.yml
  format: yaml
  label: M-Pesa (Safaricom Daraja) Transaction Status API
  slug: mpesa-transaction-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-transaction-status-api-openapi.yml
- filename: mpesa-b2-b-api-openapi.yml
  format: yaml
  label: M-Pesa (Safaricom Daraja) B2 B API
  slug: mpesa-b2-b-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/openapi/mpesa-b2-b-api-openapi.yml
consequence_counts:
  physical: 6
  read: 4
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Mpesa Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /mpesa/b2b/v1/paymentrequest
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /mpesa/b2c/v3/paymentrequest
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /mpesa/c2b/v1/simulate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /mpesa/stkpush/v1/processrequest
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /standingorder/v1/createStandingOrderExternal
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/ussdpush/get-msisdn
operation_count: 14
overview: 'M-Pesa (Safaricom Daraja) exposes 14 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read, 4 write, and 6 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: M-Pesa (Safaricom Daraja)
provider_slug: mpesa
slug: mpesa-agentic-access
source_filename: mpesa-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/mpesa-account-balance-api-openapi.yml, openapi/mpesa-authorization-api-openapi.yml,\n  openapi/mpesa-b2-b-api-openapi.yml, openapi/mpesa-b2c-api-openapi.yml, openapi/mpesa-c2b-api-openapi.yml,\n  openapi/mpesa-dynamic-qr-api-openapi.yml, openapi/mpesa-m-pesa-express-api-openapi.yml, openapi/mpesa-reversal-api-openapi.yml,\n  openapi/mpesa-standing-order-api-openapi.yml, openapi/mpesa-tax-remittance-api-openapi.yml,\n  openapi/mpesa-transaction-status-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 4\n    acting: 10\n  by_consequence:\n    read: 4\n    physical: 6\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path:\
  \ /mpesa/accountbalance/v1/query\n  method: post\n  operationId: accountBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/v1/generate\n  method: get\n  operationId: generateAccessToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mpesa/b2b/v1/paymentrequest\n  method: post\n  operationId: b2bPaymentRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ussdpush/get-msisdn\n  method: post\n  operationId: b2bExpressCheckout\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mpesa/b2c/v3/paymentrequest\n  method: post\n  operationId: b2cPaymentRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mpesa/c2b/v1/registerurl\n  method: post\n  operationId: c2bRegisterURL\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /mpesa/c2b/v1/simulate\n  method: post\n  operationId: c2bSimulate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mpesa/qrcode/v1/generate\n  method: post\n  operationId: dynamicQR\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mpesa/stkpush/v1/processrequest\n  method: post\n  operationId: stkPush\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mpesa/stkpushquery/v1/query\n  method: post\n  operationId: stkPushQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mpesa/reversal/v1/request\n  method: post\n  operationId: reversal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /standingorder/v1/createStandingOrderExternal\n  method: post\n  operationId: createStandingOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mpesa/b2b/v1/remittax\n  method: post\n  operationId: taxRemittance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mpesa/transactionstatus/v1/query\n  method: post\n  operationId: transactionStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mpesa/refs/heads/main/agentic-access/mpesa-agentic-access.yml
summary_line: 14 operations · 10 acting
tags:
- Mobile Money
- Payments
- Fintech
- Kenya
- Africa
- M-PESA
---
