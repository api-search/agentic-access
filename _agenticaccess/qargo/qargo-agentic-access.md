---
acting_count: 64
action_class_counts:
  acting: 64
  connected: 50
api_specs:
- filename: qargo-tms-openapi-original.yml
  format: yaml
  label: Qargo TMS API
  slug: qargo-tms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qargo/refs/heads/main/openapi/qargo-tms-openapi-original.yml
consequence_counts:
  physical: 21
  read: 50
  safety-critical: 7
  write: 36
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 7
kind: agentic-access
layout: agentic-access
method: generated
name: Qargo Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/webhook/fleet-document-upload
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/webhook/fleet-status-update
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/webhook/subco-document-upload
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/webhook/subco-status-update
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: https://<external-fleet-receiving-endpoint>
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: https://<external_subco_receiving_endpoint>
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: https://<location-booking-receiving-endpoint>
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/accounting/purchase-credit-note/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/accounting/purchase-credit-note/{id}/refund/update-status
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/accounting/purchase-invoice/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/accounting/purchase-invoice/{id}/payment/update-status
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/accounting/purchase_invoice/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/accounting/purchase_invoice/{id}/payment/update-status
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/accounting/sales-credit-note/{id}/refund/update-status
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/accounting/sales-invoice/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/accounting/sales-invoice/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/accounting/sales-invoice/{id}/payment/update-status
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/accounting/sales_credit_note/{id}/refund/update-status
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/accounting/sales_invoice/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/accounting/sales_invoice/{id}/payment/update-status
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/accounting/sync-tasks/{id}/update-status
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/orders/order/upload
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/orders/order/{order_id}/charges/approval
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/webhook
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/webhook/billing-document-update
operation_count: 114
overview: 'Qargo exposes 114 API operations that an AI agent could call, of which 64 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 50 read, 36 write, 21 physical, and 7 safety-critical.


  7 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Qargo
