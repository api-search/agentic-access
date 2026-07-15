---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 9
api_specs:
- filename: us-bank-corporate-account-information-openapi.yml
  format: yaml
  label: US Bank Corporate Account Information API
  slug: us-bank-corporate-account-information
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-bancorp/refs/heads/main/openapi/us-bank-corporate-account-information-openapi.yml
- filename: us-bank-rtp-openapi.yml
  format: yaml
  label: US Bank RTP Real-Time Payments API
  slug: us-bank-rtp
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-bancorp/refs/heads/main/openapi/us-bank-rtp-openapi.yml
- filename: us-bank-ach-originations-openapi.yml
  format: yaml
  label: US Bank ACH Originations API
  slug: us-bank-ach-originations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-bancorp/refs/heads/main/openapi/us-bank-ach-originations-openapi.yml
- filename: us-bank-positive-pay-openapi.yml
  format: yaml
  label: US Bank Positive Pay API
  slug: us-bank-positive-pay
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-bancorp/refs/heads/main/openapi/us-bank-positive-pay-openapi.yml
- filename: us-bank-push-to-card-openapi.yml
  format: yaml
  label: US Bank Push to Card API
  slug: us-bank-push-to-card
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-bancorp/refs/heads/main/openapi/us-bank-push-to-card-openapi.yml
consequence_counts:
  physical: 3
  read: 9
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Us Bancorp Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /push-to-card/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rtp/credit-transfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rtp/requests-for-payment
operation_count: 15
overview: 'US Bancorp exposes 15 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 3 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: US Bancorp
provider_slug: us-bancorp
slug: us-bancorp-agentic-access
source_filename: us-bancorp-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/us-bank-corporate-account-information-openapi.yml, openapi/us-bank-positive-pay-openapi.yml,\n  openapi/us-bank-push-to-card-openapi.yml, openapi/us-bank-rtp-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 9\n    acting: 6\n  by_consequence:\n    read: 9\n    write: 3\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /accounts\n  method: get\n  operationId: listAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/current-day-balances\n  method: post\n  operationId: getCurrentDayBalances\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/previous-day-balances\n  method: post\n  operationId: getPreviousDayBalances\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountNumber}/current-day-transactions\n  method: get\n  operationId: getCurrentDayTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountNumber}/transactions\n  method: get\n  operationId: getAccountTransactions\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /positive-pay/exceptions\n  method: get\n  operationId: getPositivePayExceptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /positive-pay/exceptions/{exceptionId}/decision\n  method: post\n  operationId: submitExceptionDecision\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /positive-pay/exceptions/history\n  method: get\n  operationId: getExceptionHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /push-to-card/payments\n\
  \  method: post\n  operationId: initiatePushToCardPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /push-to-card/payments/{paymentId}\n  method: get\n  operationId: getPushToCardPaymentStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rtp/eligibility\n  method: get\n  operationId: getRTPEligibility\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rtp/credit-transfers\n  method: post\n  operationId: initiateRTPCreditTransfer\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rtp/credit-transfers/{transactionId}\n  method: get\n  operationId: getRTPCreditTransferStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rtp/requests-for-payment\n  method: post\n  operationId: initiateRTPRequestForPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rtp/requests-for-payment/{requestId}\n\
  \  method: get\n  operationId: getRTPRequestForPaymentStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-bancorp/refs/heads/main/agentic-access/us-bancorp-agentic-access.yml
summary_line: 15 operations · 6 acting
tags:
- Banking
- Finance
- Fortune 500
- Corporate Banking
- Payments
- Open Banking
- Treasury Management
- Consumer Banking
---
