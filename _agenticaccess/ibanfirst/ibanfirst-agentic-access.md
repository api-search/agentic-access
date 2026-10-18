---
acting_count: 16
action_class_counts:
  acting: 16
  connected: 22
api_specs:
- filename: ibanfirst-accounts-api-openapi.yml
  format: yaml
  label: iBanFirst Accounts API
  slug: ibanfirst-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibanfirst/refs/heads/main/openapi/ibanfirst-accounts-api-openapi.yml
- filename: ibanfirst-beneficiaries-api-openapi.yml
  format: yaml
  label: iBanFirst Beneficiaries API
  slug: ibanfirst-beneficiaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibanfirst/refs/heads/main/openapi/ibanfirst-beneficiaries-api-openapi.yml
- filename: ibanfirst-documents-api-openapi.yml
  format: yaml
  label: iBanFirst Documents API
  slug: ibanfirst-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibanfirst/refs/heads/main/openapi/ibanfirst-documents-api-openapi.yml
- filename: ibanfirst-financial-movements-api-openapi.yml
  format: yaml
  label: iBanFirst Financial movements API
  slug: ibanfirst-financial-movements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibanfirst/refs/heads/main/openapi/ibanfirst-financial-movements-api-openapi.yml
- filename: ibanfirst-fixed-forward-payment-contract-api-openapi.yml
  format: yaml
  label: iBanFirst Fixed forward payment contract API
  slug: ibanfirst-fixed-forward-payment-contract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibanfirst/refs/heads/main/openapi/ibanfirst-fixed-forward-payment-contract-api-openapi.yml
- filename: ibanfirst-logs-api-openapi.yml
  format: yaml
  label: iBanFirst Logs API
  slug: ibanfirst-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibanfirst/refs/heads/main/openapi/ibanfirst-logs-api-openapi.yml
- filename: ibanfirst-payments-api-openapi.yml
  format: yaml
  label: iBanFirst Payments API
  slug: ibanfirst-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibanfirst/refs/heads/main/openapi/ibanfirst-payments-api-openapi.yml
- filename: ibanfirst-spot-trades-api-openapi.yml
  format: yaml
  label: iBanFirst Spot trades API
  slug: ibanfirst-spot-trades-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibanfirst/refs/heads/main/openapi/ibanfirst-spot-trades-api-openapi.yml
- filename: ibanfirst-webhook-subscriptions-api-openapi.yml
  format: yaml
  label: iBanFirst Webhook subscriptions API
  slug: ibanfirst-webhook-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibanfirst/refs/heads/main/openapi/ibanfirst-webhook-subscriptions-api-openapi.yml
consequence_counts:
  physical: 8
  read: 22
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ibanfirst Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /fixed-forwards
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /fixed-forwards/quote
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /payments/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /payments/{id}/confirm
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /payments/{id}/proofOfTransaction
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /quotes
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /trades
operation_count: 38
overview: 'iBanFirst exposes 38 API operations that an AI agent could call, of which 16 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read, 8 write, and 8 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: iBanFirst
provider_slug: ibanfirst
slug: ibanfirst-agentic-access
source_filename: ibanfirst-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: generated\nsource: openapi/ibanfirst-accounts-api-openapi.yml, openapi/ibanfirst-beneficiaries-api-openapi.yml,\n  openapi/ibanfirst-documents-api-openapi.yml, openapi/ibanfirst-financial-movements-api-openapi.yml,\n  openapi/ibanfirst-fixed-forward-payment-contract-api-openapi.yml, openapi/ibanfirst-logs-api-openapi.yml,\n  openapi/ibanfirst-payments-api-openapi.yml, openapi/ibanfirst-spot-trades-api-openapi.yml,\n  openapi/ibanfirst-webhook-subscriptions-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 38\n  by_action_class:\n    acting: 16\n    connected: 22\n  by_consequence:\n    write: 8\n    read: 22\n    physical: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /wallets\n  method:\
  \ post\n  operationId: postWallets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wallets\n  method: get\n  operationId: getWallets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wallets/{id}\n  method: get\n  operationId: getWalletsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wallets/{id}/balance/{date}\n  method: get\n  operationId: getWalletsByIdBalanceByDate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /externalBankAccounts\n\
  \  method: post\n  operationId: postExternalBankAccounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /externalBankAccounts\n  method: get\n  operationId: getExternalBankAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /externalBankAccounts/{id}\n  method: get\n  operationId: getExternalBankAccountsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /externalBankAccounts/{id}\n  method: delete\n  operationId: deleteExternalBankAccountsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents\n  method: get\n  operationId: getDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{id}\n  method: get\n  operationId: getDocumentsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/RIB\n  method: get\n  operationId: getDocumentsRIB\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/upload/{object}/{objectId}/{typeOfDocumentation}\n  method: put\n  operationId: putDocumentsUploadByObjectByObjectIdByTypeOfDocumentation\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /financialMovements\n  method: get\n  operationId: getFinancialMovements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /financialMovements/{id}\n  method: get\n  operationId: getFinancialMovementsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fixed-forwards/quote\n  method: post\n  operationId: postFixedForwardsQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fixed-forwards\n  method: post\n  operationId: postFixedForwards\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fixed-forwards\n  method: get\n  operationId: getFixedForwards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fixed-forwards/{fixedForwardId}\n  method: get\n  operationId: getFixedForwardsByFixedForwardId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /logs\n  method: get\n  operationId: getLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /logs/{nonce}\n  method: get\n  operationId: getLogsByNonce\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/options/{walletId}/{externalBankAccountId}\n  method: get\n  operationId: getPaymentsOptionsByWalletIdByExternalBankAccountId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments\n  method: post\n  operationId: postPayments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/{id}/confirm\n  method: put\n  operationId: putPaymentsByIdConfirm\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/{id}/proofOfTransaction\n  method: put\n  operationId: putPaymentsByIdProofOfTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/{status}\n\
  \  method: get\n  operationId: getPaymentsByStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/{id}\n  method: get\n  operationId: getPaymentsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/{id}\n  method: delete\n  operationId: deletePaymentsById\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /quotes\n  method: post\n  operationId: postQuotes\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /trades\n  method: post\n  operationId: postTrades\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /trades/_{status}\n  method: get\n  operationId: getTrades{status}\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trades/{id}\n  method: get\n  operationId: getTradesById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: post\n  operationId: postWebhooks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks\n  method: get\n  operationId: getWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/{webhookId}\n  method: get\n  operationId: getWebhooksByWebhookId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/{webhookId}\n  method: patch\n  operationId: patchWebhooksByWebhookId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{webhookId}\n  method: delete\n  operationId: deleteWebhooksByWebhookId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{webhookId}/rotate-secret\n  method: post\n  operationId: postWebhooksByWebhookIdRotateSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{webhookId}/failed-notifications\n  method:\
  \ get\n  operationId: getWebhooksByWebhookIdFailedNotifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ibanfirst/refs/heads/main/agentic-access/ibanfirst-agentic-access.yml
summary_line: 38 operations · 16 acting
tags:
- Company
- Fintech Insurtech
- Cross-Border Payments
- Foreign Exchange
- B2B Payments
- Treasury
- multi-currency-accounts
- SEPA
- PSD2
- Open Banking
- currency-risk-management
- Webhook
- MCP
- Belgium
- Europe
- SWIFT
---
