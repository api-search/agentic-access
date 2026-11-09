---
acting_count: 39
action_class_counts:
  acting: 39
  connected: 40
api_specs:
- filename: ordogrid-clients-api-openapi.yml
  format: yaml
  label: OrdoGrid Clients API
  slug: ordogrid-clients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ordogrid/openapi/ordogrid-clients-api-openapi.yml
- filename: ordogrid-credit-notes-api-openapi.yml
  format: yaml
  label: OrdoGrid Credit Notes API
  slug: ordogrid-credit-notes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ordogrid/openapi/ordogrid-credit-notes-api-openapi.yml
- filename: ordogrid-fidelity-api-openapi.yml
  format: yaml
  label: OrdoGrid Fidelity API
  slug: ordogrid-fidelity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ordogrid/openapi/ordogrid-fidelity-api-openapi.yml
- filename: ordogrid-invoices-api-openapi.yml
  format: yaml
  label: OrdoGrid Invoices API
  slug: ordogrid-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ordogrid/openapi/ordogrid-invoices-api-openapi.yml
- filename: ordogrid-meta-api-openapi.yml
  format: yaml
  label: OrdoGrid Meta API
  slug: ordogrid-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ordogrid/openapi/ordogrid-meta-api-openapi.yml
- filename: ordogrid-payments-api-openapi.yml
  format: yaml
  label: OrdoGrid Payments API
  slug: ordogrid-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ordogrid/openapi/ordogrid-payments-api-openapi.yml
- filename: ordogrid-peppol-api-openapi.yml
  format: yaml
  label: OrdoGrid Peppol API
  slug: ordogrid-peppol-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ordogrid/openapi/ordogrid-peppol-api-openapi.yml
- filename: ordogrid-quotes-api-openapi.yml
  format: yaml
  label: OrdoGrid Quotes API
  slug: ordogrid-quotes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ordogrid/openapi/ordogrid-quotes-api-openapi.yml
- filename: ordogrid-receipts-api-openapi.yml
  format: yaml
  label: OrdoGrid Receipts API
  slug: ordogrid-receipts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ordogrid/openapi/ordogrid-receipts-api-openapi.yml
