---
acting_count: 20
action_class_counts:
  acting: 20
  connected: 17
api_specs:
- filename: keycorp-account-information-api-openapi.yml
  format: yaml
  label: KeyCorp Account Information API
  slug: keycorp-account-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keycorp/refs/heads/main/openapi/keycorp-account-information-api-openapi.yml
- filename: keycorp-account-transactions-api-openapi.yml
  format: yaml
  label: KeyCorp Account Transactions API
  slug: keycorp-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keycorp/refs/heads/main/openapi/keycorp-account-transactions-api-openapi.yml
- filename: keycorp-accounts-api-openapi.yml
  format: yaml
  label: KeyCorp Accounts API
  slug: keycorp-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keycorp/refs/heads/main/openapi/keycorp-accounts-api-openapi.yml
- filename: keycorp-ach-api-openapi.yml
  format: yaml
  label: KeyCorp ACH API
  slug: keycorp-ach-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keycorp/refs/heads/main/openapi/keycorp-ach-api-openapi.yml
- filename: keycorp-ach-payment-origination-api-openapi.yml
  format: yaml
  label: KeyCorp ACH Payment Origination API
  slug: keycorp-ach-payment-origination-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keycorp/refs/heads/main/openapi/keycorp-ach-payment-origination-api-openapi.yml
- filename: keycorp-ach-payment-request-inquiry-api-openapi.yml
  format: yaml
  label: KeyCorp ACH Payment Request Inquiry API
  slug: keycorp-ach-payment-request-inquiry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keycorp/refs/heads/main/openapi/keycorp-ach-payment-request-inquiry-api-openapi.yml
- filename: keycorp-ach-transactions-api-openapi.yml
  format: yaml
  label: KeyCorp ACH Transactions API
  slug: keycorp-ach-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keycorp/refs/heads/main/openapi/keycorp-ach-transactions-api-openapi.yml
- filename: keycorp-imagecheck-api-openapi.yml
  format: yaml
  label: KeyCorp Image Check API
  slug: keycorp-imagecheck-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keycorp/refs/heads/main/openapi/keycorp-imagecheck-api-openapi.yml
- filename: keycorp-initiate-api-openapi.yml
  format: yaml
  label: KeyCorp Initiate API
  slug: keycorp-initiate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keycorp/refs/heads/main/openapi/keycorp-initiate-api-openapi.yml
- filename: keycorp-participant-api-openapi.yml
  format: yaml
  label: KeyCorp Participant API
  slug: keycorp-participant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keycorp/refs/heads/main/openapi/keycorp-participant-api-openapi.yml
- filename: keycorp-rtp-api-openapi.yml
  format: yaml
  label: KeyCorp RTP API
  slug: keycorp-rtp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keycorp/refs/heads/main/openapi/keycorp-rtp-api-openapi.yml
- filename: keycorp-stoppayments-api-openapi.yml
  format: yaml
  label: KeyCorp Stop Payments API
  slug: keycorp-stoppayments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keycorp/refs/heads/main/openapi/keycorp-stoppayments-api-openapi.yml
- filename: keycorp-undo-ach-payment-request-api-openapi.yml
  format: yaml
  label: KeyCorp Undo ACH Payment Request API
  slug: keycorp-undo-ach-payment-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keycorp/refs/heads/main/openapi/keycorp-undo-ach-payment-request-api-openapi.yml
- filename: keycorp-validate-api-openapi.yml
  format: yaml
  label: KeyCorp Validate API
  slug: keycorp-validate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keycorp/refs/heads/main/openapi/keycorp-validate-api-openapi.yml
- filename: keycorp-wire-api-openapi.yml
  format: yaml
  label: KeyCorp Wire API
  slug: keycorp-wire-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keycorp/refs/heads/main/openapi/keycorp-wire-api-openapi.yml
- filename: keycorp-wire-rtp-v1-api-openapi.yml
  format: yaml
  label: KeyCorp Wire/RTP v1 API
  slug: keycorp-wire-rtp-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keycorp/refs/heads/main/openapi/keycorp-wire-rtp-v1-api-openapi.yml
- filename: keycorp-wire-rtp-v2-api-openapi.yml
  format: yaml
  label: KeyCorp Wire/RTP v2 API
  slug: keycorp-wire-rtp-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keycorp/refs/heads/main/openapi/keycorp-wire-rtp-v2-api-openapi.yml
- filename: keycorp-health-check-api-openapi.yml
  format: yaml
  label: KeyCorp Health Check API
  slug: keycorp-health-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keycorp/refs/heads/main/openapi/keycorp-health-check-api-openapi.yml
