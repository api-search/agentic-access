---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 16
api_specs:
- filename: docuqueue-com-batch-api-openapi.yml
  format: yaml
  label: docuqueue-com Batch API
  slug: docuqueue-com-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docuqueue-com/openapi/docuqueue-com-batch-api-openapi.yml
- filename: docuqueue-com-conversion-api-openapi.yml
  format: yaml
  label: docuqueue-com Conversion API
  slug: docuqueue-com-conversion-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docuqueue-com/openapi/docuqueue-com-conversion-api-openapi.yml
- filename: docuqueue-com-document-generation-api-openapi.yml
  format: yaml
  label: docuqueue-com Document Generation API
  slug: docuqueue-com-document-generation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docuqueue-com/openapi/docuqueue-com-document-generation-api-openapi.yml
- filename: docuqueue-com-forms-api-openapi.yml
  format: yaml
  label: docuqueue-com Forms API
  slug: docuqueue-com-forms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docuqueue-com/openapi/docuqueue-com-forms-api-openapi.yml
- filename: docuqueue-com-research-api-openapi.yml
  format: yaml
  label: docuqueue-com Research API
  slug: docuqueue-com-research-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docuqueue-com/openapi/docuqueue-com-research-api-openapi.yml
- filename: docuqueue-com-shared-documents-api-openapi.yml
  format: yaml
  label: docuqueue-com Shared Documents API
  slug: docuqueue-com-shared-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docuqueue-com/openapi/docuqueue-com-shared-documents-api-openapi.yml
- filename: docuqueue-com-sharing-api-openapi.yml
  format: yaml
  label: docuqueue-com Sharing API
  slug: docuqueue-com-sharing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docuqueue-com/openapi/docuqueue-com-sharing-api-openapi.yml
- filename: docuqueue-com-system-api-openapi.yml
  format: yaml
  label: docuqueue-com System API
  slug: docuqueue-com-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docuqueue-com/openapi/docuqueue-com-system-api-openapi.yml
- filename: docuqueue-com-templates-api-openapi.yml
  format: yaml
  label: docuqueue-com Templates API
  slug: docuqueue-com-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docuqueue-com/openapi/docuqueue-com-templates-api-openapi.yml
- filename: docuqueue-com-upload-api-openapi.yml
  format: yaml
  label: docuqueue-com Upload API
  slug: docuqueue-com-upload-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docuqueue-com/openapi/docuqueue-com-upload-api-openapi.yml
consequence_counts:
  read: 16
  write: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Docuqueue Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 35
overview: 'docuqueue-com exposes 35 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read and 19 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: docuqueue-com
provider_slug: docuqueue-com
slug: docuqueue-com-agentic-access
source_filename: docuqueue-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/docuqueue-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 35\n  by_action_class:\n    acting: 19\n    connected: 16\n  by_consequence:\n    write: 19\n    read: 16\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/forms/upload\n  method: post\n  operationId: upload_form_api_v1_forms_upload_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/forms/\n  method: get\n  operationId: list_forms_api_v1_forms__get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/forms/{form_id}\n  method: get\n  operationId: get_form_api_v1_forms__form_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/forms/{form_id}\n  method: put\n  operationId: update_form_api_v1_forms__form_id__put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/forms/{form_id}\n  method: delete\n  operationId: delete_form_api_v1_forms__form_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/forms/{form_id}/fill\n  method: post\n  operationId: fill_form_api_v1_forms__form_id__fill_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/forms/{form_id}/fill-batch\n  method: post\n  operationId: fill_form_batch_api_v1_forms__form_id__fill_batch_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/convert\n  method: post\n  operationId: convert_urls_api_v1_convert_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/convert-html\n  method: post\n  operationId: convert_html_api_v1_convert_html_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/create-document\n  method: post\n  operationId: create_document_api_v1_create_document_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/v1/upload\n  method: post\n  operationId: upload_pdf_api_v1_upload_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/status/{job_id}\n  method: get\n  operationId: get_status_api_v1_status__job_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/download/{job_id}\n  method: get\n  operationId: download_pdf_api_v1_download__job_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /d/{slug}\n  method: get\n  operationId: view_shared_document_d__slug__get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/shared/{document_id}/raw\n  method: get\n  operationId: shared_document_raw_api_v1_shared__document_id__raw_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /r/{slug}\n  method: get\n  operationId: view_research_deck_r__slug__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/research/{doc_id}/raw\n  method: get\n  operationId: research_deck_raw_api_v1_research__doc_id__raw_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/health\n  method: get\n  operationId: health_check_api_v1_health_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/templates\n  method: post\n  operationId: create_template_api_v1_templates_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/templates\n  method: get\n  operationId: list_templates_api_v1_templates_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/templates/docx\n  method: post\n  operationId: create_docx_template_api_v1_templates_docx_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n \
  \   escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/templates/{template_id}\n  method: get\n  operationId: get_template_api_v1_templates__template_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/templates/{template_id}\n  method: put\n  operationId: update_template_api_v1_templates__template_id__put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/templates/{template_id}\n  method: delete\n  operationId: delete_template_api_v1_templates__template_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n  \
  \  subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/templates/{template_id}/fill\n  method: post\n  operationId: fill_template_api_v1_templates__template_id__fill_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/templates/{template_id}/fill-batch\n  method: post\n  operationId: fill_template_batch_api_v1_templates__template_id__fill_batch_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/v1/templates/{template_id}/batch-upload\n  method: post\n  operationId: batch_upload_api_v1_templates__template_id__batch_upload_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/templates/{template_id}/batch-generate\n  method: post\n  operationId: batch_generate_api_v1_templates__template_id__batch_generate_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/batch/{batch_id}/status\n  method: get\n  operationId: batch_status_api_v1_batch__batch_id__status_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/batch/{batch_id}/download-zip\n  method: get\n  operationId: batch_download_zip_api_v1_batch__batch_id__download_zip_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/templates/{template_id}/preview\n  method: post\n  operationId: preview_template_api_v1_templates__template_id__preview_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/templates/{template_id}/preview-docx\n  method: get\n  operationId: preview_docx_as_pdf_api_v1_templates__template_id__preview_docx_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/templates/{template_id}/preview-sample\n  method: get\n  operationId: preview_template_sample_api_v1_templates__template_id__preview_sample_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/shared\n  method: get\n  operationId: list_shared_documents_api_v1_shared_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/shared/{document_id}\n  method: delete\n  operationId: delete_shared_document_api_v1_shared__document_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/docuqueue-com/agentic-access/docuqueue-com-agentic-access.yml
summary_line: 35 operations · 19 acting
tags:
- Company
- Artificial Intelligence
- Document Automation
- PDF
- REST API
- MCP
---
