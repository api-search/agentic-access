---
acting_count: 26
action_class_counts:
  acting: 26
  connected: 6
api_specs:
- filename: auto-reader-com-ask-api-openapi.yml
  format: yaml
  label: Auto Reader Ask API
  slug: auto-reader-com-ask-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auto-reader-com/openapi/auto-reader-com-ask-api-openapi.yml
- filename: auto-reader-com-book-api-openapi.yml
  format: yaml
  label: Auto Reader Book API
  slug: auto-reader-com-book-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auto-reader-com/openapi/auto-reader-com-book-api-openapi.yml
- filename: auto-reader-com-correct-api-openapi.yml
  format: yaml
  label: Auto Reader Correct API
  slug: auto-reader-com-correct-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auto-reader-com/openapi/auto-reader-com-correct-api-openapi.yml
- filename: auto-reader-com-data-api-openapi.yml
  format: yaml
  label: Auto Reader Data API
  slug: auto-reader-com-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auto-reader-com/openapi/auto-reader-com-data-api-openapi.yml
- filename: auto-reader-com-detect-api-openapi.yml
  format: yaml
  label: Auto Reader Detect API
  slug: auto-reader-com-detect-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auto-reader-com/openapi/auto-reader-com-detect-api-openapi.yml
- filename: auto-reader-com-document-api-openapi.yml
  format: yaml
  label: Auto Reader Document API
  slug: auto-reader-com-document-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auto-reader-com/openapi/auto-reader-com-document-api-openapi.yml
- filename: auto-reader-com-export-api-openapi.yml
  format: yaml
  label: Auto Reader Export API
  slug: auto-reader-com-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auto-reader-com/openapi/auto-reader-com-export-api-openapi.yml
- filename: auto-reader-com-extract-api-openapi.yml
  format: yaml
  label: Auto Reader Extract API
  slug: auto-reader-com-extract-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auto-reader-com/openapi/auto-reader-com-extract-api-openapi.yml
- filename: auto-reader-com-feedback-api-openapi.yml
  format: yaml
  label: Auto Reader Feedback API
  slug: auto-reader-com-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auto-reader-com/openapi/auto-reader-com-feedback-api-openapi.yml
- filename: auto-reader-com-glossary-api-openapi.yml
  format: yaml
  label: Auto Reader Glossary API
  slug: auto-reader-com-glossary-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auto-reader-com/openapi/auto-reader-com-glossary-api-openapi.yml
- filename: auto-reader-com-health-api-openapi.yml
  format: yaml
  label: Auto Reader Health API
  slug: auto-reader-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auto-reader-com/openapi/auto-reader-com-health-api-openapi.yml
- filename: auto-reader-com-internal-api-openapi.yml
  format: yaml
  label: Auto Reader Internal API
  slug: auto-reader-com-internal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auto-reader-com/openapi/auto-reader-com-internal-api-openapi.yml
- filename: auto-reader-com-jobs-api-openapi.yml
  format: yaml
  label: Auto Reader Jobs API
  slug: auto-reader-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auto-reader-com/openapi/auto-reader-com-jobs-api-openapi.yml
- filename: auto-reader-com-manga-api-openapi.yml
  format: yaml
  label: Auto Reader Manga API
  slug: auto-reader-com-manga-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auto-reader-com/openapi/auto-reader-com-manga-api-openapi.yml
- filename: auto-reader-com-ocr-api-openapi.yml
  format: yaml
  label: Auto Reader Ocr API
  slug: auto-reader-com-ocr-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auto-reader-com/openapi/auto-reader-com-ocr-api-openapi.yml
- filename: auto-reader-com-ocr-translate-api-openapi.yml
  format: yaml
  label: Auto Reader Ocr Translate API
  slug: auto-reader-com-ocr-translate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auto-reader-com/openapi/auto-reader-com-ocr-translate-api-openapi.yml
