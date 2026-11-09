---
acting_count: 0
action_class_counts:
  connected: 17
api_specs:
- filename: itau-unibanco-accounts-api-openapi.yml
  format: yaml
  label: Itaú Unibanco Accounts API
  slug: itau-unibanco-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itau-unibanco/openapi/itau-unibanco-accounts-api-openapi.yml
- filename: itau-unibanco-channels-api-openapi.yml
  format: yaml
  label: Itaú Unibanco Channels API
  slug: itau-unibanco-channels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itau-unibanco/openapi/itau-unibanco-channels-api-openapi.yml
- filename: itau-unibanco-credit-cards-api-openapi.yml
  format: yaml
  label: Itaú Unibanco Credit Cards API
  slug: itau-unibanco-credit-cards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itau-unibanco/openapi/itau-unibanco-credit-cards-api-openapi.yml
- filename: itau-unibanco-discovery-api-openapi.yml
  format: yaml
  label: Itaú Unibanco Discovery API
  slug: itau-unibanco-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itau-unibanco/openapi/itau-unibanco-discovery-api-openapi.yml
- filename: itau-unibanco-financings-api-openapi.yml
  format: yaml
  label: Itaú Unibanco Financings API
  slug: itau-unibanco-financings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itau-unibanco/openapi/itau-unibanco-financings-api-openapi.yml
- filename: itau-unibanco-invoice-financings-api-openapi.yml
  format: yaml
  label: Itaú Unibanco Invoice Financings API
  slug: itau-unibanco-invoice-financings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itau-unibanco/openapi/itau-unibanco-invoice-financings-api-openapi.yml
- filename: itau-unibanco-loans-api-openapi.yml
  format: yaml
  label: Itaú Unibanco Loans API
  slug: itau-unibanco-loans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itau-unibanco/openapi/itau-unibanco-loans-api-openapi.yml
- filename: itau-unibanco-unarranged-account-overdraft-api-openapi.yml
  format: yaml
  label: Itaú Unibanco Unarranged Account Overdraft API
  slug: itau-unibanco-unarranged-account-overdraft-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itau-unibanco/openapi/itau-unibanco-unarranged-account-overdraft-api-openapi.yml
consequence_counts:
  read: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Itau Unibanco Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'Itaú Unibanco exposes 17 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Itaú Unibanco
provider_slug: itau-unibanco
slug: itau-unibanco-agentic-access
source_filename: itau-unibanco-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: generated\nsource: openapi/itau-unibanco-open-finance-channels-openapi.yml, openapi/itau-unibanco-open-finance-common-openapi.yml,\n  openapi/itau-unibanco-open-finance-opendata-accounts-openapi.yml, openapi/itau-unibanco-open-finance-opendata-creditcards-openapi.yml,\n  openapi/itau-unibanco-open-finance-opendata-financings-openapi.yml, openapi/itau-unibanco-open-finance-opendata-invoicefinancings-openapi.yml,\n  openapi/itau-unibanco-open-finance-opendata-loans-openapi.yml, openapi/itau-unibanco-open-finance-opendata-unarranged-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 17\n  by_consequence:\n    read: 17\n  human_in_the_loop_required: 0\noperations:\n\
  - path: /banking-agents\n  method: get\n  operationId: getBankingAgents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /branches\n  method: get\n  operationId: getBranches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /electronic-channels\n  method: get\n  operationId: getElectronicChannels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /phone-channels\n  method: get\n  operationId: getPhoneChannels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /outages\n  method: get\n  operationId: getOutage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /personal-accounts\n  method: get\n  operationId: getPersonalAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /business-accounts\n  method: get\n  operationId: getBusinessAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /personal-credit-cards\n  method: get\n  operationId: getPersonalCreditCards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /business-credit-cards\n\
  \  method: get\n  operationId: getBusinessCreditCards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /personal-financings\n  method: get\n  operationId: getPersonalFinancings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /business-financings\n  method: get\n  operationId: getBusinessFinancings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /business-invoice-financings\n  method: get\n  operationId: getBusinessInvoiceFinancings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /personal-loans\n  method: get\n  operationId: getPersonalLoans\n  x-agentic-access:\n  \
  \  action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /business-loans\n  method: get\n  operationId: getBusinessLoans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /personal-unarranged-account-overdraft\n  method: get\n  operationId: getPersonalUnarrangedAccountOverdraft\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /business-unarranged-account-overdraft\n  method: get\n  operationId: getBusinessUnarrangedAccountOverdraft\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/itau-unibanco/agentic-access/itau-unibanco-agentic-access.yml
summary_line: 17 operations
tags:
- Company
- Banking
- Financial Services
- Payments
- Pix
- Open Finance
- Brazil
- Foreign Exchange
- Credit
---
