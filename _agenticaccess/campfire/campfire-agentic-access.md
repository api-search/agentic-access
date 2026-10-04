---
acting_count: 236
action_class_counts:
  acting: 236
  connected: 132
api_specs:
- filename: campfire-accounts-payable-api-openapi.yml
  format: yaml
  label: Campfire Accounts Payable API
  slug: campfire-accounts-payable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-accounts-payable-api-openapi.yml
- filename: campfire-accounts-receivable-api-openapi.yml
  format: yaml
  label: Campfire Accounts Receivable API
  slug: campfire-accounts-receivable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-accounts-receivable-api-openapi.yml
- filename: campfire-bank-reconciliation-api-openapi.yml
  format: yaml
  label: Campfire Bank Reconciliation API
  slug: campfire-bank-reconciliation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-bank-reconciliation-api-openapi.yml
- filename: campfire-cash-management-api-openapi.yml
  format: yaml
  label: Campfire Cash Management API
  slug: campfire-cash-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-cash-management-api-openapi.yml
- filename: campfire-coa-api-openapi.yml
  format: yaml
  label: Campfire Coa API
  slug: campfire-coa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-coa-api-openapi.yml
- filename: campfire-company-objects-api-openapi.yml
  format: yaml
  label: Campfire Company Objects API
  slug: campfire-company-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-company-objects-api-openapi.yml
- filename: campfire-core-accounting-api-openapi.yml
  format: yaml
  label: Campfire Core Accounting API
  slug: campfire-core-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-core-accounting-api-openapi.yml
- filename: campfire-custom-fields-api-openapi.yml
  format: yaml
  label: Campfire Custom Fields API
  slug: campfire-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-custom-fields-api-openapi.yml
- filename: campfire-financial-statements-api-openapi.yml
  format: yaml
  label: Campfire Financial Statements API
  slug: campfire-financial-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-financial-statements-api-openapi.yml
- filename: campfire-integrations-api-openapi.yml
  format: yaml
  label: Campfire Integrations API
  slug: campfire-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-integrations-api-openapi.yml
- filename: campfire-revenue-recognition-api-openapi.yml
  format: yaml
  label: Campfire Revenue Recognition API
  slug: campfire-revenue-recognition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-revenue-recognition-api-openapi.yml
- filename: campfire-settings-api-openapi.yml
  format: yaml
  label: Campfire Settings API
  slug: campfire-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/openapi/campfire-settings-api-openapi.yml
consequence_counts:
  physical: 26
  read: 132
  safety-critical: 2
  write: 208
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
  path: /coa/api/v1/invoice/{invoice_id}/pay/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /coa/api/v1/invoice/{invoice_id}/payment/{payment_id}/void/