consequence_counts:
  physical: 16
  read: 17
  safety-critical: 1
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Keycorp Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /commercial/checks/v1/stops/place
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /"Callback URL from client for ACH alerts - AL00906"
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /"Callback URL from client for AL00901"
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /"Callback URL from client for Wire/RTP alerts - AL00907"
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ach/payments/v1/addenda
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ach/payments/v1/ccd
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ach/payments/v1/ctx
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ach/payments/v1/ppd
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ach/payments/v1/status
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ach/payments/v1/status/addenda
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ach/payments/v1/tel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ach/payments/v1/undo
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ach/payments/v1/web
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rtp/v1/payment/initiate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rtp/v1/payment/validate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rtp/v1/transactions/list
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /wireInquiry/v1/transactions/list
operation_count: 37
overview: 'KeyCorp exposes 37 API operations that an AI agent could call, of which 20 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read, 3 write, 16 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: KeyCorp
provider_slug: keycorp
slug: keycorp-agentic-access
source_filename: keycorp-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: generated\nsource: openapi/keycorp-account-information-api-openapi.yml, openapi/keycorp-account-transactions-api-openapi.yml,\n  openapi/keycorp-accounts-api-openapi.yml, openapi/keycorp-ach-api-openapi.yml, openapi/keycorp-ach-payment-origination-api-openapi.yml,\n  openapi/keycorp-ach-payment-request-inquiry-api-openapi.yml, openapi/keycorp-ach-transactions-api-openapi.yml,\n  openapi/keycorp-health-check-api-openapi.yml, openapi/keycorp-imagecheck-api-openapi.yml,\n  openapi/keycorp-initiate-api-openapi.yml, openapi/keycorp-participant-api-openapi.yml, openapi/keycorp-rtp-api-openapi.yml,\n  openapi/keycorp-stoppayments-api-openapi.yml, openapi/keycorp-undo-ach-payment-request-api-openapi.yml,\n  openapi/keycorp-validate-api-openapi.yml, openapi/keycorp-wire-api-openapi.yml, openapi/keycorp-wire-rtp-v1-api-openapi.yml,\n  openapi/keycorp-wire-rtp-v2-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified\
  \ heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 37\n  by_action_class:\n    connected: 17\n    acting: 20\n  by_consequence:\n    read: 17\n    write: 3\n    physical: 16\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /commercial/accounts/v1/{accountId}\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /commercial/accounts/v1/list\n  method: get\n  operationId: searchForAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /commercial/accounts/v1/{accountId}/transactions/previous\n  method: get\n  operationId: searchForPreviousDayAccountTransactionsV1\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /commercial/accounts/v1/{accountId}/transactions/current\n  method: get\n  operationId: searchForCurrentDayAccountTransactionsV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/validations/v2/verifyAccount\n  method: post\n  operationId: verifyAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /\"Callback URL from client for ACH alerts - AL00906\"\n  method: post\n  operationId: post\"Callback URL from client for ACH alerts  AL00906\"\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ach/payments/v1/ccd\n  method: post\n  operationId: achPaymentCCD\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ach/payments/v1/ctx\n  method: post\n  operationId: achPaymentCTX\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ach/payments/v1/ppd\n  method: post\n  operationId: achPaymentPPD\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ach/payments/v1/tel\n  method: post\n  operationId: achPaymentTEL\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ach/payments/v1/web\n  method: post\n  operationId: achPaymentWEB\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ach/payments/v1/addenda\n  method: post\n  operationId: achPaymentAddenda\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ach/payments/v1/status\n  method: post\n  operationId: achPaymentStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ach/payments/v1/status/addenda\n  method: post\n  operationId: achPaymentAddendasStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/transactions/v1/ach/detail/{parNumber}\n  method: get\n  operationId: searchAchTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/transactions/v1/ach/list\n  method: post\n  operationId: searchAchTransactions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/transactions/v1/ach/settled/{settlementTransactionId}\n  method: get\n  operationId: searchAchSettledTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/validations/v2/healthCheck\n  method: get\n  operationId: healthCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/transactions/v1/healthCheck\n  method: get\n  operationId: healthCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ach/payments/v1/healthCheck\n  method: get\n \
  \ operationId: healthCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /commercial/checks/v1/healthCheck\n  method: get\n  operationId: healthCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rtp/v1/healthCheck\n  method: get\n  operationId: healthCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rtp/v1/payment/healthCheck\n  method: get\n  operationId: healthCheckv1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wireInquiry/v1/healthCheck\n  method: get\n  operationId: healthCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /commercial/checks/v1/images/list\n  method: post\n  operationId: CheckImageListRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rtp/v1/payment/initiate\n  method: post\n  operationId: Payment-Initiate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rtp/v1/payment/rtp/participant\n  method: get\n  operationId: participantList\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rtp/v1/payment/rtp/participant/{routingNumber}\n  method: get\n  operationId: participant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rtp/v1/transactions/list\n  method: post\n  operationId: searchRtpTransactions\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rtp/v1/transactions/detail/{transactionId}\n  method: get\n  operationId: searchRtpTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n \
  \   audit: none\n- path: /commercial/checks/v1/stops/place\n  method: post\n  operationId: PlaceStopPayments\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /ach/payments/v1/undo\n  method: post\n  operationId: achPaymentUndo\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rtp/v1/payment/validate\n  method: post\n  operationId: Payment-Validate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wireInquiry/v1/transactions/list\n  method: post\n  operationId: searchWireTransactions\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wireInquiry/v1/transactions/detail/{transactionId}\n  method: get\n  operationId: searchWireTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\"Callback URL from client for AL00901\"\n  method: post\n\
  \  operationId: post\"Callback URL from client for AL00901\"\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /\"Callback URL from client for Wire/RTP alerts - AL00907\"\n  method: post\n  operationId: post\"Callback URL from client for WireRTP alerts  AL00907\"\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keycorp/refs/heads/main/agentic-access/keycorp-agentic-access.yml
summary_line: 37 operations · 20 acting · 1 human-in-the-loop
tags:
- Banking
- Commercial Banking
- Financial-Services
- Fortune 500
- Payments
- United States
- Super-Regional Bank
- Treasury Management
- Embedded Banking
- ACH
- Real-Time Payments
- Wire Transfers
---
