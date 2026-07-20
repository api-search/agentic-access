---
acting_count: 70
action_class_counts:
  acting: 70
  connected: 108
api_specs:
- filename: alasco-fincon-openapi.json
  format: json
  label: Alasco FinCon API
  slug: alasco-fincon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alasco/refs/heads/main/openapi/alasco-fincon-openapi.json
- filename: alasco-capex-openapi.json
  format: json
  label: Alasco CapEx API
  slug: alasco-capex-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alasco/refs/heads/main/openapi/alasco-capex-openapi.json
- filename: alasco-esg-openapi.json
  format: json
  label: Alasco ESG API
  slug: alasco-esg-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alasco/refs/heads/main/openapi/alasco-esg-openapi.json
consequence_counts:
  physical: 26
  read: 108
  write: 44
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Alasco Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /assets/{id}/submit-invoice/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /change_orders/{change_order_id}/documents/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /change_orders/{change_order_id}/documents/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoices/add-paid-invoice/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoices/add-paid-invoice/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /invoices/{id}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /invoices/{id}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoices/{id}/register-payment/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoices/{id}/register-payment/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoices/{id}/update-new/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoices/{id}/update-new/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoices/{id}/update-paid-invoice/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoices/{id}/update-paid-invoice/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoices/{invoice_id}/documents/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoices/{invoice_id}/documents/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoices/{invoice_id}/tags/assign/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoices/{invoice_id}/tags/assign/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoices/{invoice_id}/tags/unassign/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoices/{invoice_id}/tags/unassign/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /projects/{id}/submit-invoice/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /tags/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /tags/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /tags/{id}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /tags/{id}/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /tags/{id}/
operation_count: 178
overview: 'Alasco exposes 178 API operations that an AI agent could call, of which 70 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 108 read, 44 write, and 26 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Alasco
provider_slug: alasco
slug: alasco-agentic-access
source_filename: alasco-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: generated\nsource: openapi/alasco-capex-openapi.json, openapi/alasco-esg-openapi.json, openapi/alasco-fincon-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 178\n  by_action_class:\n    connected: 108\n    acting: 70\n  by_consequence:\n    read: 108\n    physical: 26\n    write: 44\n  human_in_the_loop_required: 0\noperations:\n- path: /assets/\n  method: get\n  operationId: get_assets_assets__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/{id}/\n  method: get\n  operationId: get_asset_details_assets__id___get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/{id}/submit-invoice/\n  method: post\n  operationId: submit_invoice_assets__id__submit_invoice__post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /change_orders/\n  method: get\n  operationId: get_change_orders_change_orders__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /change_orders/{change_order_id}/documents/\n  method: get\n  operationId: get_change_order_documents_change_orders__change_order_id__documents__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /change_orders/{change_order_id}/documents/\n  method: post\n  operationId: create_change_order_document_change_orders__change_order_id__documents__post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /change_orders/{change_order_id}/documents/{document_id}/\n  method: get\n  operationId: get_change_order_document_change_orders__change_order_id__documents__document_id___get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /change_orders/{change_order_id}/documents/{document_id}/download-annotated/\n  method: get\n\
  \  operationId: download_annotated_change_order_document_change_orders__change_order_id__documents__document_id__download_annotated__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /change_orders/{change_order_id}/documents/{document_id}/download/\n  method: get\n  operationId: download_change_order_document_change_orders__change_order_id__documents__document_id__download__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /change_orders/{id}/\n  method: get\n  operationId: get_change_order_details_change_orders__id___get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracting_entities/\n  method: get\n  operationId: get_contracting_entities_contracting_entities__get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracting_entities/\n  method: post\n  operationId: create_contracting_entity_contracting_entities__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracting_entities/{contracting_entity_id}/contracts/\n  method: get\n  operationId: get_contracts_by_contracting_entity_contracting_entities__contracting_entity_id__contracts__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracting_entities/{id}/\n  method: get\n  operationId: get_contracting_entity_details_contracting_entities__id___get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracting_entities/{id}/\n  method: patch\n  operationId: update_contracting_entity_contracting_entities__id___patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contractors/\n  method: get\n  operationId: get_contractors_contractors__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contractors/\n  method: post\n  operationId: create_contractor_contractors__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contractors/{contractor_id}/contracts/\n  method: get\n  operationId: get_contracts_by_contractor_contractors__contractor_id__contracts__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contractors/{id}/\n  method: get\n  operationId: get_contractor_details_contractors__id___get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contractors/{id}/\n  method: patch\n  operationId: update_contractor_contractors__id___patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contractors/{id}/download-tax-waiver/\n  method: get\n  operationId: download_tax_waiver_contractors__id__download_tax_waiver__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contractors/{id}/upload-tax-waiver/\n  method: post\n  operationId: upload_tax_waiver_contractors__id__upload_tax_waiver__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/\n  method: get\n  operationId: get_contracts_contracts__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /contracts/\n  method: post\n  operationId: create_contract_contracts__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/{contract_id}/change_orders/\n  method: get\n  operationId: get_change_orders_by_contract_contracts__contract_id__change_orders__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts/{contract_id}/contract_terms/\n  method: get\n  operationId: get_contract_terms_contracts__contract_id__contract_terms__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts/{contract_id}/custom_fields/\n\
  \  method: get\n  operationId: get_custom_fields_by_contract_contracts__contract_id__custom_fields__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts/{contract_id}/documents/\n  method: get\n  operationId: get_contract_documents_contracts__contract_id__documents__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts/{contract_id}/documents/\n  method: post\n  operationId: create_contract_document_contracts__contract_id__documents__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/{contract_id}/documents/{document_id}/\n\
  \  method: get\n  operationId: get_contract_document_contracts__contract_id__documents__document_id___get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts/{contract_id}/documents/{document_id}/download/\n  method: get\n  operationId: download_contract_document_contracts__contract_id__documents__document_id__download__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts/{contract_id}/invoices/\n  method: get\n  operationId: get_invoices_by_contract_contracts__contract_id__invoices__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts/{id}/\n  method: get\n  operationId: get_contract_details_contracts__id___get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts/{id}/\n  method: patch\n  operationId: update_contract_contracts__id___patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invoices/\n  method: get\n  operationId: get_invoices_invoices__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoices/add-paid-invoice/\n  method: post\n  operationId: add_paid_invoice_invoices_add_paid_invoice__post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n   \
  \   purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invoices/{id}/\n  method: delete\n  operationId: delete_paid_invoice_invoices__id___delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invoices/{id}/\n  method: get\n  operationId: get_invoice_details_invoices__id___get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoices/{id}/register-payment/\n  method: post\n  operationId: register_payment_invoices__id__register_payment__post\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invoices/{id}/update-new/\n  method: post\n  operationId: update_new_invoices__id__update_new__post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invoices/{id}/update-paid-invoice/\n  method: post\n  operationId: update_paid_invoice_invoices__id__update_paid_invoice__post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invoices/{invoice_id}/documents/\n  method: get\n  operationId: get_invoice_documents_invoices__invoice_id__documents__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoices/{invoice_id}/documents/\n  method: post\n  operationId: create_invoice_document_invoices__invoice_id__documents__post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invoices/{invoice_id}/documents/{document_id}/\n\
  \  method: get\n  operationId: get_invoice_document_invoices__invoice_id__documents__document_id___get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoices/{invoice_id}/documents/{document_id}/download-annotated/\n  method: get\n  operationId: download_annotated_invoice_document_invoices__invoice_id__documents__document_id__download_annotated__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoices/{invoice_id}/documents/{document_id}/download/\n  method: get\n  operationId: download_invoice_document_invoices__invoice_id__documents__document_id__download__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoices/{invoice_id}/tags/\n  method: get\n  operationId:\
  \ get_tags_by_invoice_invoices__invoice_id__tags__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoices/{invoice_id}/tags/assign/\n  method: post\n  operationId: assign_tag_invoices__invoice_id__tags_assign__post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invoices/{invoice_id}/tags/unassign/\n  method: post\n  operationId: unassign_tag_invoices__invoice_id__tags_unassign__post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n   \
  \ escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /measures/\n  method: get\n  operationId: get_measures_measures__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /measures/{id}/\n  method: get\n  operationId: get_measure_measures__id___get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /measures/{id}/contracts/\n  method: get\n  operationId: get_contracts_by_measure_measures__id__contracts__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tags/\n  method: get\n  operationId: get_tags_tags__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tags/\n  method: post\n  operationId: create_tag_tags__post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tags/{id}/\n  method: delete\n  operationId: delete_tag_tags__id___delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tags/{id}/\n  method: patch\n  operationId: update_tag_tags__id___patch\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /buildings/\n  method: get\n  operationId: get_buildings_buildings__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /buildings/{building_uuid}/analysis-result/\n  method: get\n  operationId: get_analysis_result_buildings__building_uuid__analysis_result__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /buildings/{building_uuid}/custom-data/\n  method: get\n  operationId: get_custom_data_buildings__building_uuid__custom_data__get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /buildings/{building_uuid}/utility-meters/\n  method: get\n  operationId: get_utility_meters_buildings__building_uuid__utility_meters__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /buildings/{building_uuid}/utility-meters/{meter_uuid}/readings/\n  method: post\n  operationId: create_utility_meter_reading_buildings__building_uuid__utility_meters__meter_uuid__readings__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /consumption-intervals/\n  method: post\n  operationId: create_consumption_interval_consumption_intervals__post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /consumption-intervals/bulk-partial/\n  method: post\n  operationId: bulk_create_consumption_intervals_partial_consumption_intervals_bulk_partial__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /consumption-intervals/bulk/\n  method: post\n  operationId: bulk_create_consumption_intervals_consumption_intervals_bulk__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n    \
  \  human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /consumption/annual/\n  method: get\n  operationId: get_annual_consumption_consumption_annual__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /consumption/annual/{annual_consumption_id}/\n  method: patch\n  operationId: update_annual_consumption_consumption_annual__annual_consumption_id___patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /file-events/\n  method: get\n  operationId: get_file_events_file_events__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /files/\n  method: delete\n  operationId: delete_file_files__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files/\n  method: post\n  operationId: upload_file_files__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files/metadata/\n  method: get\n  operationId: get_file_metadata_files_metadata__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/metadata/\n\
  \  method: patch\n  operationId: patch_file_metadata_files_metadata__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files/{file_id}/\n  method: get\n  operationId: get_file_files__file_id___get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/{file_id}/external-id/\n  method: post\n  operationId: create_file_external_id_files__file_id__external_id__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /meter-readings/\n  method: post\n  operationId: create_utility_meter_reading_with_external_id_meter_readings__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /meter-readings/bulk/\n  method: post\n  operationId: bulk_create_utility_meter_readings_meter_readings_bulk__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /raw-audit/\n  method: get\n  operationId: get_events_raw_audit__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /raw-user-audit/\n  method: get\n  operationId: get_user_events_raw_user_audit__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenant-consumption-links/\n  method: delete\n  operationId: delete_tenant_consumption_link_tenant_consumption_links__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenant-consumption-links/\n  method: post\n  operationId: create_tenant_consumption_link_tenant_consumption_links__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/\n  method: post\n  operationId: upsert_tenant_tenants__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{external_tenant_id}/attachments/\n  method: post\n  operationId: create_tenant_attachment_tenants__external_tenant_id__attachments__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /utility-data-batch-info/\n  method: post\n  operationId: add_utility_data_batch_info_utility_data_batch_info__post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /utility-meters/\n  method: post\n  operationId: add_utility_meter_utility_meters__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /utility-meters/bulk-import-partial/\n  method: post\n  operationId: bulk_add_utility_meter_import_partial_utility_meters_bulk_import_partial__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /utility-meters/import/\n  method: post\n  operationId: add_utility_meter_import_utility_meters_import__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /utility-meters/{meter_external_id}/\n  method: patch\n  operationId: update_utility_meter_utility_meters__meter_external_id___patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /budget_shifts/\n  method: get\n  operationId: get_budget_shifts_budget_shifts__get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /change_orders/\n  method: get\n  operationId: get_change_orders_change_orders__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /change_orders/{change_order_id}/documents/\n  method: get\n  operationId: get_change_order_documents_change_orders__change_order_id__documents__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /change_orders/{change_order_id}/documents/\n  method: post\n  operationId: create_change_order_document_change_orders__change_order_id__documents__post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /change_orders/{change_order_id}/documents/{document_id}/\n  method: get\n  operationId: get_change_order_document_change_orders__change_order_id__documents__document_id___get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /change_orders/{change_order_id}/documents/{document_id}/download-annotated/\n  method: get\n  operationId: download_annotated_change_order_document_change_orders__change_order_id__documents__document_id__download_annotated__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /change_orders/{change_order_id}/documents/{document_id}/download/\n  method: get\n  operationId: download_change_order_document_change_orders__change_order_id__documents__document_id__download__get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /change_orders/{id}/\n  method: get\n  operationId: get_change_order_details_change_orders__id___get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/\n  method: get\n  operationId: get_contacts_contacts__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/\n  method: post\n  operationId: create_contact_contacts__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/{id}/\n\
  \  method: get\n  operationId: get_contact_details_contacts__id___get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/{id}/\n  method: patch\n  operationId: update_contact_contacts__id___patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contract_units/\n  method: get\n  operationId: get_contract_units_contract_units__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contract_units/\n  method: post\n  operationId: create_contract_unit\n\n# --- truncated at 32 KB (55 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/alasco/refs/heads/main/agentic-access/alasco-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alasco/refs/heads/main/agentic-access/alasco-agentic-access.yml
summary_line: 178 operations · 70 acting
tags:
- Company
- Ai Enterprise Software
- Real Estate
- Construction
- PropTech
- Financial Management
- Cost Management
- Capital Expenditure
- ESG
- Sustainability
---