- filename: auto-reader-com-reduce-api-openapi.yml
  format: yaml
  label: Auto Reader Reduce API
  slug: auto-reader-com-reduce-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auto-reader-com/openapi/auto-reader-com-reduce-api-openapi.yml
- filename: auto-reader-com-rewrite-api-openapi.yml
  format: yaml
  label: Auto Reader Rewrite API
  slug: auto-reader-com-rewrite-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auto-reader-com/openapi/auto-reader-com-rewrite-api-openapi.yml
- filename: auto-reader-com-translate-api-openapi.yml
  format: yaml
  label: Auto Reader Translate API
  slug: auto-reader-com-translate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auto-reader-com/openapi/auto-reader-com-translate-api-openapi.yml
consequence_counts:
  read: 6
  write: 26
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Auto Reader Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 32
overview: 'Auto Reader exposes 32 API operations that an AI agent could call, of which 26 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 26 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Auto Reader
provider_slug: auto-reader-com
slug: auto-reader-com-agentic-access
source_filename: auto-reader-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/auto-reader-com.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 32\n  by_action_class:\n    acting: 26\n    connected: 6\n  by_consequence:\n    write: 26\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /internal/quota\n  method: post\n  operationId: internal_quota_internal_quota_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ocr\n  method: post\n  operationId: ocr_multipart_v1_ocr_post\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ocr/base64\n  method: post\n  operationId: ocr_base64_v1_ocr_base64_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/manga\n  method: post\n  operationId: manga_multipart_v1_manga_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/manga/base64\n  method: post\n\
  \  operationId: manga_base64_v1_manga_base64_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/detect\n  method: post\n  operationId: detect_multipart_v1_detect_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/detect/base64\n  method: post\n  operationId: detect_base64_v1_detect_base64_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/extract\n  method: post\n  operationId: extract_multipart_v1_extract_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/extract/base64\n  method: post\n  operationId: extract_base64_v1_extract_base64_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ocr-translate\n  method: post\n  operationId: ocr_translate_multipart_v1_ocr_translate_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n \
  \   audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ocr-translate/base64\n  method: post\n  operationId: ocr_translate_base64_v1_ocr_translate_base64_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/document\n  method: post\n  operationId: document_v1_document_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/book\n  method: post\n  operationId: book_submit_v1_book_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/reduce\n  method: post\n  operationId: reduce_sync_v1_reduce_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/book/{job_id}\n  method: get\n  operationId: book_status_v1_book__job_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/book/{job_id}\n  method: delete\n  operationId: book_delete_v1_book__job_id__delete\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/book/{job_id}/download\n  method: get\n  operationId: book_download_v1_book__job_id__download_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/translate/batch\n  method: post\n  operationId: translate_batch_v1_translate_batch_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/jobs/{job_id}\n  method: get\n  operationId: job_status_v1_jobs__job_id__get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{job_id}\n  method: delete\n  operationId: job_delete_v1_jobs__job_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/feedback\n  method: post\n  operationId: feedback_v1_feedback_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/data\n  method: delete\n  operationId: delete_data_v1_data_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/translate\n  method: post\n  operationId: translate_v1_translate_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/correct\n  method: post\n  operationId: correct_v1_correct_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/rewrite\n  method: post\n  operationId: rewrite_v1_rewrite_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/export\n  method: post\n  operationId: export_document_v1_export_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/glossary\n  method: put\n  operationId: put_glossary_v1_glossary_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/glossary\n \
  \ method: get\n  operationId: get_glossary_v1_glossary_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/glossary\n  method: delete\n  operationId: delete_glossary_v1_glossary_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ask\n  method: post\n  operationId: ask_v1_ask_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /health\n  method: get\n  operationId: health_health_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health/deep\n  method: get\n  operationId: health_deep_health_deep_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/auto-reader-com/agentic-access/auto-reader-com-agentic-access.yml
summary_line: 32 operations · 26 acting
tags:
- Mobile
- Accessibility
- Audio
- eBook
- Offline
---
