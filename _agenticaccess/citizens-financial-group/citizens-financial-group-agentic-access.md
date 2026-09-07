---
acting_count: 0
action_class_counts:
  connected: 4
api_specs:
- filename: citizens-financial-group-accounts-openapi.yml
  format: yaml
  label: Citizens Accounts API
  slug: citizens-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citizens-financial-group/refs/heads/main/openapi/citizens-financial-group-accounts-openapi.yml
- filename: citizens-financial-group-statements-openapi.yml
  format: yaml
  label: Citizens Statements API
  slug: citizens-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citizens-financial-group/refs/heads/main/openapi/citizens-financial-group-statements-openapi.yml
- filename: citizens-financial-group-payments-openapi.yml
  format: yaml
  label: Citizens Payments API
  slug: citizens-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citizens-financial-group/refs/heads/main/openapi/citizens-financial-group-payments-openapi.yml
- filename: citizens-financial-group-account-validation-openapi.yml
  format: yaml
  label: Citizens Account Validation API
  slug: citizens-account-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citizens-financial-group/refs/heads/main/openapi/citizens-financial-group-account-validation-openapi.yml
- filename: citizens-financial-group-account-transfer-openapi.yml
  format: yaml
  label: Citizens Account Transfer API
  slug: citizens-account-transfer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citizens-financial-group/refs/heads/main/openapi/citizens-financial-group-account-transfer-openapi.yml
- filename: citizens-financial-group-information-reporting-openapi.yml
  format: yaml
  label: Citizens Information Reporting API
  slug: citizens-information-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citizens-financial-group/refs/heads/main/openapi/citizens-financial-group-information-reporting-openapi.yml
- filename: citizens-financial-group-authorize-openapi.yml
  format: yaml
  label: Citizens Authorize API
  slug: citizens-authorize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citizens-financial-group/refs/heads/main/openapi/citizens-financial-group-authorize-openapi.yml
- filename: citizens-financial-group-atm-locator-openapi.yml
  format: yaml
  label: Citizens ATM Locator API
  slug: citizens-atm-locator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citizens-financial-group/refs/heads/main/openapi/citizens-financial-group-atm-locator-openapi.yml
- filename: citizens-financial-group-branch-locator-openapi.yml
  format: yaml
  label: Citizens Branch Locator API
  slug: citizens-branch-locator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citizens-financial-group/refs/heads/main/openapi/citizens-financial-group-branch-locator-openapi.yml
consequence_counts:
  read: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Citizens Financial Group Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'Citizens Financial Group exposes 4 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Citizens Financial Group
provider_slug: citizens-financial-group
slug: citizens-financial-group-agentic-access
source_filename: citizens-financial-group-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/citizens-bank-accounts-api-openapi.yml, openapi/citizens-bank-atm-locator-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    connected: 4\n  by_consequence:\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /accounts\n  method: get\n  operationId: getAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}\n  method: get\n  operationId: getAccountById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /accounts/{accountId}/transactions\n  method: get\n  operationId: getTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /atms\n  method: get\n  operationId: searchATMs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/citizens-financial-group/refs/heads/main/agentic-access/citizens-financial-group-agentic-access.yml
summary_line: 4 operations
tags:
- Banking
- Buy Now Pay Later
- Financial-Services
- FDX
- Locator
- Open Banking
- Payments
---
