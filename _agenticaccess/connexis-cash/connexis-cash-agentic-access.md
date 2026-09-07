---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 9
api_specs:
- filename: connexis-cash-account-information-psd2-stet-mock-openapi.yml
  format: yaml
  label: Connexis Cash PSD2 Account Information API (STET)
  slug: psd2-account-information
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/connexis-cash/refs/heads/main/openapi/connexis-cash-account-information-psd2-stet-mock-openapi.yml
- filename: connexis-cash-accounts-api-openapi.yml
  format: yaml
  label: Connexis Cash Accounts API
  slug: connexis-cash-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/connexis-cash/refs/heads/main/openapi/connexis-cash-accounts-api-openapi.yml
- filename: connexis-cash-balances-api-openapi.yml
  format: yaml
  label: Connexis Cash Balances API
  slug: connexis-cash-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/connexis-cash/refs/heads/main/openapi/connexis-cash-balances-api-openapi.yml
- filename: connexis-cash-beneficiaries-api-openapi.yml
  format: yaml
  label: Connexis Cash Beneficiaries API
  slug: connexis-cash-beneficiaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/connexis-cash/refs/heads/main/openapi/connexis-cash-beneficiaries-api-openapi.yml
- filename: connexis-cash-consents-api-openapi.yml
  format: yaml
  label: Connexis Cash Consents API
  slug: connexis-cash-consents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/connexis-cash/refs/heads/main/openapi/connexis-cash-consents-api-openapi.yml
- filename: connexis-cash-transactions-api-openapi.yml
  format: yaml
  label: Connexis Cash Transactions API
  slug: connexis-cash-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/connexis-cash/refs/heads/main/openapi/connexis-cash-transactions-api-openapi.yml
consequence_counts:
  read: 9
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Connexis Cash Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'Connexis Cash exposes 10 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Connexis Cash
provider_slug: connexis-cash
slug: connexis-cash-agentic-access
source_filename: connexis-cash-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: generated\nsource: openapi/connexis-cash-account-information-psd2-stet-mock-openapi.yml, openapi/connexis-cash-accounts-api-openapi.yml,\n  openapi/connexis-cash-balances-api-openapi.yml, openapi/connexis-cash-beneficiaries-api-openapi.yml,\n  openapi/connexis-cash-consents-api-openapi.yml, openapi/connexis-cash-transactions-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 9\n    acting: 1\n  by_consequence:\n    read: 9\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/accounts\n  method: get\n  operationId: accountsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    -\
  \ aisp\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{accountResourceId}/balances\n  method: get\n  operationId: accountsBalancesGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - aisp\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{accountResourceId}/transactions\n  method: get\n  operationId: accountsTransactionsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - aisp\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/trusted-beneficiaries\n  method: get\n  operationId: trustedBeneficiariesGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - aisp\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - aisp\n- path: /v1/accounts/{accountResourceId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - aisp\n- path: /v1/accounts/{accountResourceId}/balances\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - aisp\n- path: /v1/trusted-beneficiaries\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - aisp\n- path: /v1/consents\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n  \
  \    triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - aisp\n- path: /v1/accounts/{accountResourceId}/transactions\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - aisp\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/connexis-cash/refs/heads/main/agentic-access/connexis-cash-agentic-access.yml
summary_line: 10 operations · 1 acting
tags:
- Account Information
- BNP Paribas
- Cash Management
- Corporate Banking
- Digital Banking
- Liquidity Management
- Open Banking
- Payments
- PSD2
- SCA
- STET
---