provider_slug: qargo
slug: qargo-agentic-access
source_filename: qargo-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/qargo-tms-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 114\n  by_action_class:\n    connected: 50\n    acting: 64\n  by_consequence:\n    read: 50\n    write: 36\n    physical: 21\n    safety-critical: 7\n  human_in_the_loop_required: 7\noperations:\n- path: /v1/accounting/accounts\n  method: get\n  operationId: List_accounts_v1_accounting_accounts_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounting/accounts/{id}\n  method: get\n  operationId: Retrieve_account_v1_accounting_accounts__id__get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounting/exchange-rate\n  method: post\n  operationId: Create_an_exchange_rate_v1_accounting_exchange_rate_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounting/exchange-rate\n  method: get\n  operationId: List_exchange_rates_v1_accounting_exchange_rate_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounting/purchase-credit-note/{id}\n  method: get\n  operationId: Retrieve_purchase_credit_note_v1_accounting_purchase_credit_note__id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n   \
  \ subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounting/purchase-credit-note/{id}\n  method: patch\n  operationId: Update_purchase_credit_note_v1_accounting_purchase_credit_note__id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounting/purchase-credit-note/{id}/documents\n  method: get\n  operationId: Retrieve_purchase_credit_note_documents_v1_accounting_purchase_credit_note__id__documents_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounting/purchase-credit-note/{id}/refund/update-status\n  method: post\n  operationId: Report_refund_status_for_purchase_credit_note_v1_accounting_purchase_credit_note__id__refund_update_status_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounting/purchase-invoice/{id}\n  method: get\n  operationId: Retrieve_purchase_invoice_v1_accounting_purchase_invoice__id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounting/purchase-invoice/{id}\n  method: patch\n  operationId: Update_purchase_invoice_v1_accounting_purchase_invoice__id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounting/purchase-invoice/{id}/documents\n  method: get\n  operationId: Retrieve_purchase_invoice_documents_v1_accounting_purchase_invoice__id__documents_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounting/purchase-invoice/{id}/payment/update-status\n  method: post\n  operationId: Report_payment_status_for_purchase_invoice_v1_accounting_purchase_invoice__id__payment_update_status_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounting/sales-credit-note/\n  method:\
  \ post\n  operationId: Create_a_sales_credit_note_v1_accounting_sales_credit_note__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounting/sales-credit-note/{id}\n  method: get\n  operationId: Retrieve_sales_credit_note_v1_accounting_sales_credit_note__id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounting/sales-credit-note/{id}\n  method: patch\n  operationId: Update_credit_note_v1_accounting_sales_credit_note__id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounting/sales-credit-note/{id}/documents\n  method: get\n  operationId: Retrieve_sales_credit_note_documents_v1_accounting_sales_credit_note__id__documents_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounting/sales-credit-note/{id}/refund/update-status\n  method: post\n  operationId: Report_refund_status_for_sales_credit_note_v1_accounting_sales_credit_note__id__refund_update_status_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounting/sales-invoice/\n  method: post\n  operationId:\
  \ Create_a_sales_invoice_v1_accounting_sales_invoice__post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounting/sales-invoice/{id}\n  method: get\n  operationId: Retrieve_sales_invoice_v1_accounting_sales_invoice__id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounting/sales-invoice/{id}\n  method: patch\n  operationId: Update_sales_invoice_v1_accounting_sales_invoice__id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounting/sales-invoice/{id}/documents\n  method: get\n  operationId: Retrieve_sales_invoice_documents_v1_accounting_sales_invoice__id__documents_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounting/sales-invoice/{id}/payment/update-status\n  method: post\n  operationId: Report_payment_status_for_sales_invoice_v1_accounting_sales_invoice__id__payment_update_status_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounting/sync-tasks\n\
  \  method: get\n  operationId: List_invoices_credit_notes_to_sync_v1_accounting_sync_tasks_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounting/sync-tasks/{id}\n  method: get\n  operationId: Get_details_of_Invoice_Credit_note_to_sync_v1_accounting_sync_tasks__id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounting/sync-tasks/{id}/update-status\n  method: post\n  operationId: Report_sync_status_for_invoice_credit_note_v1_accounting_sync_tasks__id__update_status_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/accounting/tax-rates\n  method: get\n  operationId: List_tax_rates_v1_accounting_tax_rates_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounting/tax-rates/{id}\n  method: get\n  operationId: Retrieve_tax_rate_v1_accounting_tax_rates__id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/documents/document/{id}/download\n  method: get\n  operationId: download_document_v1_documents_document__id__download_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhook/billing-document-update\n  method: post\n  operationId: billing-document-update-webhook\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: https://<accounting-visibility-event-receiving-payload>\n  method: post\n  operationId: Accounting_visibility_eventhttps____accounting_visibility_event_receiving_payload__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounting/company\n  method: get\n  operationId: list_companies__deprecated__v1_accounting_company_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/accounting/company\n  method: post\n  operationId: create_company__deprecated__v1_accounting_company_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounting/company/{id}\n  method: get\n  operationId: get_company__deprecated__v1_accounting_company__id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounting/company/{id}\n  method: put\n  operationId: update_company__deprecated__v1_accounting_company__id__put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounting/company/{id}\n  method: patch\n  operationId: update_company__deprecated__v1_accounting_company__id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounting/company/{id}\n  method: delete\n  operationId: Archive_company__deprecated__v1_accounting_company__id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounting/purchase_invoice/{id}\n  method: get\n  operationId: Retrieve_purchase_invoice__deprecated__v1_accounting_purchase_invoice__id__get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounting/purchase_invoice/{id}\n  method: patch\n  operationId: Update_purchase_invoice__deprecated__v1_accounting_purchase_invoice__id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounting/purchase_invoice/{id}/documents\n  method: get\n  operationId: Retrieve_purchase_invoice_documents__deprecated__v1_accounting_purchase_invoice__id__documents_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounting/purchase_invoice/{id}/payment/update-status\n\
  \  method: post\n  operationId: Report_payment_status_for_purchase_invoice__deprecated__v1_accounting_purchase_invoice__id__payment_update_status_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounting/sales_credit_note/{id}\n  method: get\n  operationId: Retrieve_sales_credit_note__deprecated__v1_accounting_sales_credit_note__id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounting/sales_credit_note/{id}\n  method: patch\n  operationId: Update_credit_note__deprecated__v1_accounting_sales_credit_note__id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounting/sales_credit_note/{id}/documents\n  method: get\n  operationId: Retrieve_sales_credit_note_documents__deprecated__v1_accounting_sales_credit_note__id__documents_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounting/sales_credit_note/{id}/refund/update-status\n  method: post\n  operationId: Report_refund_status_for_sales_credit_note__deprecated__v1_accounting_sales_credit_note__id__refund_update_status_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounting/sales_invoice/{id}\n  method: get\n  operationId: Retrieve_sales_invoice__deprecated__v1_accounting_sales_invoice__id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounting/sales_invoice/{id}\n  method: patch\n  operationId: Update_sales_invoice__deprecated__v1_accounting_sales_invoice__id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounting/sales_invoice/{id}/documents\n  method: get\n  operationId: Retrieve_sales_invoice_documents__deprecated__v1_accounting_sales_invoice__id__documents_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounting/sales_invoice/{id}/payment/update-status\n  method: post\n  operationId: Report_payment_status_for_sales_invoice__deprecated__v1_accounting_sales_invoice__id__payment_update_status_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/orders/order/upload\n  method: post\n  operationId: import_order_v1_orders_order_upload_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n   \
  \ escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/orders/order/upload/{upload_id}\n  method: get\n  operationId: get_order_import_status_v1_orders_order_upload__upload_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/orders/order/{order_id}\n  method: get\n  operationId: get_order_details_v1_orders_order__order_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/orders/order/{order_id}/charges\n  method: get\n  operationId: List_Order_Charges_v1_orders_order__order_id__charges_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/orders/order/{order_id}/charges/approval\n\
  \  method: post\n  operationId: Approve_Order_Charges_v1_orders_order__order_id__charges_approval_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/orders/order/{order_id}/documents\n  method: get\n  operationId: list_order_documents_v1_orders_order__order_id__documents_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/orders/order/{order_id}/export\n  method: get\n  operationId: order_export_v1_orders_order__order_id__export_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/orders/order/{order_id}/status\n  method: get\n  operationId: order_status_v1_orders_order__order_id__status_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: https://<visibility-event-receiving-endpoint>\n  method: post\n  operationId: operational_visibility_event_webhook_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/documents/document/upload_content\n  method: post\n  operationId: Upload_document_content_v1_documents_document_upload_content_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhook/document-import\n  method: post\n  operationId: document-import-webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhook/fleet-document-upload\n  method: post\n  operationId: fleet-document-upload-webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/webhook/subco-document-upload\n  method: post\n\
  \  operationId: subcontractor-document-upload-webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/webhook/e-invoicing\n  method: post\n  operationId: e-invoicing-webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhook/fleet-status-update\n  method: post\n  operationId: fleet-status-update-webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: https://<external-fleet-receiving-endpoint>\n  method: post\n  operationId: fleet-dispatch-payload\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/webhook/intermodal-status\n  method: post\n  operationId: intermodal-booking-status-webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: https://<intermodal-booking-receiving-payload>\n  method: post\n  operationId: Intermodal_booking_payloadhttps____intermodal_booking_receiving_payload__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhook/location-booking-update\n  method: post\n  operationId: location-booking-update-webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: https://<location-booking-receiving-endpoint>\n  method: post\n  operationId: location-dispatch-payload\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/companies/company\n  method: get\n  operationId: list_companies_v1_companies_company_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/company\n  method: post\n  operationId: create_company_v1_companies_company_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/companies/company/{company_id}/documents\n  method: get\n  operationId: get_company_documents_v1_companies_company__company_id__documents_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/company/{company_id}/documents\n  method: post\n  operationId: create_company_document_v1_companies_company__company_id__documents_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/companies/company/{company_id}/validity\n  method: get\n  operationId: List_company_validities_v1_companies_company__company_id__validity_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/company/{company_id}/validity\n  method: post\n  operationId: Create_company_validity_request_v1_companies_company__company_id__validity_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/companies/company/{company_id}/validity/{id}\n  method: get\n  operationId: Get_company_validity_v1_companies_company__company_id__validity__id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/company/{company_id}/validity/{id}\n  method: put\n  operationId: Update_company_validity_v1_companies_company__company_id__validity__id__put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/companies/company/{company_id}/validity/{id}\n  method: delete\n  operationId: Delete_company_validity_v1_companies_company__company_id__validity__id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/companies/company/{company_id}/validity/{id}/documents\n  method: get\n  operationId: Get_company_validity_documents_v1_companies_company__company_id__validity__id__documents_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/company/{id}\n  method: get\n  operationId: get_company_v1_companies_company__id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/company/{id}\n  method: put\n  operationId: update_company_v1_companies_company__id__put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/companies/company/{id}\n  method: patch\n  operationId: update_company_v1_companies_company__id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/companies/company/{id}\n  method: delete\n  operationId: Archive_company_v1_companies_company__id__delete\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/resources/resource\n  method: post\n  operationId: Create_resource_v1_resources_resource_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/resources/resource\n  method: get\n  operationId: List_resources_v1_resources_resource_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/resources/resource/{resource_id}\n  method: put\n  operationId: Update_resource_v1_resources_resource__resource_id__put\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/resources/resource/{resource_id}\n  method: patch\n  operationId: Patch_resource_v1_resources_resource__resource_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/resources/resource/{resource_id}\n  method: delete\n  operationId: Archive_resource_v1_resources_resource__resource_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n     \
  \ human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/resources/resource/{resource_id}\n  method: get\n  operationId: Get_resource_v1_resources_resource__resource_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/resources/resource/{resource_id}/unavailability\n  method: get\n  operationId: List_resource_unavailabilities_v1_resources_resource__resource_id__unavailability_get\n  x-agentic-access:\n    action-class: connected\n    consequence: \n\n# --- truncated at 32 KB (40 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/qargo/refs/heads/main/agentic-access/qargo-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qargo/refs/heads/main/agentic-access/qargo-agentic-access.yml
summary_line: 114 operations · 64 acting · 7 human-in-the-loop
tags:
- Company
- Transport Management
- Logistics
- Supply Chain
- Freight
- TMS
- Accounting
- Webhooks
---
