---
acting_count: 25
action_class_counts:
  acting: 25
  connected: 23
api_specs:
- filename: helcim-api.json
  format: json
  label: Helcim Payment API
  slug: helcim-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helcim/refs/heads/main/openapi/helcim-api.json
- filename: helcim-api.json
  format: json
  label: Helcim ACH Payment API
  slug: helcim-ach-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helcim/refs/heads/main/openapi/helcim-api.json
- filename: helcim-api.json
  format: json
  label: Helcim Customer API
  slug: helcim-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helcim/refs/heads/main/openapi/helcim-api.json
- filename: helcim-api.json
  format: json
  label: Helcim Invoice API
  slug: helcim-invoice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helcim/refs/heads/main/openapi/helcim-api.json
- filename: helcim-api.json
  format: json
  label: Helcim Card Transaction & Batch API
  slug: helcim-card-transaction-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helcim/refs/heads/main/openapi/helcim-api.json
- filename: helcim-api.json
  format: json
  label: Helcim Card Terminal & Device API
  slug: helcim-terminal-device-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helcim/refs/heads/main/openapi/helcim-api.json
consequence_counts:
  physical: 16
  read: 23
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Helcim Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /ach/batches/{batchId}/settle
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /ach/transactions/{transactionId}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /ach/transactions/{transactionId}/refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /ach/transactions/{transactionId}/void
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /ach/withdraw
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /devices/{code}/payment/purchase
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /devices/{code}/payment/refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /invoices/{invoiceId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment/capture
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment/preauth
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment/purchase
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment/refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment/reverse
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment/verify
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment/withdraw
operation_count: 48
overview: 'Helcim exposes 48 API operations that an AI agent could call, of which 25 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 23 read, 9 write, and 16 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Helcim
provider_slug: helcim
slug: helcim-agentic-access
source_filename: helcim-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: generated\nsource: openapi/helcim-api.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 48\n  by_action_class:\n    connected: 23\n    acting: 25\n  by_consequence:\n    read: 23\n    physical: 16\n    write: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /connection-test\n  method: get\n  operationId: connectionTest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment/purchase\n  method: post\n  operationId: purchase\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n\
  \      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment/preauth\n  method: post\n  operationId: preauth\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment/capture\n  method: post\n  operationId: capture\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment/verify\n  method: post\n\
  \  operationId: verify\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment/refund\n  method: post\n  operationId: refund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment/reverse\n  method: post\n  operationId: reverse\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment/withdraw\n  method: post\n  operationId: withdraw\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /card-batches\n  method: get\n  operationId: get-card-batches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /card-batches/{cardBatchId}\n  method: get\n  operationId: get-card-batch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /card-batches/{cardBatchId}/settle\n\
  \  method: post\n  operationId: settle-card-batch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /card-transactions\n  method: get\n  operationId: get-card-transactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /card-transactions/{cardTransactionId}\n  method: get\n  operationId: get-card-transaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers\n  method: get\n  operationId: get-customers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /customers\n  method: post\n  operationId: create-customer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{customerId}\n  method: get\n  operationId: get-customer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}\n  method: put\n  operationId: update-customer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{customerId}/cards\n  method: get\n  operationId:\
  \ get-customer-cards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}/cards/{cardId}\n  method: get\n  operationId: get-customer-card\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}/cards/{cardId}\n  method: delete\n  operationId: delete-customer-card\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{customerId}/cards/{cardId}/default\n  method: patch\n  operationId: set-customer-card-default\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{customerId}/pads\n  method: get\n  operationId: get-pads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}/bank-accounts\n  method: get\n  operationId: get-customer-bank-accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}/bank-accounts\n  method: post\n  operationId: create-bank-account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n     \
  \ - high-value\n    audit: required\n- path: /customers/{customerId}/bank-accounts/request-new\n  method: get\n  operationId: request-new-bank-account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}/bank-accounts/{bankAccountId}\n  method: get\n  operationId: get-customer-bank-account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}/bank-accounts/{bankAccountId}\n  method: delete\n  operationId: delete-customer-bank-account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{customerId}/bank-accounts/{bankAccountId}/default\n\
  \  method: patch\n  operationId: set-customer-bank-account-default\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{customerId}/bank-accounts/{bankAccountId}/pads/{padId}\n  method: get\n  operationId: get-pad\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customerId}/bank-accounts/{bankAccountId}/pads/{padId}\n  method: put\n  operationId: update-pad\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /invoices\n  method: post\n  operationId: create-invoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invoices\n  method: get\n  operationId: get-invoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoices/{invoiceId}\n  method: get\n  operationId: get-invoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoices/{invoiceId}\n  method: put\n  operationId: update-invoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ach/withdraw\n  method: put\n  operationId: ach-withdraw\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ach/transactions\n  method: get\n  operationId: get-many-ach-transactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ach/transactions/{transactionId}\n  method: get\n  operationId: get-ach-transaction-by-id\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ach/transactions/{transactionId}/refund\n  method: put\n  operationId: ach-refund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ach/transactions/{transactionId}/void\n  method: put\n  operationId: ach-void\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ach/transactions/{transactionId}/cancel\n\
  \  method: patch\n  operationId: ach-cancel\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ach/batches\n  method: get\n  operationId: get-many-ach-batches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ach/batches/{batchId}/settle\n  method: put\n  operationId: ach-batch-settle\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /card-terminals\n  method: get\n  operationId: card-terminals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices\n  method: get\n  operationId: get-devices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices/{code}\n  method: get\n  operationId: get-device\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices/{code}/payment/purchase\n  method: post\n  operationId: start-purchase\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n     \
  \ triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /devices/{code}/payment/refund\n  method: post\n  operationId: start-refund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /devices/{code}/ping\n  method: get\n  operationId: ping-device\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/helcim/refs/heads/main/agentic-access/helcim-agentic-access.yml
summary_line: 48 operations · 25 acting
tags:
- Payments
- Canada
- Payment Gateway
- Payment Processing
- Acquiring
- Merchant Services
- ACH
- Invoicing
- Card Terminal
- Small Business
---
