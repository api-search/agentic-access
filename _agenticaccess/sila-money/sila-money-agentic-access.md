---
acting_count: 19
action_class_counts:
  acting: 19
api_specs:
- filename: sila-money-openapi.yml
  format: yaml
  label: Sila Identity & KYC/KYB API
  slug: sila-money-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sila-money/refs/heads/main/openapi/sila-money-openapi.yml
- filename: sila-money-openapi.yml
  format: yaml
  label: Sila Wallets API
  slug: sila-money-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sila-money/refs/heads/main/openapi/sila-money-openapi.yml
- filename: sila-money-openapi.yml
  format: yaml
  label: Sila Bank Accounts API
  slug: sila-money-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sila-money/refs/heads/main/openapi/sila-money-openapi.yml
- filename: sila-money-openapi.yml
  format: yaml
  label: Sila Payments & Transactions API
  slug: sila-money-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sila-money/refs/heads/main/openapi/sila-money-openapi.yml
- filename: sila-money-openapi.yml
  format: yaml
  label: Sila Payment Methods & Cards API
  slug: sila-money-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sila-money/refs/heads/main/openapi/sila-money-openapi.yml
consequence_counts:
  physical: 7
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sila Money Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /cancel_transaction
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /get_payment_methods
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /get_transactions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /issue_sila
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /link_card
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /redeem_sila
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transfer_sila
operation_count: 19
overview: 'Sila exposes 19 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 write and 7 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Sila
provider_slug: sila-money
slug: sila-money-agentic-access
source_filename: sila-money-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/sila-money-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    acting: 19\n  by_consequence:\n    write: 12\n    physical: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /check_handle\n  method: post\n  operationId: checkHandle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /register\n  method: post\n  operationId: register\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /request_kyc\n  method: post\n  operationId: requestKyc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /check_kyc\n  method: post\n  operationId: checkKyc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents\n  method: post\n  operationId: uploadDocument\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /register_wallet\n  method: post\n  operationId: registerWallet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /get_wallet\n  method: post\n  operationId: getWallet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /get_wallets\n  method: post\n  operationId: getWallets\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /link_account\n  method: post\n  operationId: linkAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /get_accounts\n  method: post\n  operationId: getAccounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /get_account_balance\n  method: post\n  operationId: getAccountBalance\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /check_bank_account_capabilities\n  method: post\n  operationId: checkBankAccountCapabilities\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /issue_sila\n  method: post\n  operationId: issueSila\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n     \
  \ - abnormal\n      - high-value\n    audit: required\n- path: /transfer_sila\n  method: post\n  operationId: transferSila\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /redeem_sila\n  method: post\n  operationId: redeemSila\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /get_transactions\n  method: post\n  operationId: getTransactions\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cancel_transaction\n  method: post\n  operationId: cancelTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /get_payment_methods\n  method: post\n  operationId: getPaymentMethods\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /link_card\n  method: post\n  operationId: linkCard\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sila-money/refs/heads/main/agentic-access/sila-money-agentic-access.yml
summary_line: 19 operations · 19 acting
tags:
- Embedded Finance
- Banking as a Service
- Payments
- Digital Wallet
- ACH
- KYC
- KYB
- Money Transfer
- Fintech
- Banking API
- Virtual Accounts
---
