---
acting_count: 27
action_class_counts:
  acting: 27
  connected: 24
api_specs:
- filename: weel-accounting-codes-api-openapi.yml
  format: yaml
  label: Weel Accounting Codes API
  slug: weel-accounting-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weel/refs/heads/main/openapi/weel-accounting-codes-api-openapi.yml
- filename: weel-budget-members-api-openapi.yml
  format: yaml
  label: Weel Budget Members API
  slug: weel-budget-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weel/refs/heads/main/openapi/weel-budget-members-api-openapi.yml
- filename: weel-budget-owners-api-openapi.yml
  format: yaml
  label: Weel Budget Owners API
  slug: weel-budget-owners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weel/refs/heads/main/openapi/weel-budget-owners-api-openapi.yml
- filename: weel-budget-topups-api-openapi.yml
  format: yaml
  label: Weel Budget Topups API
  slug: weel-budget-topups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weel/refs/heads/main/openapi/weel-budget-topups-api-openapi.yml
- filename: weel-budgets-api-openapi.yml
  format: yaml
  label: Weel Budgets API
  slug: weel-budgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weel/refs/heads/main/openapi/weel-budgets-api-openapi.yml
- filename: weel-categories-api-openapi.yml
  format: yaml
  label: Weel Categories API
  slug: weel-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weel/refs/heads/main/openapi/weel-categories-api-openapi.yml
- filename: weel-custom-field-budgets-api-openapi.yml
  format: yaml
  label: Weel Custom Field Budgets API
  slug: weel-custom-field-budgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weel/refs/heads/main/openapi/weel-custom-field-budgets-api-openapi.yml
- filename: weel-custom-field-options-api-openapi.yml
  format: yaml
  label: Weel Custom Field Options API
  slug: weel-custom-field-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weel/refs/heads/main/openapi/weel-custom-field-options-api-openapi.yml
- filename: weel-custom-fields-api-openapi.yml
  format: yaml
  label: Weel Custom Fields API
  slug: weel-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weel/refs/heads/main/openapi/weel-custom-fields-api-openapi.yml
- filename: weel-invites-api-openapi.yml
  format: yaml
  label: Weel Invites API
  slug: weel-invites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weel/refs/heads/main/openapi/weel-invites-api-openapi.yml
- filename: weel-roles-api-openapi.yml
  format: yaml
  label: Weel Roles API
  slug: weel-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weel/refs/heads/main/openapi/weel-roles-api-openapi.yml
- filename: weel-statements-api-openapi.yml
  format: yaml
  label: Weel Statements API
  slug: weel-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weel/refs/heads/main/openapi/weel-statements-api-openapi.yml
- filename: weel-tax-rates-api-openapi.yml
  format: yaml
  label: Weel Tax Rates API
  slug: weel-tax-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weel/refs/heads/main/openapi/weel-tax-rates-api-openapi.yml
- filename: weel-transactions-api-openapi.yml
  format: yaml
  label: Weel Transactions API
  slug: weel-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weel/refs/heads/main/openapi/weel-transactions-api-openapi.yml
- filename: weel-users-api-openapi.yml
  format: yaml
  label: Weel Users API
  slug: weel-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weel/refs/heads/main/openapi/weel-users-api-openapi.yml