operation_count: 368
overview: 'Campfire exposes 368 API operations that an AI agent could call, of which 236 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 132 read, 208 write, 26 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Campfire
provider_slug: campfire
slug: campfire-agentic-access
source_filename: campfire-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/campfire-accounts-payable-api-openapi.yml, openapi/campfire-accounts-receivable-api-openapi.yml,\n  openapi/campfire-bank-reconciliation-api-openapi.yml, openapi/campfire-cash-management-api-openapi.yml,\n  openapi/campfire-coa-api-openapi.yml, openapi/campfire-company-objects-api-openapi.yml, openapi/campfire-core-accounting-api-openapi.yml,\n  openapi/campfire-custom-fields-api-openapi.yml, openapi/campfire-financial-statements-api-openapi.yml,\n  openapi/campfire-integrations-api-openapi.yml, openapi/campfire-revenue-recognition-api-openapi.yml,\n  openapi/campfire-settings-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 368\n  by_action_class:\n    connected: 132\n\
  \    acting: 236\n  by_consequence:\n    read: 132\n    write: 208\n    physical: 26\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /coa/api/v1/bill/\n  method: get\n  operationId: coa_api_v1_bill_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/v1/bill/\n  method: post\n  operationId: coa_api_v1_bill_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/bill-draft\n  method: get\n  operationId: list_bill_drafts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/v1/bill-draft\n\
  \  method: post\n  operationId: create_bill_draft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/bill-draft/{id}\n  method: get\n  operationId: get_bill_draft\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/v1/bill-draft/{id}\n  method: put\n  operationId: update_bill_draft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/bill-draft/{id}\n  method: patch\n  operationId: partial_update_bill_draft\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/bill-draft/{id}/abandon\n  method: post\n  operationId: abandon_bill_draft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/bill-draft/{id}/discard\n  method: post\n  operationId: discard_bill_draft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /coa/api/v1/bill-draft/{id}/promote\n  method: post\n  operationId: promote_bill_draft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/bill-payments\n  method: get\n  operationId: coa_api_v1_bill_payments_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/v1/bill/{bill_id}/empty-transaction-default-department-tags\n  method: get\n  operationId: coa_api_v1_bill_empty_transaction_default_department_tags_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/v1/bill/{bill_id}/pay/\n\
  \  method: post\n  operationId: coa_api_v1_bill_pay_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/bill/{bill_id}/payment/{payment_id}/void/\n  method: post\n  operationId: coa_api_v1_bill_payment_void_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/bill/{bill_id}/payment/{payment_id}/void/\n  method: delete\n  operationId: coa_api_v1_bill_payment_void_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/bill/{bill_id}/reopen/\n  method: post\n  operationId: coa_api_v1_bill_reopen_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/bill/{bill_id}/sync-to-ramp/\n  method: post\n  operationId: coa_api_v1_bill_sync_to_ramp_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n   \
  \   - high-value\n    audit: required\n- path: /coa/api/v1/bill/{bill_id}/void/\n  method: post\n  operationId: coa_api_v1_bill_void_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/bill/{id}/\n  method: get\n  operationId: coa_api_v1_bill_retrieve_2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/v1/bill/{id}/\n  method: put\n  operationId: coa_api_v1_bill_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n   \
  \ audit: required\n- path: /coa/api/v1/bill/{id}/\n  method: patch\n  operationId: coa_api_v1_bill_partial_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/bill/{id}/\n  method: delete\n  operationId: coa_api_v1_bill_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/bill/amortization/generate-schedule\n  method: get\n  operationId: generate_bill_amortization_schedule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /coa/api/v1/bill/amortization/generate-schedule\n  method: put\n  operationId: save_bill_amortization_schedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/bill/bulk-search\n  method: post\n  operationId: coa_api_v1_bill_bulk_search_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/bill/bulk-sync-to-ramp/\n  method: post\n  operationId: bulk_sync_bills_to_ramp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/debit-memo\n  method: get\n  operationId: coa_api_v1_debit_memo_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/v1/debit-memo\n  method: post\n  operationId: coa_api_v1_debit_memo_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/debit-memo/{debit_memo_id}/mark-used\n  method: post\n  operationId: coa_api_v1_debit_memo_mark_used_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/debit-memo/{debit_memo_id}/payment/{payment_id}/void\n  method: post\n  operationId: coa_api_v1_debit_memo_payment_void_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/debit-memo/{debit_memo_id}/payment/{payment_id}/void\n  method: delete\n  operationId: coa_api_v1_debit_memo_payment_void_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n  \
  \    purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/debit-memo/{debit_memo_id}/reopen/\n  method: post\n  operationId: coa_api_v1_debit_memo_reopen_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/debit-memo/{debit_memo_id}/void/\n  method: post\n  operationId: coa_api_v1_debit_memo_void_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/debit-memo/{id}\n  method:\
  \ get\n  operationId: coa_api_v1_debit_memo_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/v1/debit-memo/{id}\n  method: put\n  operationId: coa_api_v1_debit_memo_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/debit-memo/{id}\n  method: patch\n  operationId: coa_api_v1_debit_memo_partial_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/debit-memo/{id}\n  method:\
  \ delete\n  operationId: coa_api_v1_debit_memo_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/debit-memo/bulk-search\n  method: post\n  operationId: coa_api_v1_debit_memo_bulk_search_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/debit-memo/next-debit-memo-number\n  method: get\n  operationId: coa_api_v1_debit_memo_next_debit_memo_number_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /coa/api/v1/credit-memo\n  method: get\n  operationId: coa_api_v1_credit_memo_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/v1/credit-memo\n  method: post\n  operationId: coa_api_v1_credit_memo_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/credit-memo/{credit_memo_id}/mark-used\n  method: post\n  operationId: coa_api_v1_credit_memo_mark_used_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /coa/api/v1/credit-memo/{credit_memo_id}/payment/{payment_id}/void\n  method: post\n  operationId: coa_api_v1_credit_memo_payment_void_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/credit-memo/{credit_memo_id}/payment/{payment_id}/void\n  method: delete\n  operationId: coa_api_v1_credit_memo_payment_void_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /coa/api/v1/credit-memo/{credit_memo_id}/reopen/\n  method: post\n  operationId: coa_api_v1_credit_memo_reopen_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/credit-memo/{credit_memo_id}/void/\n  method: post\n  operationId: coa_api_v1_credit_memo_void_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/credit-memo/{id}\n  method: get\n  operationId: coa_api_v1_credit_memo_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/v1/credit-memo/{id}\n  method: put\n  operationId: coa_api_v1_credit_memo_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/credit-memo/{id}\n  method: patch\n  operationId: coa_api_v1_credit_memo_partial_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/credit-memo/{id}\n  method: delete\n  operationId: coa_api_v1_credit_memo_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/credit-memo/{id}/pdf/\n  method: get\n  operationId: get_credit_memo_pdf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/v1/credit-memo/{id}/send/\n  method: put\n  operationId: send_credit_memo\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/credit-memo/bulk-search\n  method: post\n  operationId: coa_api_v1_credit_memo_bulk_search_create\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/credit-memo/next-credit-memo-number\n  method: get\n  operationId: coa_api_v1_credit_memo_next_credit_memo_number_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/v1/invoice/\n  method: get\n  operationId: coa_api_v1_invoice_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/v1/invoice/\n  method: post\n  operationId: coa_api_v1_invoice_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n    \
  \  max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/invoice-payments\n  method: get\n  operationId: coa_api_v1_invoice_payments_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/v1/invoice/{invoice_id}/calculate-payment\n  method: post\n  operationId: coa_api_v1_invoice_calculate_payment_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/invoice/{invoice_id}/default-payment\n  method: post\n  operationId:\
  \ coa_api_v1_invoice_default_payment_create\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/v1/invoice/{invoice_id}/pay/\n  method: post\n  operationId: coa_api_v1_invoice_pay_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/invoice/{invoice_id}/payment/{payment_id}/void/\n  method: post\n  operationId: coa_api_v1_invoice_payment_void_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/invoice/{invoice_id}/payment/{payment_id}/void/\n  method: delete\n  operationId: coa_api_v1_invoice_payment_void_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/invoice/{invoice_id}/reopen/\n  method: post\n  operationId: coa_api_v1_invoice_reopen_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /coa/api/v1/invoice/{invoice_id}/void/\n  method: post\n  operationId: coa_api_v1_invoice_void_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/invoice/{id}/\n  method: get\n  operationId: coa_api_v1_invoice_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/v1/invoice/{id}/\n  method: put\n  operationId: coa_api_v1_invoice_update\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/invoice/{id}/\n  method: patch\n  operationId: coa_api_v1_invoice_partial_update\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/invoice/{id}/\n  method: delete\n  operationId: coa_api_v1_invoice_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/invoice/bulk-apply-payment\n\
  \  method: post\n  operationId: coa_api_v1_invoice_bulk_apply_payment_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/invoice/bulk-create\n  method: post\n  operationId: bulk_create_invoices\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/invoice/bulk-search\n  method: post\n  operationId: coa_api_v1_invoice_bulk_search_create\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v1/invoice/report/{id}/data\n  method: get\n  operationId: coa_api_v1_invoice_report_data_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/v1/invoice/report/preview\n  method: get\n  operationId: coa_api_v1_invoice_report_preview_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/v1/invoice/statement/client/{client_id}/pdf/\n  method: get\n  operationId: get_client_invoice_statement_pdf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rr/api/v1/product\n  method: get\n  operationId: list_products\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rr/api/v1/product\n  method: post\n  operationId: create_product\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rr/api/v1/product/{id}\n  method: get\n  operationId: rr_api_v1_product_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rr/api/v1/product/{id}\n  method: put\n  operationId: rr_api_v1_product_update\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rr/api/v1/product/{id}\n  method: patch\n  operationId: rr_api_v1_product_partial_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rr/api/v1/product/{id}\n  method: delete\n  operationId: rr_api_v1_product_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v2/reconciliation\n\
  \  method: get\n  operationId: coa_api_v2_reconciliation_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/v2/reconciliation\n  method: post\n  operationId: coa_api_v2_reconciliation_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v2/reconciliation/{id}\n  method: get\n  operationId: coa_api_v2_reconciliation_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/v2/reconciliation/{id}\n  method: put\n  operationId: coa_api_v2_reconciliation_update\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v2/reconciliation/{id}\n  method: patch\n  operationId: coa_api_v2_reconciliation_partial_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v2/reconciliation/{id}\n  method: delete\n  operationId: coa_api_v2_reconciliation_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /coa/api/v2/reconciliation/{id}/bulk-match-transactions\n  method: post\n  operationId: coa_api_v2_reconciliation_bulk_match_transactions_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v2/reconciliation/{id}/source-transactions\n  method: get\n  operationId: coa_api_v2_reconciliation_source_transactions_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coa/api/v2/reconciliation/{id}/transactions/confirm\n  method: post\n  operationId: coa_api_v2_reconciliation_transactions_confirm_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coa/api/v2/reconciliation/parse-statement-page\n  method: post\n  operationId: parse_bank_statement_page\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca/api/account\n  method: get\n  operationId: list_accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\n\n# --- truncated at 32 KB (118 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/agentic-access/campfire-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/campfire/refs/heads/main/agentic-access/campfire-agentic-access.yml
summary_line: 368 operations · 236 acting · 2 human-in-the-loop
tags:
- Company
- Accounting
- ERP
- Finance
- Revenue Recognition
- Accounts Payable
- Accounts Receivable
- Artificial Intelligence
---
