---
acting_count: 16
action_class_counts:
  acting: 16
  connected: 17
api_specs:
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto Business API
  slug: qonto-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto Transactions & Statements API
  slug: qonto-transactions-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto SEPA Transfers API
  slug: qonto-sepa-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto International Transfers API
  slug: qonto-international-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto Internal Transfers API
  slug: qonto-internal-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto Cards API
  slug: qonto-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto Client Invoices & Quotes API
  slug: qonto-client-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto Supplier Invoices API
  slug: qonto-supplier-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto SEPA Direct Debit API
  slug: qonto-sepa-direct-debit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto Payment Links API
  slug: qonto-payment-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto Terminals API
  slug: qonto-terminals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto Webhooks API
  slug: qonto-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto Onboarding API
  slug: qonto-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto Embed SDK & Hosted Pages API
  slug: qonto-embed-sdk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
consequence_counts:
  read: 17
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the modeled OpenAPI. A governance starting point for exposing this business-banking API to AI agents - review and bind audience per deployment. Money-movement operations (SEPA/internal/international transfers, SDD collection mandates, card issuance, terminal payments) are marked human-in-the-loop required because they move real funds and are subject to PSD2 Strong Customer Authentication (SCA). See research/curity/agentic-governance/.
human_in_the_loop: 7
kind: agentic-access
layout: agentic-access
method: generated
name: Qonto Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 33
overview: 'Qonto exposes 33 API operations that an AI agent could call, of which 16 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read and 16 write.


  7 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Qonto
provider_slug: qonto
slug: qonto-agentic-access
source_filename: qonto-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: generated\nsource: openapi/qonto-openapi.yml\ndescription: >-\n  Recommended x-agentic-access execution contracts, classified heuristically from\n  the modeled OpenAPI. A governance starting point for exposing this business-banking\n  API to AI agents - review and bind audience per deployment. Money-movement\n  operations (SEPA/internal/international transfers, SDD collection mandates, card\n  issuance, terminal payments) are marked human-in-the-loop required because they\n  move real funds and are subject to PSD2 Strong Customer Authentication (SCA).\n  See research/curity/agentic-governance/.\nsummary:\n  operations: 33\n  by_action_class:\n    acting: 16\n    connected: 17\n  by_consequence:\n    write: 16\n    read: 17\n  human_in_the_loop_required: 7\noperations:\n- path: /oauth2/token\n  method: post\n  operationId: createOrRefreshTokens\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n   \
  \ audience: null\n    token:\n      max-ttl: 3600\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    audit: required\n- path: /v2/organization\n  method: get\n  operationId: getOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/memberships\n  method: get\n  operationId: listMemberships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/memberships\n  method: post\n  operationId: createMembership\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/labels\n  method: get\n  operationId:\
  \ listLabels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/teams\n  method: get\n  operationId: listTeams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/teams\n  method: post\n  operationId: createTeam\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    audit: required\n- path: /v2/transactions\n  method: get\n  operationId: listTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/transactions/{id}\n  method: get\n  operationId: getTransaction\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/statements\n  method: get\n  operationId: listStatements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/cards\n  method: get\n  operationId: listCards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/cards\n  method: post\n  operationId: createCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - always\n    audit: required\n- path: /v2/sepa/transfers\n  method: get\n  operationId: listSepaTransfers\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/sepa/transfers\n  method: post\n  operationId: createSepaTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - always\n    sca: required\n    audit: required\n- path: /v2/sepa/bulk_transfers\n  method: post\n  operationId: createSepaBulkTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - always\n    sca: required\n    audit: required\n- path: /v2/beneficiaries\n  method: get\n  operationId: listBeneficiaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v2/internal_transfers\n  method: post\n  operationId: createInternalTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - always\n    audit: required\n- path: /v2/international_transfers/currencies\n  method: get\n  operationId: listInternationalCurrencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/international_transfers\n  method: post\n  operationId: createInternationalTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - always\n    sca: required\n    audit: required\n- path: /v2/client_invoices\n  method:\
  \ get\n  operationId: listClientInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/client_invoices\n  method: post\n  operationId: createClientInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/supplier_invoices\n  method: get\n  operationId: listSupplierInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/supplier_invoices\n  method: post\n  operationId: createSupplierInvoices\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/attachments\n  method: post\n  operationId: uploadAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    audit: required\n- path: /v2/sepa/direct_debit_collections/mandates\n  method: post\n  operationId: createSddMandate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - always\n    audit: required\n- path: /v2/sepa/direct_debit_collections\n  method: get\n  operationId: listSddCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/payment_links\n  method: get\n  operationId: listPaymentLinks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/payment_links\n  method: post\n  operationId: createPaymentLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/terminals\n  method: get\n  operationId: listTerminals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/terminal_payments\n  method: post\n  operationId: createTerminalPayment\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - always\n    audit: required\n- path: /v2/webhook_subscriptions\n  method: get\n  operationId: listWebhookSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/webhook_subscriptions\n  method: post\n  operationId: createWebhookSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    audit: required\n- path: /v2/webhook_subscriptions/{id}\n  method: delete\n  operationId: deleteWebhookSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/agentic-access/qonto-agentic-access.yml
summary_line: 33 operations · 16 acting · 7 human-in-the-loop
tags:
- Business Banking
- Neobank
- Fintech
- Payments
- SEPA
- Open Banking
- EUR
- Europe
---
