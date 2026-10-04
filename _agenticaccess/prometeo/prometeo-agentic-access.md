---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 17
api_specs:
- filename: prometeo-account-validation-api-openapi.yml
  format: yaml
  label: Prometeo Account Validation API
  slug: prometeo-account-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometeo/refs/heads/main/openapi/prometeo-account-validation-api-openapi.yml
- filename: prometeo-banking-api-openapi.yml
  format: yaml
  label: Prometeo Banking API
  slug: prometeo-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometeo/refs/heads/main/openapi/prometeo-banking-api-openapi.yml
- filename: prometeo-cross-border-api-openapi.yml
  format: yaml
  label: Prometeo Cross-Border API
  slug: prometeo-cross-border-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometeo/refs/heads/main/openapi/prometeo-cross-border-api-openapi.yml
- filename: prometeo-identity-api-openapi.yml
  format: yaml
  label: Prometeo Identity API
  slug: prometeo-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometeo/refs/heads/main/openapi/prometeo-identity-api-openapi.yml
- filename: prometeo-payment-api-openapi.yml
  format: yaml
  label: Prometeo Payment API
  slug: prometeo-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prometeo/refs/heads/main/openapi/prometeo-payment-api-openapi.yml
consequence_counts:
  physical: 7
  read: 17
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Prometeo Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/payment-intent/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /fx/exchange
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payin/intent
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payin/refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payout/transfer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transfer/confirm
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transfer/preprocess
operation_count: 28
overview: 'Prometeo exposes 28 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read, 4 write, and 7 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Prometeo
provider_slug: prometeo
slug: prometeo-agentic-access
source_filename: prometeo-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/prometeo-account-validation-api-openapi.yml, openapi/prometeo-banking-api-openapi.yml,\n  openapi/prometeo-cross-border-api-openapi.yml, openapi/prometeo-identity-api-openapi.yml,\n  openapi/prometeo-payment-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 28\n  by_action_class:\n    acting: 11\n    connected: 17\n  by_consequence:\n    write: 4\n    read: 17\n    physical: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /validate-account/\n  method: post\n  operationId: validateAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /login/\n  method: post\n  operationId: login\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /login-procedure/\n  method: post\n  operationId: loginProcedure\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /info/\n  method: get\n  operationId: getClientInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/\n\
  \  method: get\n  operationId: listClients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/{client_id}/\n  method: get\n  operationId: selectClient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/\n  method: get\n  operationId: listAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /movement/\n  method: get\n  operationId: listMovements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /credit-card/\n  method: get\n  operationId: listCreditCards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /credit-card/{card_number}/movements\n  method: get\n  operationId: listCreditCardMovements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provider/\n  method: get\n  operationId: listProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provider/{provider_code}/\n  method: get\n  operationId: getProviderDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transfer/destinations\n  method: get\n  operationId: listTransferDestinations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transfer/preprocess\n\
  \  method: post\n  operationId: preprocessTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transfer/confirm\n  method: post\n  operationId: confirmTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /logout/\n  method: get\n  operationId: logout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /payin/intent\n  method: post\n  operationId: createPayinIntent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payin/intent\n  method: get\n  operationId: listPayinIntents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payin/intent/{intent_id}\n  method: get\n  operationId: getPayinIntent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payin/refund\n  method: post\n  operationId: refundPayin\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payout/transfer\n  method: post\n  operationId: createPayout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payout/transfer\n  method: get\n  operationId: listPayouts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payout/transfer/{payout_id}\n  method: get\n  operationId: getPayout\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fx/exchange\n  method: post\n  operationId: exchangeFx\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /query\n  method: post\n  operationId: curpQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reverse-query\n  method: post\n  operationId: curpReverseQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/v1/payment-intent/\n  method: post\n  operationId: createPaymentIntent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/payment-intent/{intent_id}\n  method: get\n  operationId: getPaymentIntent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prometeo/refs/heads/main/agentic-access/prometeo-agentic-access.yml
summary_line: 28 operations · 11 acting
tags:
- Open Banking
- Payments
- Fintech
- Latin America
- Financial Data
- Account Validation
- Cross-Border
---
