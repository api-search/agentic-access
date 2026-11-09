---
acting_count: 17
action_class_counts:
  acting: 17
  connected: 17
api_specs:
- filename: two-api-key-api-openapi.yml
  format: yaml
  label: Two API Key API
  slug: two-api-key-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/two/openapi/two-api-key-api-openapi.yml
- filename: two-invoice-api-openapi.yml
  format: yaml
  label: Two Invoice API
  slug: two-invoice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/two/openapi/two-invoice-api-openapi.yml
- filename: two-order-api-openapi.yml
  format: yaml
  label: Two Order API
  slug: two-order-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/two/openapi/two-order-api-openapi.yml
- filename: two-order-intent-api-openapi.yml
  format: yaml
  label: Two Order intent API
  slug: two-order-intent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/two/openapi/two-order-intent-api-openapi.yml
- filename: two-settlement-report-api-openapi.yml
  format: yaml
  label: Two Settlement report API
  slug: two-settlement-report-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/two/openapi/two-settlement-report-api-openapi.yml
consequence_counts:
  physical: 15
  read: 17
  safety-critical: 1
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Two Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/merchant/{merchant_id}/api_key/{api_key_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoicing/v0/invoice
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/invoice/{invoice_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/invoice/{invoice_id}/emails
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/order/{order_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/order/{order_id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/order/{order_id}/confirm
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/order/{order_id}/fulfillments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/order/{order_id}/fulfillments/complete_partial
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/order/{order_id}/notify
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/order/{order_id}/refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/order/{order_id}/renew
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/order/{order_id}/transactions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/order_intent
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/pricing/order/fee
operation_count: 34
overview: 'Two exposes 34 API operations that an AI agent could call, of which 17 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read, 1 write, 15 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Two
provider_slug: two
slug: two-agentic-access
source_filename: two-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/two-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 34\n  by_action_class:\n    acting: 17\n    connected: 17\n  by_consequence:\n    physical: 15\n    read: 17\n    write: 1\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /v1/order_intent\n  method: post\n  operationId: create_order_intent_handler.post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/order_intent/{order_intent_id}\n\
  \  method: get\n  operationId: get_order_intent_handler.get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/order\n  method: post\n  operationId: create_order_handler.post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pricing/order/fee\n  method: post\n  operationId: calculate_pricing_order_fee_v1_handler.post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /v1/order/{order_id}\n  method: get\n  operationId: get_order_handler.get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/order/{order_id}\n  method: put\n  operationId: edit_order_handler.put\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/order/{order_id}/payment_link\n  method: get\n  operationId: get_order_payment_link_handler.get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/order/merchant-order-id/{merchant_order_id}\n\
  \  method: get\n  operationId: get_orders_by_merchant_order_id_handler.get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/order/{order_id}/confirm\n  method: post\n  operationId: mark_confirmed_order_handler.post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/order/{order_id}/renew\n  method: post\n  operationId: renew_order_handler.post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/order/{order_id}/cancel\n  method: post\n  operationId: cancel_order_handler.post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/order/{order_id}/fulfillments\n  method: get\n  operationId: get_fulfilled_order_handler.get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/order/{order_id}/fulfillments\n  method: post\n  operationId: fulfill_order_handler.post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/order/{order_id}/fulfillments/complete_partial\n  method: post\n  operationId: complete_partial_order_handler.post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/order/{order_id}/invoice_details\n  method: get\n  operationId: get_invoice_details_handler.get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/orders\n  method: get\n  operationId: retrieve_order_list_handler.get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/order/{order_id}/verification_data\n  method: get\n  operationId: get_order_verification_data.get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/order/{order_id}/notify\n  method: post\n  operationId: notify_order_handler.post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/order/{order_id}/refund\n  method: post\n  operationId: refund_order_handler.post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/invoice/{order_id}/pdf\n  method: get\n  operationId: invoice_pdf_handler.get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/invoice/{invoice_id}/document\n  method: get\n  operationId: invoice_document_handler.get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/invoice/pdfs\n  method: get\n  operationId: zipped_invoice_pdfs_handler.get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/invoice/{invoice_id}\n  method:\
  \ patch\n  operationId: edit_invoice.patch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/invoice/{invoice_id}/emails\n  method: put\n  operationId: edit_invoice_emails.put\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invoicing/v0/invoice\n  method: post\n  operationId: invoice_creation_handler.post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tax_codes/{country_code}\n  method: get\n  operationId: get_tax_codes_handler.get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/merchant/{merchant_id}/api_key\n  method: post\n  operationId: create_merchant_api_key_handler.post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/merchant/{merchant_id}/api_key\n  method: get\n  operationId: retrieve_merchant_api_keys_handler.get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/merchant/{merchant_id}/api_key/{api_key_id}\n  method: get\n  operationId: retrieve_merchant_api_key_handler.get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/merchant/{merchant_id}/api_key/{api_key_id}\n  method: delete\n  operationId: revoke_merchant_api_key_handler.delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/merchant/settlement\n  method: get\n  operationId: get_merchant_settlements_v2_handler.get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/merchant/settlement/{settlement_id}/statement\n  method: get\n  operationId: get_merchant_settlement_statement_handler.get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/merchant/statement\n  method: get\n  operationId: get_merchant_statement_handler.get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/order/{order_id}/transactions\n  method: put\n  operationId: update_reconciliation_events_handler.put\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/two/agentic-access/two-agentic-access.yml
summary_line: 34 operations · 17 acting · 1 human-in-the-loop
tags:
- Company
- B2B Payments
- Fintech
- API Platform
- Checkout
- Trade Accounts
---
