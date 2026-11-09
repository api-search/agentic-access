---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 20
api_specs:
- filename: auravms-com-analytics-export-api-openapi.yml
  format: yaml
  label: AuraVMS Analytics & Export API
  slug: auravms-com-analytics-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auravms-com/openapi/auravms-com-analytics-export-api-openapi.yml
- filename: auravms-com-api-key-management-api-openapi.yml
  format: yaml
  label: AuraVMS API Key Management API
  slug: auravms-com-api-key-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auravms-com/openapi/auravms-com-api-key-management-api-openapi.yml
- filename: auravms-com-attachments-api-openapi.yml
  format: yaml
  label: AuraVMS Attachments API
  slug: auravms-com-attachments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auravms-com/openapi/auravms-com-attachments-api-openapi.yml
- filename: auravms-com-authentication-api-openapi.yml
  format: yaml
  label: AuraVMS Authentication API
  slug: auravms-com-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auravms-com/openapi/auravms-com-authentication-api-openapi.yml
- filename: auravms-com-discovery-api-openapi.yml
  format: yaml
  label: AuraVMS Discovery API
  slug: auravms-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auravms-com/openapi/auravms-com-discovery-api-openapi.yml
- filename: auravms-com-draft-rfqs-api-openapi.yml
  format: yaml
  label: AuraVMS Draft RFQs API
  slug: auravms-com-draft-rfqs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auravms-com/openapi/auravms-com-draft-rfqs-api-openapi.yml
- filename: auravms-com-feedback-api-openapi.yml
  format: yaml
  label: AuraVMS Feedback API
  slug: auravms-com-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auravms-com/openapi/auravms-com-feedback-api-openapi.yml
- filename: auravms-com-reference-data-api-openapi.yml
  format: yaml
  label: AuraVMS Reference Data API
  slug: auravms-com-reference-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auravms-com/openapi/auravms-com-reference-data-api-openapi.yml
- filename: auravms-com-rfq-lifecycle-api-openapi.yml
  format: yaml
  label: AuraVMS RFQ Lifecycle API
  slug: auravms-com-rfq-lifecycle-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auravms-com/openapi/auravms-com-rfq-lifecycle-api-openapi.yml
- filename: auravms-com-supplier-management-api-openapi.yml
  format: yaml
  label: AuraVMS Supplier Management API
  slug: auravms-com-supplier-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auravms-com/openapi/auravms-com-supplier-management-api-openapi.yml
consequence_counts:
  physical: 5
  read: 20
  safety-critical: 1
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Auravms Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/api-keys/{key_id}/revoke/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/request-a-feature/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/rfq-item-data/{rfq_item_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/save-rfq-draft/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/send-reminders/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/send-rfq-draft/{rfq_id}/
operation_count: 35
overview: 'AuraVMS exposes 35 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read, 9 write, 5 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AuraVMS
provider_slug: auravms-com
slug: auravms-com-agentic-access
source_filename: auravms-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/auravms-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 35\n  by_action_class:\n    acting: 15\n    connected: 20\n  by_consequence:\n    write: 9\n    read: 20\n    physical: 5\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /api/create-supplier/\n  method: post\n  operationId: post_suppliers_api_create_supplier_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/create-supplier/\n  method: put\n \
  \ operationId: put_suppliers_api_create_supplier_2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/get-suppliers/\n  method: get\n  operationId: get_suppliers_api_get_suppliers_3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/get-supplier-categories/\n  method: get\n  operationId: get_suppliers_api_get_supplier_categories_4\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/get-supplier-stats-data/\n  method: get\n  operationId: get_suppliers_api_get_supplier_stats_data_5\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/create-rfq/\n  method: post\n  operationId: post_rfq-lifecycle_api_create_rfq_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/get-rfq-list/\n  method: get\n  operationId: get_rfq-lifecycle_api_get_rfq_list_2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/get-rfq-items/{rfq_id}/\n  method: get\n  operationId: get_rfq-lifecycle_api_get_rfq_items_rfq_id_3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rfq-item-data/{rfq_item_id}\n  method:\
  \ get\n  operationId: get_rfq-lifecycle_api_rfq_item_data_rfq_item_id_4\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rfq-item-data/{rfq_item_id}\n  method: post\n  operationId: post_rfq-lifecycle_api_rfq_item_data_rfq_item_id_5\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/close-rfq/{rfq_id}/\n  method: post\n  operationId: post_rfq-lifecycle_api_close_rfq_rfq_id_6\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/send-reminders/\n  method: post\n  operationId: post_rfq-lifecycle_api_send_reminders_7\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/get-rfq/\n  method: get\n  operationId: get_rfq-lifecycle_api_get_rfq_8\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/get-rfq-metadata/\n  method: get\n  operationId: get_rfq-lifecycle_api_get_rfq_metadata_9\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/save-rfq-draft/\n\
  \  method: post\n  operationId: post_drafts_api_save_rfq_draft_1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/get-rfq-draft/{rfq_id}/\n  method: get\n  operationId: get_drafts_api_get_rfq_draft_rfq_id_2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/send-rfq-draft/{rfq_id}/\n  method: post\n  operationId: post_drafts_api_send_rfq_draft_rfq_id_3\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/delete-rfq-draft/{rfq_id}/\n  method: delete\n  operationId: delete_drafts_api_delete_rfq_draft_rfq_id_4\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/rfq-item/{rfq_item_id}/attachments/upload/\n  method: post\n  operationId: post_attachments_api_rfq_item_rfq_item_id_attachments_upload_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/rfq-item/{rfq_item_id}/attachments/\n  method: get\n  operationId: get_attachments_api_rfq_item_rfq_item_id_attachments_2\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rfq-attachment/{attachment_id}/\n  method: delete\n  operationId: delete_attachments_api_rfq_attachment_attachment_id_3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/rfq-attachment/{attachment_id}/download/\n  method: get\n  operationId: get_attachments_api_rfq_attachment_attachment_id_download_4\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/supplier-attachment/{attachment_id}/download/\n  method: get\n  operationId: get_attachments_api_supplier_attachment_attachment_id_download_5\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/dashboard-stats/\n  method: get\n  operationId: get_analytics_api_dashboard_stats_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/export-quotation-pdf/{rfq_item_id}/\n  method: get\n  operationId: get_analytics_api_export_quotation_pdf_rfq_item_id_2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/send-rfq-data-file/\n  method: get\n  operationId: get_analytics_api_send_rfq_data_file_3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/get-item-uom/\n  method: get\n  operationId: get_reference_api_get_item_uom_1\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/get-item-product/\n  method: get\n  operationId: get_reference_api_get_item_product_2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/api-keys/\n  method: get\n  operationId: get_api-keys_api_api_keys_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/api-keys/\n  method: post\n  operationId: post_api-keys_api_api_keys_2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/api-keys/{key_id}/revoke/\n\
  \  method: post\n  operationId: post_api-keys_api_api_keys_key_id_revoke_3\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/request-a-feature/\n  method: post\n  operationId: post_feedback_api_request_a_feature_1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/login/\n  method: post\n  operationId: create_jwt_session\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/status\n  method: get\n  operationId: get_public_api_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/async-jobs/{job_id}/\n  method: get\n  operationId: get_async_job_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/auravms-com/agentic-access/auravms-com-agentic-access.yml
summary_line: 35 operations · 15 acting · 1 human-in-the-loop
tags:
- Procurement
- RFQ
- Small Business
- Artificial Intelligence
---