consequence_counts:
  read: 24
  write: 27
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Weel Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 51
overview: 'Weel exposes 51 API operations that an AI agent could call, of which 27 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 24 read and 27 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Weel
provider_slug: weel
slug: weel-agentic-access
source_filename: weel-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: generated\nsource: openapi/weel-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 51\n  by_action_class:\n    connected: 24\n    acting: 27\n  by_consequence:\n    read: 24\n    write: 27\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/businesses/{client_id}/transactions\n  method: get\n  operationId: listTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/businesses/{client_id}/transactions/{transaction_id}\n  method: get\n  operationId: getTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/businesses/{client_id}/statements\n  method: get\n  operationId: listStatements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/businesses/{client_id}/users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/businesses/{client_id}/roles\n  method: get\n  operationId: listRoles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/businesses/{client_id}/users/{user_id}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/businesses/{client_id}/users/{user_id}\n\
  \  method: patch\n  operationId: updateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/businesses/{client_id}/users/{user_id}\n  method: delete\n  operationId: deleteUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/businesses/{client_id}/invites\n  method: get\n  operationId: listInvites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/businesses/{client_id}/invites\n  method: post\n  operationId:\
  \ createInvite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/businesses/{client_id}/invites/{invite_id}\n  method: delete\n  operationId: cancelInvite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/businesses/{client_id}/users/{user_id}/budget-members\n  method: get\n  operationId: listBudgetMembersByUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/businesses/{client_id}/budgets\n  method: get\n\
  \  operationId: listBudgets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/businesses/{client_id}/budgets\n  method: post\n  operationId: createBudget\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/businesses/{client_id}/budgets/{budget_id}\n  method: get\n  operationId: getBudget\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/businesses/{client_id}/budgets/{budget_id}\n  method: patch\n  operationId: updateBudget\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/businesses/{client_id}/budgets/{budget_id}\n  method: delete\n  operationId: deleteBudget\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/businesses/{client_id}/budgets/{budget_id}/topups\n  method: get\n  operationId: listBudgetTopups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/businesses/{client_id}/budgets/{budget_id}/topups\n  method: post\n  operationId: createBudgetTopup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/businesses/{client_id}/budgets/{budget_id}/members\n  method: get\n  operationId: listBudgetMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/businesses/{client_id}/budgets/{budget_id}/members\n  method: post\n  operationId: createBudgetMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/businesses/{client_id}/budgets/{budget_id}/members/{budget_member_id}\n  method: get\n  operationId: getBudgetMember\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/businesses/{client_id}/budgets/{budget_id}/members/{budget_member_id}\n  method: patch\n  operationId: updateBudgetMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/businesses/{client_id}/budgets/{budget_id}/members/{budget_member_id}\n  method: delete\n  operationId: deleteBudgetMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/businesses/{client_id}/budgets/{budget_id}/owners\n  method:\
  \ get\n  operationId: listBudgetOwners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/businesses/{client_id}/budgets/{budget_id}/owners\n  method: post\n  operationId: createBudgetOwner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/businesses/{client_id}/budgets/{budget_id}/owners/{budget_owner_id}\n  method: delete\n  operationId: deleteBudgetOwner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/businesses/{client_id}/budgets/{budget_id}/members/{budget_member_id}/topups\n\
  \  method: get\n  operationId: listBudgetMemberTopups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/businesses/{client_id}/budgets/{budget_id}/members/{budget_member_id}/topups\n  method: post\n  operationId: createBudgetMemberTopup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/businesses/{client_id}/balance\n  method: get\n  operationId: listBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/businesses/{client_id}/custom-fields\n  method: get\n  operationId: listCustomFields\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/businesses/{client_id}/custom-fields\n  method: post\n  operationId: createCustomField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/businesses/{client_id}/custom-fields/{custom_field_id}\n  method: get\n  operationId: getCustomField\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/businesses/{client_id}/custom-fields/{custom_field_id}\n  method: patch\n  operationId: updateCustomField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/businesses/{client_id}/custom-fields/{custom_field_id}\n  method: delete\n  operationId: deleteCustomField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/businesses/{client_id}/custom-fields/{custom_field_id}/options\n  method: get\n  operationId: listCustomFieldOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/businesses/{client_id}/custom-fields/{custom_field_id}/options\n  method: post\n  operationId: createCustomFieldOption\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/businesses/{client_id}/custom-fields/{custom_field_id}/options/{option_id}\n  method: patch\n  operationId: updateCustomFieldOption\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/businesses/{client_id}/custom-fields/{custom_field_id}/options/{option_id}\n  method: delete\n  operationId: deleteCustomFieldOption\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/businesses/{client_id}/custom-fields/{custom_field_id}/budgets\n  method: get\n  operationId: listCustomFieldBudgets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/businesses/{client_id}/custom-fields/{custom_field_id}/budgets\n  method: post\n  operationId: linkCustomFieldBudget\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/businesses/{client_id}/custom-fields/{custom_field_id}/budgets/{budget_id}\n  method: delete\n  operationId: unlinkCustomFieldBudget\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/businesses/{client_id}/accounting-codes\n  method: get\n  operationId: listAccountingCodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/businesses/{client_id}/accounting-codes\n  method: post\n  operationId: upsertAccountingCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/businesses/{client_id}/accounting-codes/{accounting_code_id}\n  method: delete\n  operationId: deleteAccountingCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n  \
  \  subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/businesses/{client_id}/categories\n  method: get\n  operationId: listCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/businesses/{client_id}/categories\n  method: post\n  operationId: createCategory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/businesses/{client_id}/categories/{category_id}\n  method: patch\n  operationId: updateCategory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/businesses/{client_id}/categories/{category_id}\n  method: delete\n  operationId: deleteCategory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/businesses/{client_id}/tax-rates\n  method: get\n  operationId: listTaxRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/businesses/{client_id}/tax-rates/{tax_rate_id}\n  method: get\n  operationId: getTaxRate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weel/refs/heads/main/agentic-access/weel-agentic-access.yml
summary_line: 51 operations · 27 acting
tags:
- Payments
- Australia
- Spend Management
- Expense Management
- Corporate Cards
- Accounts Payable
- Card Issuing
- Reimbursement
- Budgets
- Fintech
---
