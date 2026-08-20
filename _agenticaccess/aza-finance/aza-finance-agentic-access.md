---
acting_count: 22
action_class_counts:
  acting: 22
  connected: 27
api_specs:
- filename: aza-finance-account-debits-api-openapi.yml
  format: yaml
  label: AZA Finance Account Debits API
  slug: aza-finance-account-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-account-debits-api-openapi.yml
- filename: aza-finance-account-validation-api-openapi.yml
  format: yaml
  label: AZA Finance Account Validation API
  slug: aza-finance-account-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-account-validation-api-openapi.yml
- filename: aza-finance-accounts-api-openapi.yml
  format: yaml
  label: AZA Finance Accounts API
  slug: aza-finance-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-accounts-api-openapi.yml
- filename: aza-finance-api-logs-api-openapi.yml
  format: yaml
  label: AZA Finance API Logs API
  slug: aza-finance-api-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-api-logs-api-openapi.yml
- filename: aza-finance-currency-info-api-openapi.yml
  format: yaml
  label: AZA Finance Currency Info API
  slug: aza-finance-currency-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-currency-info-api-openapi.yml
- filename: aza-finance-dlocal-balance-api-openapi.yml
  format: yaml
  label: AZA Finance dlocal balance API
  slug: aza-finance-dlocal-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-dlocal-balance-api-openapi.yml
- filename: aza-finance-documents-api-openapi.yml
  format: yaml
  label: AZA Finance Documents API
  slug: aza-finance-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-documents-api-openapi.yml
- filename: aza-finance-logs-api-openapi.yml
  format: yaml
  label: AZA Finance Logs API
  slug: aza-finance-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-logs-api-openapi.yml
- filename: aza-finance-mandates-api-openapi.yml
  format: yaml
  label: AZA Finance Mandates API
  slug: aza-finance-mandates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-mandates-api-openapi.yml
- filename: aza-finance-payin-methods-api-openapi.yml
  format: yaml
  label: AZA Finance Payin Methods API
  slug: aza-finance-payin-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-payin-methods-api-openapi.yml
- filename: aza-finance-payment-methods-api-openapi.yml
  format: yaml
  label: AZA Finance Payment Methods API
  slug: aza-finance-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-payment-methods-api-openapi.yml
- filename: aza-finance-payout-methods-api-openapi.yml
  format: yaml
  label: AZA Finance Payout Methods API
  slug: aza-finance-payout-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-payout-methods-api-openapi.yml
- filename: aza-finance-recipients-api-openapi.yml
  format: yaml
  label: AZA Finance Recipients API
  slug: aza-finance-recipients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-recipients-api-openapi.yml
- filename: aza-finance-senders-api-openapi.yml
  format: yaml
  label: AZA Finance Senders API
  slug: aza-finance-senders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-senders-api-openapi.yml
- filename: aza-finance-transactions-api-openapi.yml
  format: yaml
  label: AZA Finance Transactions API
  slug: aza-finance-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-transactions-api-openapi.yml
- filename: aza-finance-webhooks-api-openapi.yml
  format: yaml
  label: AZA Finance Webhooks API
  slug: aza-finance-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-webhooks-api-openapi.yml
consequence_counts:
  physical: 7
  read: 27
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Aza Finance Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payout_methods
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /payout_methods/{Payout Method ID}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /payout_methods/{Payout Method ID}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /senders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /senders/{Sender ID}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /senders/{Sender ID}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transactions/{Transaction ID}/payout
operation_count: 49
overview: 'AZA Finance exposes 49 API operations that an AI agent could call, of which 22 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 27 read, 15 write, and 7 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AZA Finance
provider_slug: aza-finance
slug: aza-finance-agentic-access
source_filename: aza-finance-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/aza-finance-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 49\n  by_action_class:\n    connected: 27\n    acting: 22\n  by_consequence:\n    read: 27\n    write: 15\n    physical: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /accounts\n  method: get\n  operationId: get-accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{Currency}\n  method: get\n  operationId: get-account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/debits\n\
  \  method: post\n  operationId: post-accounts-debits\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account_validations\n  method: post\n  operationId: post-account-validations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api_logs\n  method: get\n  operationId: get-api-logs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api_logs/{API Log ID}\n  method: get\n  operationId: get-api-log\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dlocal/balance\n  method: get\n  operationId: get-balance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /info/currencies\n  method: get\n  operationId: info-currencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /info/currencies/in\n  method: get\n  operationId: info-currencies-in\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /info/currencies/out\n  method: get\n  operationId: info-currencies-out\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /documents\n  method: get\n  operationId: get-documents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents\n  method: post\n  operationId: post-documents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{Document ID}\n  method: get\n  operationId: get-document\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /info/payment_methods/in\n  method: get\n  operationId: payment-methods-in\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /info/payment_methods/out\n  method: get\n  operationId: payment-methods-out\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /logs/webhooks\n  method: get\n  operationId: get-webhook-logs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /logs/{Webhook Log ID}\n  method: get\n  operationId: get-webhook-log\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mandates/{Mandate ID}\n  method: get\n  operationId: get-mandate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payin_methods/{PayinMethod ID}\n  method: get\n  operationId: get-payin-method\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payin_methods/{PayinMethod ID}\n  method: delete\n  operationId: delete-payin-method\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payin_methods/{PayinMethod ID}\n  method: patch\n  operationId: patch-payin-method\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payin_methods/{PayinMethod ID}/retry\n  method: post\n  operationId: retry-payin-method\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payout_methods\n  method: get\n  operationId: get-payout-methods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payout_methods\n  method: post\n  operationId: post-payout-methods\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payout_methods/{Payout Method ID}\n  method: get\n  operationId: get-payout-method\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payout_methods/{Payout Method ID}\n  method: delete\n  operationId: delete-payout-method\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payout_methods/{Payout Method ID}\n  method: patch\n  operationId: patch-payout-method\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recipients\n\
  \  method: get\n  operationId: get-recipients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recipients/{Recipient ID}\n  method: delete\n  operationId: delete-recipient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recipients/{Recipient ID}\n  method: patch\n  operationId: patch-recipient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recipients/{Recipient ID}/proof_of_payments\n  method: get\n  operationId:\
  \ proof-of-payments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /senders\n  method: get\n  operationId: get-senders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /senders\n  method: post\n  operationId: post-senders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /senders/{Sender ID}\n  method: get\n  operationId: get-sender\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /senders/{Sender\
  \ ID}\n  method: delete\n  operationId: delete-sender\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /senders/{Sender ID}\n  method: patch\n  operationId: patch-sender\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transactions\n  method: get\n  operationId: get-transactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /transactions\n  method: post\n  operationId: post-transactions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transactions/calculate\n  method: post\n  operationId: calculate-transactions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transactions/validate\n  method: post\n  operationId: validate-transactions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transactions/create_and_fund\n  method: post\n  operationId: create-and-fund-transaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transactions/{Transaction ID}\n  method: get\n  operationId: get-transaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/{Transaction ID}/payin\n  method: post\n  operationId: payin-transaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /transactions/{Transaction ID}/payout\n  method: post\n  operationId: payout-transaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks\n  method: get\n  operationId: get-webhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: post\n  operationId: post-webhooks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /webhooks/{Webhook ID}\n  method: get\n  operationId: get-webhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/{Webhook ID}\n  method: delete\n  operationId: delete-webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/events\n  method: get\n  operationId: get-webhook-events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/agentic-access/aza-finance-agentic-access.yml
summary_line: 49 operations · 22 acting
tags:
- Company
- Financial-Services
- Payments
- Foreign Exchange
- Cross-Border Payments
- Africa
- Fintech
---
