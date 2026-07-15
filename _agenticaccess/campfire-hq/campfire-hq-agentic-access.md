---
acting_count: 17
action_class_counts:
  acting: 17
  connected: 26
api_specs:
- filename: campfire-hq-openapi.yml
  format: yaml
  label: Campfire Core Accounting API
  slug: campfire-hq-core-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire-hq/refs/heads/main/openapi/campfire-hq-openapi.yml
- filename: campfire-hq-openapi.yml
  format: yaml
  label: Campfire Chart of Accounts & Company Objects API
  slug: campfire-hq-chart-of-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire-hq/refs/heads/main/openapi/campfire-hq-openapi.yml
- filename: campfire-hq-openapi.yml
  format: yaml
  label: Campfire Financial Statements API
  slug: campfire-hq-financial-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire-hq/refs/heads/main/openapi/campfire-hq-openapi.yml
- filename: campfire-hq-openapi.yml
  format: yaml
  label: Campfire Accounts Payable API
  slug: campfire-hq-accounts-payable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire-hq/refs/heads/main/openapi/campfire-hq-openapi.yml
- filename: campfire-hq-openapi.yml
  format: yaml
  label: Campfire Accounts Receivable API
  slug: campfire-hq-accounts-receivable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire-hq/refs/heads/main/openapi/campfire-hq-openapi.yml
- filename: campfire-hq-openapi.yml
  format: yaml
  label: Campfire Revenue Recognition API
  slug: campfire-hq-revenue-recognition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire-hq/refs/heads/main/openapi/campfire-hq-openapi.yml
- filename: campfire-hq-openapi.yml
  format: yaml
  label: Campfire Cash Management API
  slug: campfire-hq-cash-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire-hq/refs/heads/main/openapi/campfire-hq-openapi.yml
- filename: campfire-hq-openapi.yml
  format: yaml
  label: Campfire Bank Reconciliation API
  slug: campfire-hq-bank-reconciliation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire-hq/refs/heads/main/openapi/campfire-hq-openapi.yml
- filename: campfire-hq-openapi.yml
  format: yaml
  label: Campfire Settings API
  slug: campfire-hq-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire-hq/refs/heads/main/openapi/campfire-hq-openapi.yml
- filename: campfire-hq-openapi.yml
  format: yaml
  label: Campfire Integrations & Webhooks API
  slug: campfire-hq-integrations-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire-hq/refs/heads/main/openapi/campfire-hq-openapi.yml
consequence_counts:
  physical: 3
  read: 26
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Campfire Hq Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ca/api/v1/custom-fields/reorder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /coa/api/entity/{entity_id}/attachment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /coa/api/v1/invoice/
operation_count: 43
overview: 'Campfire exposes 43 API operations that an AI agent could call, of which 17 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 26 read, 14 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Campfire
provider_slug: campfire-hq
slug: campfire-hq-agentic-access
source_filename: campfire-hq-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/campfire-hq-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 43\n  by_action_class:\n    connected: 26\n    acting: 17\n  by_consequence:\n    read: 26\n    write: 14\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /ca/api/account\n  method: get\n  operationId: list_accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca/api/account\n  method: post\n  operationId: create_account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca/api/cash-basis\n  method: get\n  operationId: ca_api_cash_basis_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca/api/file\n  method: get\n  operationId: ca_api_file_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca/api/get_balance_sheet\n  method: get\n  operationId: ca_api_get_balance_sheet_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca/api/get_cash_flow\n  method: get\n  operationId: ca_api_get_cash_flow_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /ca/api/get_income_statement\n  method: get\n  operationId: ca_api_get_income_statement_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca/api/get_trial_balance\n  method: get\n  operationId: ca_api_get_trial_balance_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca/api/transaction\n  method: get\n  operationId: list_bank_transactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca/api/transaction\n  method: post\n  operationId: create_bank_transaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca/api/v1/custom-fields/reorder\n  method: post\n  operationId: ca_api_v1_custom_fields_reorder_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/budgets\n  method: get\n  operationId: coa_api_budgets_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/budgets\n  method: post\n  operationId: coa_api_budgets_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/budgets/{id}\n  method: get\n  operationId: coa_api_budgets_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/entity\n  method: get\n  operationId: coa_api_entity_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/entity\n  method: post\n  operationId: coa_api_entity_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/entity/{entity_id}/attachment\n\
  \  method: post\n  operationId: coa_api_entity_attachment_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/fixed-asset\n  method: get\n  operationId: coa_api_fixed_asset_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/fixed-asset\n  method: post\n  operationId: coa_api_fixed_asset_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /coa/api/general-ledger\n  method: get\n  operationId: coa_api_general_ledger_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/tag\n  method: get\n  operationId: coa_api_tag_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/tag\n  method: post\n  operationId: coa_api_tag_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/transaction\n  method: get\n  operationId: coa_api_transaction_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /coa/api/v1/bill-draft\n  method: get\n  operationId: list_bill_drafts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/v1/bill-draft\n  method: post\n  operationId: create_bill_draft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/bill/\n  method: get\n  operationId: coa_api_v1_bill_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/v1/bill/\n  method: post\n  operationId: coa_api_v1_bill_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/credit-memo\n  method: get\n  operationId: coa_api_v1_credit_memo_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/v1/credit-memo\n  method: post\n  operationId: coa_api_v1_credit_memo_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/invoice/\n  method: get\n  operationId: coa_api_v1_invoice_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n \
  \   token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/v1/invoice/\n  method: post\n  operationId: coa_api_v1_invoice_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v2/reconciliation\n  method: get\n  operationId: coa_api_v2_reconciliation_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/v2/reconciliation\n  method: post\n  operationId: coa_api_v2_reconciliation_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/vendor\n  method: get\n  operationId: coa_api_vendor_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/vendor\n  method: post\n  operationId: coa_api_vendor_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integrations/api/v1/webhook\n  method: get\n  operationId: integrations_api_v1_webhook_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrations/api/v1/webhook\n  method: post\n  operationId: integrations_api_v1_webhook_create\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integrations/api/v1/webhook/{id}\n  method: get\n  operationId: integrations_api_v1_webhook_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rr/api/v1/contracts\n  method: get\n  operationId: list_contracts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rr/api/v1/contracts\n  method: post\n  operationId: create_contract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n \
  \     human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rr/api/v1/customers\n  method: get\n  operationId: rr_api_v1_customers_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rr/api/v1/product\n  method: get\n  operationId: list_products\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rr/api/v1/product\n  method: post\n  operationId: create_product\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/campfire-hq/refs/heads/main/agentic-access/campfire-hq-agentic-access.yml
summary_line: 43 operations · 17 acting
tags:
- Accounting
- ERP
- General Ledger
- Revenue Recognition
- FinTech
- AI
---