consequence_counts:
  physical: 12
  read: 40
  write: 27
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ordogrid Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/invoices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/v1/invoices/{doc_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/v1/invoices/{doc_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/v1/invoices/{doc_id}/pdf
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/invoices/{doc_id}/status
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/invoices/{invoice_id}/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/invoices/{invoice_id}/payments/{payment_id}/reversals
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/invoices/{invoice_id}/refunds
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/invoices/{invoice_id}/refunds/{refund_id}/reversals
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/peppol/credit-notes/{document_id}/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/peppol/invoices/{document_id}/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/peppol/send
operation_count: 79
overview: 'OrdoGrid exposes 79 API operations that an AI agent could call, of which 39 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 40 read, 27 write, and 12 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: OrdoGrid
provider_slug: ordogrid
slug: ordogrid-agentic-access
source_filename: ordogrid-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/ordogrid-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 79\n  by_action_class:\n    connected: 40\n    acting: 39\n  by_consequence:\n    read: 40\n    write: 27\n    physical: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/clients\n  method: get\n  operationId: get_api_v1_clients_list_clients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/clients\n  method: post\n  operationId: post_api_v1_clients_create_client\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/clients/{client_id}\n  method: get\n  operationId: get_api_v1_clients_get_client\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/clients/{client_id}\n  method: patch\n  operationId: patch_api_v1_clients_update_client\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/credit-notes\n  method: get\n  operationId: get_api_v1_credit_notes_list_credit_note\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/v1/credit-notes\n  method: post\n  operationId: post_api_v1_credit_notes_create_credit_note\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/credit-notes/lookup\n  method: get\n  operationId: get_api_v1_credit_notes_lookup_credit_note\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/credit-notes/{doc_id}\n  method: delete\n  operationId: delete_api_v1_credit_notes_delete_credit_note\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/credit-notes/{doc_id}\n  method: get\n  operationId: get_api_v1_credit_notes_get_credit_note\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/credit-notes/{doc_id}\n  method: patch\n  operationId: patch_api_v1_credit_notes_update_credit_note\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/credit-notes/{doc_id}/pdf\n  method: get\n  operationId: get_api_v1_credit_notes_pdf_credit_note\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/credit-notes/{doc_id}/pdf\n\
  \  method: put\n  operationId: put_api_v1_credit_notes_put_pdf_credit_note\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/credit-notes/{doc_id}/status\n  method: post\n  operationId: post_api_v1_credit_notes_status_credit_note\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/fidelity/cards\n  method: get\n  operationId: get_api_v1_fidelity_list_cards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/v1/fidelity/cards\n  method: post\n  operationId: post_api_v1_fidelity_create_card\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/fidelity/ledger\n  method: get\n  operationId: get_api_v1_fidelity_list_ledger\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/fidelity/members\n  method: get\n  operationId: get_api_v1_fidelity_list_members\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/fidelity/members\n  method: post\n  operationId: post_api_v1_fidelity_create_member\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/fidelity/members/lookup\n  method: get\n  operationId: get_api_v1_fidelity_lookup_member\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/fidelity/members/{member_id}\n  method: get\n  operationId: get_api_v1_fidelity_get_member\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/fidelity/members/{member_id}\n  method: patch\n  operationId: patch_api_v1_fidelity_update_member\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n \
  \   escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/fidelity/members/{member_id}/adjust\n  method: post\n  operationId: post_api_v1_fidelity_adjust_points\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/fidelity/members/{member_id}/balance\n  method: get\n  operationId: get_api_v1_fidelity_get_balance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/fidelity/members/{member_id}/burn\n  method: post\n  operationId: post_api_v1_fidelity_burn_points\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/fidelity/members/{member_id}/earn\n  method: post\n  operationId: post_api_v1_fidelity_earn_points\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/fidelity/program\n  method: get\n  operationId: get_api_v1_fidelity_get_program\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/fidelity/program\n  method: put\n  operationId: put_api_v1_fidelity_upsert_program\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/fidelity/rewards\n  method: get\n  operationId: get_api_v1_fidelity_list_rewards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/fidelity/rewards\n  method: post\n  operationId: post_api_v1_fidelity_create_reward\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/fidelity/rewards/{reward_id}\n  method: get\n  operationId: get_api_v1_fidelity_get_reward\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n \
  \   subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/fidelity/rewards/{reward_id}\n  method: patch\n  operationId: patch_api_v1_fidelity_update_reward\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/fidelity/rewards/{reward_id}/issue\n  method: post\n  operationId: post_api_v1_fidelity_issue_reward\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/invoices\n  method: get\n  operationId: get_api_v1_invoices_list_invoice\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/invoices\n  method: post\n  operationId: post_api_v1_invoices_create_invoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/invoices/lookup\n  method: get\n  operationId: get_api_v1_invoices_lookup_invoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/invoices/payments/lookup\n  method: get\n  operationId: get_api_v1_invoices_lookup_payment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api/v1/invoices/{doc_id}\n  method: delete\n  operationId: delete_api_v1_invoices_delete_invoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/invoices/{doc_id}\n  method: get\n  operationId: get_api_v1_invoices_get_invoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/invoices/{doc_id}\n  method: patch\n  operationId: patch_api_v1_invoices_update_invoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/invoices/{doc_id}/pdf\n  method: get\n  operationId: get_api_v1_invoices_pdf_invoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/invoices/{doc_id}/pdf\n  method: put\n  operationId: put_api_v1_invoices_put_pdf_invoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/invoices/{doc_id}/status\n  method: post\n  operationId: post_api_v1_invoices_status_invoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/invoices/{invoice_id}/payments\n  method: get\n  operationId: get_api_v1_invoices_payment_history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/invoices/{invoice_id}/payments\n  method: post\n  operationId: post_api_v1_invoices_record_payment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/invoices/{invoice_id}/payments/{payment_id}/reversals\n\
  \  method: post\n  operationId: post_api_v1_invoices_reverse_payment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/invoices/{invoice_id}/refunds\n  method: post\n  operationId: post_api_v1_invoices_record_refund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/invoices/{invoice_id}/refunds/{refund_id}/reversals\n  method: post\n  operationId: post_api_v1_invoices_reverse_refund\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/me\n  method: get\n  operationId: get_api_v1_meta_whoami\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/openapi.json\n  method: get\n  operationId: get_api_v1_meta_openapi_document\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/peppol/credit-notes/{document_id}/send\n  method: post\n  operationId: post_api_v1_peppol_send_credit_note\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/peppol/credit-notes/{document_id}/status\n  method: get\n  operationId: get_api_v1_peppol_status_credit_note\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/peppol/documents\n  method: get\n  operationId: get_api_v1_peppol_list_documents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/peppol/documents/{document_id}\n  method: get\n  operationId: get_api_v1_peppol_get_document\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/v1/peppol/documents/{document_id}/pdf\n  method: get\n  operationId: get_api_v1_peppol_get_document_pdf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/peppol/documents/{document_id}/xml\n  method: get\n  operationId: get_api_v1_peppol_get_document_xml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/peppol/inbox\n  method: get\n  operationId: get_api_v1_peppol_list_inbox\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/peppol/invoices/{document_id}/send\n  method: post\n  operationId: post_api_v1_peppol_send_invoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/peppol/invoices/{document_id}/status\n  method: get\n  operationId: get_api_v1_peppol_status_invoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/peppol/participants/{vat_number}\n  method: get\n  operationId: get_api_v1_peppol_lookup_participant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/peppol/send\n  method: post\n  operationId: post_api_v1_peppol_create_and_send\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n\
  \      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/quotes\n  method: get\n  operationId: get_api_v1_quotes_list_quote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/quotes\n  method: post\n  operationId: post_api_v1_quotes_create_quote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/quotes/lookup\n  method: get\n  operationId: get_api_v1_quotes_lookup_quote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/v1/quotes/{doc_id}\n  method: delete\n  operationId: delete_api_v1_quotes_delete_quote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/quotes/{doc_id}\n  method: get\n  operationId: get_api_v1_quotes_get_quote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/quotes/{doc_id}\n  method: patch\n  operationId: patch_api_v1_quotes_update_quote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/quotes/{doc_id}/pdf\n\
  \  method: get\n  operationId: get_api_v1_quotes_pdf_quote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/quotes/{doc_id}/pdf\n  method: put\n  operationId: put_api_v1_quotes_put_pdf_quote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/quotes/{doc_id}/status\n  method: post\n  operationId: post_api_v1_quotes_status_quote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/receipts\n  method:\
  \ get\n  operationId: get_api_v1_receipts_list_receipt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/receipts\n  method: post\n  operationId: post_api_v1_receipts_create_receipt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/receipts/lookup\n  method: get\n  operationId: get_api_v1_receipts_lookup_receipt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/receipts/{doc_id}\n  method: delete\n  operationId: delete_api_v1_receipts_delete_receipt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n   \
  \ subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/receipts/{doc_id}\n  method: get\n  operationId: get_api_v1_receipts_get_receipt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/receipts/{doc_id}\n  method: patch\n  operationId: patch_api_v1_receipts_update_receipt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/receipts/{doc_id}/pdf\n  method: get\n  operationId: get_api_v1_receipts_pdf_receipt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/receipts/{doc_id}/pdf\n  method: put\n  operationId: put_api_v1_receipts_put_pdf_receipt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/receipts/{doc_id}/status\n  method: post\n  operationId: post_api_v1_receipts_status_receipt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/scopes\n  method: get\n  operationId: get_api_v1_meta_list_scopes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/ordogrid/agentic-access/ordogrid-agentic-access.yml
summary_line: 79 operations · 39 acting
tags:
- Invoicing
- PEPPOL
- Belgium
- Software-as-a-Service
- business-documents
---
