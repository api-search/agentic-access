---
acting_count: 233
action_class_counts:
  acting: 233
  connected: 129
api_specs:
- filename: campfire-openapi-original.json
  format: json
  label: Campfire Developer APIs
  slug: campfire-developer-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-openapi-original.json
consequence_counts:
  physical: 27
  read: 129
  safety-critical: 2
  write: 204
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Campfire Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /rr/api/v1/contracts/{contract_id}/tier-price-overrides
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /rr/api/v1/contracts/{id}/terminate
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
  path: /coa/api/transaction/{transaction_id}/bill_payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /coa/api/transaction/{transaction_id}/credit_memo_payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /coa/api/transaction/{transaction_id}/debit_memo_payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /coa/api/transaction/{transaction_id}/invoice_payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /coa/api/v1/bill/{bill_id}/payment/{payment_id}/void/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /coa/api/v1/bill/{bill_id}/payment/{payment_id}/void/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /coa/api/v1/credit-memo/{credit_memo_id}/payment/{payment_id}/void
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /coa/api/v1/credit-memo/{credit_memo_id}/payment/{payment_id}/void
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /coa/api/v1/credit-memo/{id}/send/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /coa/api/v1/debit-memo/{debit_memo_id}/payment/{payment_id}/void
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /coa/api/v1/debit-memo/{debit_memo_id}/payment/{payment_id}/void
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /coa/api/v1/invoice/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /coa/api/v1/invoice/bulk-apply-payment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /coa/api/v1/invoice/bulk-create
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /coa/api/v1/invoice/bulk-search
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /coa/api/v1/invoice/{id}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /coa/api/v1/invoice/{id}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /coa/api/v1/invoice/{id}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /coa/api/v1/invoice/{invoice_id}/calculate-payment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /coa/api/v1/invoice/{invoice_id}/default-payment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /coa/api/v1/invoice/{invoice_id}/pay/
operation_count: 362
overview: 'Campfire exposes 362 API operations that an AI agent could call, of which 233 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 129 read, 204 write, 27 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Campfire
provider_slug: campfire
slug: campfire-agentic-access
source_filename: campfire-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/campfire-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 362\n  by_action_class:\n    connected: 129\n    acting: 233\n  by_consequence:\n    read: 129\n    write: 204\n    physical: 27\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /ca/api/account\n  method: get\n  operationId: list_accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca/api/account\n  method: post\n  operationId: create_account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca/api/account/{id}\n  method: get\n  operationId: ca_api_account_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca/api/account/{id}\n  method: put\n  operationId: ca_api_account_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca/api/account/{id}\n  method: patch\n  operationId: ca_api_account_partial_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca/api/account/{id}\n  method: delete\n  operationId: ca_api_account_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca/api/balance-sheet/comparative\n  method: get\n  operationId: ca_api_balance_sheet_comparative_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca/api/bank-feed/{account_id}\n  method: post\n  operationId: ca_api_bank_feed_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca/api/cash-basis\n  method: get\n  operationId: ca_api_cash_basis_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca/api/cash-basis-operating-statement\n  method: get\n  operationId: ca_api_cash_basis_operating_statement_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca/api/cash-operating-statement/transactions\n  method: get\n  operationId: ca_api_cash_operating_statement_transactions_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca/api/file\n  method: get\n  operationId: ca_api_file_list\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca/api/file/{id}\n  method: get\n  operationId: ca_api_file_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca/api/file/{id}\n  method: put\n  operationId: ca_api_file_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca/api/file/{id}\n  method: patch\n  operationId: ca_api_file_partial_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /ca/api/file/{id}\n  method: delete\n  operationId: ca_api_file_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca/api/file/{id}/temp-download-url\n  method: get\n  operationId: get_file_temp_download_url\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca/api/file/upload\n  method: post\n  operationId: ca_api_file_upload_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /ca/api/get_balance_sheet\n  method: get\n  operationId: ca_api_get_balance_sheet_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca/api/get_cash_flow\n  method: get\n  operationId: ca_api_get_cash_flow_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca/api/get_cash_flow_activity\n  method: get\n  operationId: ca_api_get_cash_flow_activity_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca/api/get_cash_flow_v2\n  method: get\n  operationId: ca_api_get_cash_flow_v2_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /ca/api/get_income_statement\n  method: get\n  operationId: ca_api_get_income_statement_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca/api/get_trial_balance\n  method: get\n  operationId: ca_api_get_trial_balance_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca/api/income-statement/comparative\n  method: get\n  operationId: ca_api_income_statement_comparative_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca/api/transaction\n  method: get\n  operationId: list_bank_transactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /ca/api/transaction\n  method: post\n  operationId: create_bank_transaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca/api/transaction/{id}\n  method: get\n  operationId: ca_api_transaction_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca/api/transaction/{id}\n  method: put\n  operationId: ca_api_transaction_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca/api/transaction/{id}\n\
  \  method: patch\n  operationId: ca_api_transaction_partial_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca/api/transaction/{id}\n  method: delete\n  operationId: ca_api_transaction_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca/api/user_currency\n  method: get\n  operationId: ca_api_user_currency_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca/api/user_currency\n  method: post\n \
  \ operationId: ca_api_user_currency_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca/api/user_currency/{id}\n  method: get\n  operationId: ca_api_user_currency_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca/api/user_currency/{id}\n  method: put\n  operationId: ca_api_user_currency_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca/api/user_currency/{id}\n  method: patch\n  operationId:\
  \ ca_api_user_currency_partial_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca/api/user_currency/{id}\n  method: delete\n  operationId: ca_api_user_currency_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca/api/user_currency/rate\n  method: get\n  operationId: ca_api_user_currency_rate_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca/api/user_currency/with_rate\n  method: get\n  operationId:\
  \ ca_api_user_currency_with_rate_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca/api/v1/custom-fields\n  method: get\n  operationId: ca_api_v1_custom_fields_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca/api/v1/custom-fields\n  method: post\n  operationId: ca_api_v1_custom_fields_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca/api/v1/custom-fields/{id}\n  method: get\n  operationId: ca_api_v1_custom_fields_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca/api/v1/custom-fields/{id}\n  method: put\n  operationId: ca_api_v1_custom_fields_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca/api/v1/custom-fields/{id}\n  method: patch\n  operationId: ca_api_v1_custom_fields_partial_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca/api/v1/custom-fields/{id}\n  method: delete\n  operationId: ca_api_v1_custom_fields_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca/api/v1/custom-fields/reorder\n  method: post\n  operationId: ca_api_v1_custom_fields_reorder_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/account\n  method: get\n  operationId: coa_api_account_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/account\n  method: post\n  operationId: coa_api_account_create\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/account/{id}\n  method: get\n  operationId: coa_api_account_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/account/{id}\n  method: put\n  operationId: coa_api_account_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/account/{id}\n  method: patch\n  operationId: coa_api_account_partial_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/account/{id}\n  method: delete\n  operationId: coa_api_account_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/account/balance-sheet\n  method: get\n  operationId: coa_api_account_balance_sheet_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/account/balance-sheet\n  method: post\n  operationId: coa_api_account_balance_sheet_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/account/income-statement\n  method: get\n  operationId: coa_api_account_income_statement_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/account/income-statement\n  method: post\n  operationId: coa_api_account_income_statement_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/budgets\n  method: get\n  operationId: coa_api_budgets_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/budgets\n  method: post\n  operationId: coa_api_budgets_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/budgets/{budget_pk}/accounts\n  method: get\n  operationId: coa_api_budgets_accounts_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/budgets/{budget_pk}/accounts\n  method: post\n  operationId: coa_api_budgets_accounts_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /coa/api/budgets/{budget_pk}/accounts/{id}\n  method: get\n  operationId: coa_api_budgets_accounts_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/budgets/{budget_pk}/accounts/{id}\n  method: put\n  operationId: coa_api_budgets_accounts_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/budgets/{budget_pk}/accounts/{id}\n  method: patch\n  operationId: coa_api_budgets_accounts_partial_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n   \
  \   human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/budgets/{budget_pk}/accounts/{id}\n  method: delete\n  operationId: coa_api_budgets_accounts_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/budgets/{id}\n  method: get\n  operationId: coa_api_budgets_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/budgets/{id}\n  method: put\n  operationId: coa_api_budgets_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/budgets/{id}\n  method: patch\n  operationId: coa_api_budgets_partial_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/budgets/{id}\n  method: delete\n  operationId: coa_api_budgets_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/chart-account-settings\n  method: get\n  operationId: settings_retrieve_chart_account_settings\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/chart-account-settings\n  method: put\n  operationId: settings_update_chart_account_settings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/chart-account-settings\n  method: patch\n  operationId: settings_partial_update_chart_account_settings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/cost-allocations\n  method: get\n  operationId: coa_api_cost_allocations_list\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/cost-allocations\n  method: post\n  operationId: coa_api_cost_allocations_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/cost-allocations/{id}\n  method: get\n  operationId: coa_api_cost_allocations_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/cost-allocations/{id}\n  method: put\n  operationId: coa_api_cost_allocations_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/cost-allocations/{id}\n  method: patch\n  operationId: coa_api_cost_allocations_partial_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/cost-allocations/{id}\n  method: delete\n  operationId: coa_api_cost_allocations_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/department\n  method: get\n  operationId: coa_api_department_list\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/department\n  method: post\n  operationId: coa_api_department_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/department/{id}\n  method: get\n  operationId: coa_api_department_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/department/{id}\n  method: put\n  operationId: coa_api_department_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/department/{id}\n  method: patch\n  operationId: coa_api_department_partial_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/department/{id}\n  method: delete\n  operationId: coa_api_department_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/department/bulk-search\n  method: post\n  operationId: coa_api_department_bulk_search_create\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/entity\n  method: get\n  operationId: coa_api_entity_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/entity\n  method: post\n  operationId: coa_api_entity_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/entity/{entity_id}/attachment\n  method: post\n  operationId: coa_api_entity_attachment_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/entity/{id}\n  method: get\n  operationId: coa_api_entity_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/entity/{id}\n  method: put\n  operationId: coa_api_entity_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/entity/{id}\n  method: patch\n  operationId: coa_api_entity_partial_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/entity/{id}\n  method: delete\n  operationId: coa_api_entity_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/entity/{id}/logo\n  method: post\n  operationId: coa_api_entity_logo_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/entity/for-intercompany\n  method: get\n  operationId:\
  \ coa_api_entity_for_intercompany_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/fixed-asset\n  method: get\n  operationId: coa_api_fixed_asset_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/fixed-asset\n  method: post\n  operationId: coa_api_fixed_asset_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/fixed-asset-automation/\n  method: get\n  operationId: list_fixed_asset_automations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n- path: /coa/api/fixed-asset-automation/\n  method: post\n  operationId: create_fixed_asset_automation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/fixed-asset-automation-match/{id}/\n  method: get\n  operationId: get_fixed_asset_automation_match\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/fixed-asset-automation-match/{id}/\n  method: put\n  operationId: update_fixed_asset_automation_match\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/fixed-asset-automation-match/{id}/\n  method: patch\n  operationId: partial_update_fixed_asset_automation_match\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/fixed-asset-automation/{id}/\n  method: get\n  operationId: get_fixed_asset_automation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/fixed-asset-automation/{id}/\n  method: put\n  operationId: update_fixed_asset_automation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/fixed-asset-automation/{id}/\n  method: patch\n  operationId: partial_update_fixed_asset_automation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/fixed-asset-automation/{id}/\n  method: delete\n  operationId: delete_fixed_asset_automation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/fixed-asset-automation/accounts\n  method: get\n  operationId: list_fixed_asset_automation_accounts\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      \n\n# --- truncated at 32 KB (116 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/agentic-access/campfire-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/agentic-access/campfire-agentic-access.yml
summary_line: 362 operations · 233 acting · 2 human-in-the-loop
tags:
- Company
- Accounting
- ERP
- Finance
- Revenue Recognition
- Accounts Payable
- Accounts Receivable
- AI
---
