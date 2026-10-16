---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 18
api_specs:
- filename: clarafintech-accounts-payable-api-openapi.yml
  format: yaml
  label: Clarafintech Accounts Payable API
  slug: clarafintech-accounts-payable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarafintech/refs/heads/main/openapi/clarafintech-accounts-payable-api-openapi.yml
- filename: clarafintech-authentication-api-openapi.yml
  format: yaml
  label: Clarafintech Authentication API
  slug: clarafintech-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarafintech/refs/heads/main/openapi/clarafintech-authentication-api-openapi.yml
- filename: clarafintech-billing-statements-api-openapi.yml
  format: yaml
  label: Clarafintech Billing Statements API
  slug: clarafintech-billing-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarafintech/refs/heads/main/openapi/clarafintech-billing-statements-api-openapi.yml
- filename: clarafintech-cards-api-openapi.yml
  format: yaml
  label: Clarafintech Cards API
  slug: clarafintech-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarafintech/refs/heads/main/openapi/clarafintech-cards-api-openapi.yml
- filename: clarafintech-digital-account-api-openapi.yml
  format: yaml
  label: Clarafintech Digital Account API
  slug: clarafintech-digital-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarafintech/refs/heads/main/openapi/clarafintech-digital-account-api-openapi.yml
- filename: clarafintech-extracted-documents-api-openapi.yml
  format: yaml
  label: Clarafintech Extracted Documents API
  slug: clarafintech-extracted-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarafintech/refs/heads/main/openapi/clarafintech-extracted-documents-api-openapi.yml
- filename: clarafintech-invoices-api-openapi.yml
  format: yaml
  label: Clarafintech Invoices API
  slug: clarafintech-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarafintech/refs/heads/main/openapi/clarafintech-invoices-api-openapi.yml
- filename: clarafintech-reimbursements-api-openapi.yml
  format: yaml
  label: Clarafintech Reimbursements API
  slug: clarafintech-reimbursements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarafintech/refs/heads/main/openapi/clarafintech-reimbursements-api-openapi.yml
- filename: clarafintech-transactions-api-openapi.yml
  format: yaml
  label: Clarafintech Transactions API
  slug: clarafintech-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarafintech/refs/heads/main/openapi/clarafintech-transactions-api-openapi.yml
- filename: clarafintech-users-api-openapi.yml
  format: yaml
  label: Clarafintech Users API
  slug: clarafintech-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarafintech/refs/heads/main/openapi/clarafintech-users-api-openapi.yml
consequence_counts:
  physical: 2
  read: 18
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Clarafintech Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v3/accounts-payable/pix
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/v3/accounts-payable/pix/{externalId}
operation_count: 29
overview: 'Clarafintech exposes 29 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read, 9 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Clarafintech
provider_slug: clarafintech
slug: clarafintech-agentic-access
source_filename: clarafintech-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: generated\nsource: openapi/clarafintech-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 29\n  by_action_class:\n    acting: 11\n    connected: 18\n  by_consequence:\n    write: 9\n    read: 18\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /oauth/token\n  method: post\n  operationId: createOAuthToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v3/cards\n  method: get\n  operationId: listCardsV3\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/cards\n  method: post\n  operationId: createCardV3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v3/cards/{uuid}\n  method: get\n  operationId: getCardV3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/cards/{uuid}\n  method: delete\n  operationId: deleteCardV3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/v3/cards/{uuid}/lock\n  method: patch\n  operationId: setCardLockV3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v3/cards/{uuid}/threshold\n  method: patch\n  operationId: updateCardThresholdV3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v3/transactions\n  method: get\n  operationId: listTransactionsV3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/transactions/{uuid}\n\
  \  method: get\n  operationId: getTransactionV3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/transactions/{uuid}/documents\n  method: get\n  operationId: listTransactionDocumentsV3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/users\n  method: get\n  operationId: listUsersV3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/users\n  method: post\n  operationId: createUserV3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/v3/users/{uuid}\n  method: get\n  operationId: getUserV3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/users/{uuid}\n  method: patch\n  operationId: updateUserV3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v3/users/{uuid}\n  method: delete\n  operationId: deleteUserV3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v3/transactions/labels/bulk\n  method: post\n  operationId: bulkBindTransactionLabelsV3\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v3/transactions/{uuid}/invoices\n  method: get\n  operationId: listTransactionInvoicesV3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/invoices\n  method: get\n  operationId: listInvoicesV3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/transactions/{uuid}/extracted-documents\n  method: get\n  operationId: listTransactionExtractedDocumentsV3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n \
  \   audit: none\n- path: /api/v3/reimbursements\n  method: get\n  operationId: listReimbursementsV3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/reimbursements/{uuid}\n  method: get\n  operationId: getReimbursementV3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/billing-statements\n  method: get\n  operationId: listBillingStatementsV3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/billing-statements/{uuid}/transactions\n  method: get\n  operationId: listBillingStatementTransactionsV3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/digital-accounts\n\
  \  method: get\n  operationId: listDigitalAccountTransactionsV3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/accounts-payable/pix\n  method: post\n  operationId: createPixPaymentV3\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v3/accounts-payable/pix/{externalId}\n  method: delete\n  operationId: cancelPixPaymentV3\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/v3/accounts-payable/{externalId}\n  method: get\n  operationId: getAccountsPayablePaymentV3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/accounts-payable\n  method: get\n  operationId: listAccountsPayablePaymentsV3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/digital-accounts/balance\n  method: get\n  operationId: getDigitalAccountBalanceV3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clarafintech/refs/heads/main/agentic-access/clarafintech-agentic-access.yml
summary_line: 29 operations · 11 acting
tags:
- Fintech
- Spend Management
- Latin America
- Corporate Cards
- Financial Automation
- Company
---
