---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 6
api_specs:
- filename: algbra-accounts-api-openapi.yml
  format: yaml
  label: Algbra Accounts API
  slug: algbra-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algbra/openapi/algbra-accounts-api-openapi.yml
- filename: algbra-transactions-api-openapi.yml
  format: yaml
  label: Algbra Transactions API
  slug: algbra-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algbra/openapi/algbra-transactions-api-openapi.yml
- filename: algbra-automated-payments-api-openapi.yml
  format: yaml
  label: Algbra Automated Payments API
  slug: algbra-automated-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algbra/openapi/algbra-automated-payments-api-openapi.yml
- filename: algbra-cards-api-openapi.yml
  format: yaml
  label: Algbra Cards API
  slug: algbra-cards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algbra/openapi/algbra-cards-api-openapi.yml
- filename: algbra-compliance-api-openapi.yml
  format: yaml
  label: Algbra Compliance API
  slug: algbra-compliance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algbra/openapi/algbra-compliance-api-openapi.yml
- filename: algbra-customers-api-openapi.yml
  format: yaml
  label: Algbra Customers API
  slug: algbra-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algbra/openapi/algbra-customers-api-openapi.yml
- filename: algbra-investments-api-openapi.yml
  format: yaml
  label: Algbra Investments API
  slug: algbra-investments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algbra/openapi/algbra-investments-api-openapi.yml
- filename: algbra-onboarding-prospects-business-api-openapi.yml
  format: yaml
  label: Algbra Onboarding Prospects - Business API
  slug: algbra-onboarding-prospects-business-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algbra/openapi/algbra-onboarding-prospects-business-api-openapi.yml
- filename: algbra-onboarding-prospects-personal-api-openapi.yml
  format: yaml
  label: Algbra Onboarding Prospects - Personal API
  slug: algbra-onboarding-prospects-personal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algbra/openapi/algbra-onboarding-prospects-personal-api-openapi.yml
- filename: algbra-partner-api-openapi.yml
  format: yaml
  label: Algbra Partner API
  slug: algbra-partner-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algbra/openapi/algbra-partner-api-openapi.yml
- filename: algbra-partners-api-openapi.yml
  format: yaml
  label: Algbra Partners API
  slug: algbra-partners-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algbra/openapi/algbra-partners-api-openapi.yml
- filename: algbra-payment-simulations-api-openapi.yml
  format: yaml
  label: Algbra Payment Simulations API
  slug: algbra-payment-simulations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algbra/openapi/algbra-payment-simulations-api-openapi.yml
- filename: algbra-payments-api-openapi.yml
  format: yaml
  label: Algbra Payments API
  slug: algbra-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algbra/openapi/algbra-payments-api-openapi.yml
consequence_counts:
  read: 6
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Algbra Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Algbra exposes 8 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Algbra
provider_slug: algbra
slug: algbra-agentic-access
source_filename: algbra-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: generated\nsource: openapi/algbra-account-transaction-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 2\n    connected: 6\n  by_consequence:\n    write: 2\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /account-access-consents\n  method: post\n  operationId: CreateAccountAccessConsents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account-access-consents/{ConsentId}\n  method:\
  \ get\n  operationId: GetAccountAccessConsentsConsentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account-access-consents/{ConsentId}\n  method: delete\n  operationId: DeleteAccountAccessConsentsConsentId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts\n  method: get\n  operationId: GetAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{AccountId}\n  method: get\n  operationId: GetAccountsAccountId\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{AccountId}/balances\n  method: get\n  operationId: GetAccountsAccountIdBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{AccountId}/beneficiaries\n  method: get\n  operationId: GetAccountsAccountIdBeneficiaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{AccountId}/transactions\n  method: get\n  operationId: GetAccountsAccountIdTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/algbra/agentic-access/algbra-agentic-access.yml
summary_line: 8 operations · 2 acting
tags:
- Financial Services
- Banking
- Open Banking
- PSD2
- OBIE
- United Kingdom
- Payments
- Account Information
- Fintech
- Ethical Finance
- Banking as a Service
---
