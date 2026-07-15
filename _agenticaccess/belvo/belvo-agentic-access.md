---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 18
api_specs:
- filename: belvo-openapi.yml
  format: yaml
  label: Belvo Links API
  slug: belvo-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/belvo/refs/heads/main/openapi/belvo-openapi.yml
- filename: belvo-openapi.yml
  format: yaml
  label: Belvo Accounts API
  slug: belvo-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/belvo/refs/heads/main/openapi/belvo-openapi.yml
- filename: belvo-openapi.yml
  format: yaml
  label: Belvo Transactions & Balances API
  slug: belvo-transactions-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/belvo/refs/heads/main/openapi/belvo-openapi.yml
- filename: belvo-openapi.yml
  format: yaml
  label: Belvo Owners & Incomes API
  slug: belvo-owners-incomes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/belvo/refs/heads/main/openapi/belvo-openapi.yml
- filename: belvo-openapi.yml
  format: yaml
  label: Belvo Institutions API
  slug: belvo-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/belvo/refs/heads/main/openapi/belvo-openapi.yml
- filename: belvo-openapi.yml
  format: yaml
  label: Belvo Payments (Brazil / Pix) API
  slug: belvo-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/belvo/refs/heads/main/openapi/belvo-openapi.yml
- filename: belvo-openapi.yml
  format: yaml
  label: Belvo Webhooks API
  slug: belvo-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/belvo/refs/heads/main/openapi/belvo-openapi.yml
consequence_counts:
  physical: 2
  read: 18
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Belvo Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/br/customers/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/br/payment-intents/
operation_count: 32
overview: 'Belvo exposes 32 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read, 12 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Belvo
provider_slug: belvo
slug: belvo-agentic-access
source_filename: belvo-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/belvo-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 32\n  by_action_class:\n    connected: 18\n    acting: 14\n  by_consequence:\n    read: 18\n    write: 12\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/links/\n  method: get\n  operationId: listLinks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/links/\n  method: post\n  operationId: registerLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/links/{id}/\n  method: get\n  operationId: detailLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/links/{id}/\n  method: patch\n  operationId: patchLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/links/{id}/\n  method: delete\n  operationId: deleteLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/accounts/\n  method: get\n  operationId: listAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/\n  method: post\n  operationId: retrieveAccounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{id}/\n  method: get\n  operationId: detailAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{id}/\n  method: delete\n  operationId: deleteAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/transactions/\n  method: get\n  operationId: listTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/transactions/\n  method: post\n  operationId: retrieveTransactions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/transactions/{id}/\n  method: get\n  operationId: detailTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/balances/\n  method: get\n  operationId:\
  \ listBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/balances/\n  method: post\n  operationId: retrieveBalances\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/owners/\n  method: get\n  operationId: listOwners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/owners/\n  method: post\n  operationId: retrieveOwners\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/incomes/\n  method: get\n  operationId: listIncomes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/incomes/\n  method: post\n  operationId: retrieveIncomes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/recurring-expenses/\n  method: get\n  operationId: listRecurringExpenses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/recurring-expenses/\n  method: post\n  operationId: retrieveRecurringExpenses\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/institutions/\n  method: get\n  operationId: listInstitutions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/institutions/{id}/\n  method: get\n  operationId: detailInstitution\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/webhooks/\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/webhooks/\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/webhooks/{id}/\n  method: get\n  operationId: detailWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/webhooks/{id}/\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/br/payment-intents/\n  method: get\n  operationId: listPaymentIntents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /payments/br/payment-intents/\n  method: post\n  operationId: createPaymentIntent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/br/payment-intents/{id}/\n  method: get\n  operationId: detailPaymentIntent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/br/customers/\n  method: get\n  operationId: listCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/br/customers/\n  method: post\n  operationId: createCustomer\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/br/payment-institutions/\n  method: get\n  operationId: listPaymentInstitutions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/belvo/refs/heads/main/agentic-access/belvo-agentic-access.yml
summary_line: 32 operations · 14 acting
tags:
- Open Finance
- Open Banking
- Bank Data
- Aggregation
- Payments
- Pix
- Latin America
---
