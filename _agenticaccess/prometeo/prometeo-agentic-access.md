---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 12
api_specs:
- filename: prometeo-openapi.yml
  format: yaml
  label: Prometeo Banking API
  slug: prometeo-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometeo/refs/heads/main/openapi/prometeo-openapi.yml
- filename: prometeo-openapi.yml
  format: yaml
  label: Prometeo Account Validation API
  slug: prometeo-account-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometeo/refs/heads/main/openapi/prometeo-openapi.yml
- filename: prometeo-openapi.yml
  format: yaml
  label: Prometeo Cross-Border Payments API
  slug: prometeo-cross-border-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometeo/refs/heads/main/openapi/prometeo-openapi.yml
- filename: prometeo-openapi.yml
  format: yaml
  label: Prometeo Payment API
  slug: prometeo-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometeo/refs/heads/main/openapi/prometeo-openapi.yml
- filename: prometeo-openapi.yml
  format: yaml
  label: Prometeo Identity API (CURP)
  slug: prometeo-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometeo/refs/heads/main/openapi/prometeo-openapi.yml
consequence_counts:
  read: 12
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents - review and bind audience per deployment. Prometeo moves real money and touches regulated financial and identity data, so money-movement operations are marked human-in-the-loop required. See research/curity/agentic-governance/.
human_in_the_loop: 5
kind: agentic-access
layout: agentic-access
method: generated
name: Prometeo Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 26
overview: 'Prometeo exposes 26 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read and 14 write.


  5 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Prometeo
provider_slug: prometeo
slug: prometeo-agentic-access
source_filename: prometeo-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: generated\nsource: openapi/prometeo-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents - review and bind\n  audience per deployment. Prometeo moves real money and touches regulated financial and\n  identity data, so money-movement operations are marked human-in-the-loop required.\n  See research/curity/agentic-governance/.\nsummary:\n  operations: 26\n  by_action_class:\n    acting: 14\n    connected: 12\n  by_consequence:\n    write: 14\n    read: 12\n  human_in_the_loop_required: 5\noperations:\n- path: /login/\n  method: post\n  operationId: login\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - credential-entry\n\
  \    audit: required\n- path: /login-procedure/\n  method: post\n  operationId: loginProcedure\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - mfa\n    audit: required\n- path: /info/\n  method: get\n  operationId: getClientInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/\n  method: get\n  operationId: listClients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/{client_id}/\n  method: get\n  operationId: selectClient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    audit: required\n\
  - path: /account/\n  method: get\n  operationId: listAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: required\n- path: /movement/\n  method: get\n  operationId: listMovements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: required\n- path: /credit-card/\n  method: get\n  operationId: listCreditCards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: required\n- path: /credit-card/{card_number}/movements\n  method: get\n  operationId: listCreditCardMovements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: required\n- path: /provider/\n  method: get\n  operationId: listProviders\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provider/{provider_code}/\n  method: get\n  operationId: getProviderDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transfer/destinations\n  method: get\n  operationId: listTransferDestinations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: required\n- path: /transfer/preprocess\n  method: post\n  operationId: preprocessTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 600\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - high-value\n      - abnormal\n    audit: required\n- path: /transfer/confirm\n  method: post\n  operationId: confirmTransfer\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - money-movement\n    audit: required\n- path: /logout/\n  method: get\n  operationId: logout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    audit: none\n- path: /validate-account/\n  method: post\n  operationId: validateAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - pii\n    audit: required\n- path: /query\n  method: post\n  operationId: curpQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - pii\n    audit: required\n- path: /reverse-query\n  method: post\n  operationId: curpReverseQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - pii\n    audit: required\n- path: /payin/intent\n  method: post\n  operationId: createPayinIntent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 600\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - high-value\n    audit: required\n- path: /payin/intent\n  method: get\n  operationId: listPayinIntents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: required\n- path: /payin/intent/{intent_id}\n\
  \  method: get\n  operationId: getPayinIntent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: required\n- path: /payin/refund\n  method: post\n  operationId: refundPayin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - money-movement\n    audit: required\n- path: /payout/transfer\n  method: post\n  operationId: createPayout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - money-movement\n    audit: required\n- path: /payout/transfer/{payout_id}\n  method: get\n  operationId: getPayout\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: required\n- path: /fx/exchange\n  method: post\n  operationId: exchangeFx\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - money-movement\n    audit: required\n- path: /api/v1/payment-intent/\n  method: post\n  operationId: createPaymentIntent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - money-movement\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prometeo/refs/heads/main/agentic-access/prometeo-agentic-access.yml
summary_line: 26 operations · 14 acting · 5 human-in-the-loop
tags:
- Open Banking
- Payments
- FinTech
- LatAm
- Financial Data
- Account Validation
- Cross-Border
---
