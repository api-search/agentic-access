---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 21
api_specs:
- filename: kanmon-bank-accounts-api-openapi.yml
  format: yaml
  label: Kanmon Bank Accounts API
  slug: kanmon-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/openapi/kanmon-bank-accounts-api-openapi.yml
- filename: kanmon-businesses-api-openapi.yml
  format: yaml
  label: Kanmon Businesses API
  slug: kanmon-businesses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/openapi/kanmon-businesses-api-openapi.yml
- filename: kanmon-connect-tokens-api-openapi.yml
  format: yaml
  label: Kanmon Connect Tokens API
  slug: kanmon-connect-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/openapi/kanmon-connect-tokens-api-openapi.yml
- filename: kanmon-documents-api-openapi.yml
  format: yaml
  label: Kanmon Documents API
  slug: kanmon-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/openapi/kanmon-documents-api-openapi.yml
- filename: kanmon-draw-requests-api-openapi.yml
  format: yaml
  label: Kanmon Draw Requests API
  slug: kanmon-draw-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/openapi/kanmon-draw-requests-api-openapi.yml
- filename: kanmon-embedded-sessions-api-openapi.yml
  format: yaml
  label: Kanmon Embedded Sessions API
  slug: kanmon-embedded-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/openapi/kanmon-embedded-sessions-api-openapi.yml
- filename: kanmon-integrated-mca-api-openapi.yml
  format: yaml
  label: Kanmon Integrated MCA API
  slug: kanmon-integrated-mca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/openapi/kanmon-integrated-mca-api-openapi.yml
- filename: kanmon-invoices-api-openapi.yml
  format: yaml
  label: Kanmon Invoices API
  slug: kanmon-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/openapi/kanmon-invoices-api-openapi.yml
- filename: kanmon-issued-products-api-openapi.yml
  format: yaml
  label: Kanmon Issued Products API
  slug: kanmon-issued-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/openapi/kanmon-issued-products-api-openapi.yml
- filename: kanmon-offers-api-openapi.yml
  format: yaml
  label: Kanmon Offers API
  slug: kanmon-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/openapi/kanmon-offers-api-openapi.yml
- filename: kanmon-payments-api-openapi.yml
  format: yaml
  label: Kanmon Payments API
  slug: kanmon-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/openapi/kanmon-payments-api-openapi.yml
- filename: kanmon-prequalifications-api-openapi.yml
  format: yaml
  label: Kanmon Prequalifications API
  slug: kanmon-prequalifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/openapi/kanmon-prequalifications-api-openapi.yml
- filename: kanmon-sandbox-utilities-api-openapi.yml
  format: yaml
  label: Kanmon Sandbox Utilities API
  slug: kanmon-sandbox-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/openapi/kanmon-sandbox-utilities-api-openapi.yml
- filename: kanmon-users-api-openapi.yml
  format: yaml
  label: Kanmon Users API
  slug: kanmon-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/openapi/kanmon-users-api-openapi.yml
consequence_counts:
  physical: 1
  read: 21
  safety-critical: 1
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Kanmon Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/platform/v2/sandbox/businesses/{id}/reset
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/platform/v2/invoices/finance
operation_count: 35
overview: 'Kanmon exposes 35 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read, 12 write, 1 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Kanmon
provider_slug: kanmon
slug: kanmon-agentic-access
source_filename: kanmon-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/kanmon-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 35\n  by_action_class:\n    connected: 21\n    acting: 14\n  by_consequence:\n    read: 21\n    write: 12\n    physical: 1\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /api/platform/v2/prequalifications\n  method: get\n  operationId: getAllPrequalifiedBusinesses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/platform/v2/businesses\n  method: get\n  operationId: getAllBusinesses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/platform/v2/businesses\n  method: post\n  operationId: createBusiness\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/platform/v2/businesses/{id}\n  method: get\n  operationId: getBusiness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/platform/v2/businesses/{id}\n  method: patch\n  operationId: updateBusiness\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/platform/v2/businesses/{id}/activity-logs\n  method: get\n  operationId: getBusinessActivityLog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/platform/v2/users\n  method: get\n  operationId: getAllUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/platform/v2/users\n  method: post\n  operationId: createUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/platform/v2/users/{id}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/platform/v2/users/{id}\n  method: patch\n  operationId: updateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/platform/v2/users/merge\n  method: post\n  operationId: mergeUserIntoBusiness\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/platform/v2/connect-tokens\n  method: post\n  operationId: createConnectToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/platform/v2/invoices/{id}\n  method: get\n  operationId: getInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/platform/v2/invoices\n  method: get\n  operationId: getAllInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/platform/v2/invoices/finance\n  method: post\n  operationId: financeInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/platform/v2/offers/{id}\n  method: get\n  operationId: getOfferById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/platform/v2/offers\n  method: get\n  operationId: getAllOffers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/platform/v2/issued-products/{id}\n  method: get\n  operationId: getIssuedProductById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/platform/v2/issued-products\n  method: get\n  operationId: getAllIssuedProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/platform/v2/bank-accounts\n\
  \  method: get\n  operationId: getAllBusinessBankAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/platform/v2/bank-accounts\n  method: post\n  operationId: createBusinessBankAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/platform/v2/bank-accounts/{id}\n  method: get\n  operationId: getBusinessBankAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/platform/v2/bank-accounts/{id}\n  method: patch\n  operationId: updateBusinessBankAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/platform/v2/payments/{id}\n  method: get\n  operationId: getPaymentById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/platform/v2/issued-products/{id}/payment-schedule\n  method: get\n  operationId: getPaymentScheduleForAIssuedProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/platform/v2/payment-intents\n  method: get\n  operationId: getPaymentIntents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/platform/v2/draw-requests/{id}\n \
  \ method: get\n  operationId: getDrawRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/platform/v2/draw-requests\n  method: get\n  operationId: getAllDrawRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/platform/v2/documents\n  method: post\n  operationId: createBusinessDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/platform/v2/integrated-mca-receivables\n  method: get\n  operationId: getReceivables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/platform/v2/integrated-mca-receivables\n  method: post\n  operationId: createIntegratedMcaReceivable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/platform/v2/issued-products/{id}/integrated-mca-payment-windows\n  method: get\n  operationId: getIntegratedMcaPaymentWindows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/platform/v2/sandbox/businesses/{id}/reset\n  method: post\n  operationId: sandboxResetBusiness\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n\
  \      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/platform/v2/sandbox/businesses/{id}/delete\n  method: delete\n  operationId: sandboxDeleteBusiness\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/platform/v2/embedded-session\n  method: post\n  operationId: createEmbeddedSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kanmon/refs/heads/main/agentic-access/kanmon-agentic-access.yml
summary_line: 35 operations · 14 acting · 1 human-in-the-loop
tags:
- Company
- Fintech
- Embedded Finance
- Embedded Lending
- Lending
- Working Capital
- Invoice Financing
---
