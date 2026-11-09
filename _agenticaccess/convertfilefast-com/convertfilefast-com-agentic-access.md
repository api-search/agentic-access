---
acting_count: 64
action_class_counts:
  acting: 64
  connected: 4
api_specs:
- filename: convertfilefast-com-billing-api-openapi.yml
  format: yaml
  label: convertfilefast-com Billing API
  slug: convertfilefast-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/convertfilefast-com/openapi/convertfilefast-com-billing-api-openapi.yml
- filename: convertfilefast-com-conversion-api-openapi.yml
  format: yaml
  label: convertfilefast-com Conversion API
  slug: convertfilefast-com-conversion-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/convertfilefast-com/openapi/convertfilefast-com-conversion-api-openapi.yml
- filename: convertfilefast-com-data-conversion-api-openapi.yml
  format: yaml
  label: convertfilefast-com Data Conversion API
  slug: convertfilefast-com-data-conversion-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/convertfilefast-com/openapi/convertfilefast-com-data-conversion-api-openapi.yml
- filename: convertfilefast-com-documents-to-pdf-api-openapi.yml
  format: yaml
  label: convertfilefast-com Documents to PDF API
  slug: convertfilefast-com-documents-to-pdf-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/convertfilefast-com/openapi/convertfilefast-com-documents-to-pdf-api-openapi.yml
- filename: convertfilefast-com-documents-to-text-api-openapi.yml
  format: yaml
  label: convertfilefast-com Documents to Text API
  slug: convertfilefast-com-documents-to-text-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/convertfilefast-com/openapi/convertfilefast-com-documents-to-text-api-openapi.yml
- filename: convertfilefast-com-feedback-api-openapi.yml
  format: yaml
  label: convertfilefast-com Feedback API
  slug: convertfilefast-com-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/convertfilefast-com/openapi/convertfilefast-com-feedback-api-openapi.yml
- filename: convertfilefast-com-health-api-openapi.yml
  format: yaml
  label: convertfilefast-com Health API
  slug: convertfilefast-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/convertfilefast-com/openapi/convertfilefast-com-health-api-openapi.yml
- filename: convertfilefast-com-html-to-pdf-api-openapi.yml
  format: yaml
  label: convertfilefast-com HTML to PDF API
  slug: convertfilefast-com-html-to-pdf-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/convertfilefast-com/openapi/convertfilefast-com-html-to-pdf-api-openapi.yml
- filename: convertfilefast-com-image-conversion-api-openapi.yml
  format: yaml
  label: convertfilefast-com Image Conversion API
  slug: convertfilefast-com-image-conversion-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/convertfilefast-com/openapi/convertfilefast-com-image-conversion-api-openapi.yml
- filename: convertfilefast-com-image-operations-api-openapi.yml
  format: yaml
  label: convertfilefast-com Image Operations API
  slug: convertfilefast-com-image-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/convertfilefast-com/openapi/convertfilefast-com-image-operations-api-openapi.yml
- filename: convertfilefast-com-images-to-pdf-api-openapi.yml
  format: yaml
  label: convertfilefast-com Images to PDF API
  slug: convertfilefast-com-images-to-pdf-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/convertfilefast-com/openapi/convertfilefast-com-images-to-pdf-api-openapi.yml
- filename: convertfilefast-com-information-api-openapi.yml
  format: yaml
  label: convertfilefast-com Information API
  slug: convertfilefast-com-information-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/convertfilefast-com/openapi/convertfilefast-com-information-api-openapi.yml
- filename: convertfilefast-com-pdf-operations-api-openapi.yml
  format: yaml
  label: convertfilefast-com PDF Operations API
  slug: convertfilefast-com-pdf-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/convertfilefast-com/openapi/convertfilefast-com-pdf-operations-api-openapi.yml
- filename: convertfilefast-com-pdf-to-others-api-openapi.yml
  format: yaml
  label: convertfilefast-com PDF to Others API
  slug: convertfilefast-com-pdf-to-others-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/convertfilefast-com/openapi/convertfilefast-com-pdf-to-others-api-openapi.yml
consequence_counts:
  physical: 3
  read: 4
  write: 61
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Convertfilefast Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/billing/auto-recharge
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/billing/checkout/credits
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/billing/checkout/subscription
operation_count: 68
overview: 'convertfilefast-com exposes 68 API operations that an AI agent could call, of which 64 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read, 61 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: convertfilefast-com
provider_slug: convertfilefast-com
slug: convertfilefast-com-agentic-access
source_filename: convertfilefast-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/convertfilefast-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 68\n  by_action_class:\n    acting: 64\n    connected: 4\n  by_consequence:\n    write: 61\n    read: 4\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/convert\n  method: post\n  operationId: convert_file_v1_convert_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/convert/from-url\n  method: post\n  operationId: convert_from_url_v1_convert_from_url_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/convert/docx-to-pdf\n  method: post\n  operationId: docx_to_pdf_v2_convert_docx_to_pdf_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/convert/docx-to-txt\n  method: post\n  operationId: docx_to_txt_v2_convert_docx_to_txt_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v2/convert/xlsx-to-pdf\n  method: post\n  operationId: xlsx_to_pdf_v2_convert_xlsx_to_pdf_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/convert/pptx-to-pdf\n  method: post\n  operationId: pptx_to_pdf_v2_convert_pptx_to_pdf_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/convert/ppt-to-pdf\n  method: post\n  operationId: ppt_to_pdf_v2_convert_ppt_to_pdf_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/convert/doc-to-pdf\n  method: post\n  operationId: doc_to_pdf_v2_convert_doc_to_pdf_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/convert/rtf-to-pdf\n  method: post\n  operationId: rtf_to_pdf_v2_convert_rtf_to_pdf_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/convert/odt-to-pdf\n  method: post\n  operationId:\
  \ odt_to_pdf_v2_convert_odt_to_pdf_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/convert/txt-to-pdf\n  method: post\n  operationId: txt_to_pdf_v2_convert_txt_to_pdf_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/convert/csv-to-pdf\n  method: post\n  operationId: csv_to_pdf_v2_convert_csv_to_pdf_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/convert/html-to-pdf\n  method: post\n  operationId: html_to_pdf_v2_convert_html_to_pdf_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/convert/markdown-to-pdf\n  method: post\n  operationId: markdown_to_pdf_v2_convert_markdown_to_pdf_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/convert/url-to-pdf\n  method: post\n  operationId: url_to_pdf_v2_convert_url_to_pdf_post\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/convert/pdf-to-jpg\n  method: post\n  operationId: pdf_to_jpg_v2_convert_pdf_to_jpg_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/convert/pdf-to-png\n  method: post\n  operationId: pdf_to_png_v2_convert_pdf_to_png_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/convert/pdf-to-txt\n\
  \  method: post\n  operationId: pdf_to_txt_v2_convert_pdf_to_txt_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/convert/pdf-to-docx\n  method: post\n  operationId: pdf_to_docx_v2_convert_pdf_to_docx_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/convert/pdf-to-xlsx\n  method: post\n  operationId: pdf_to_xlsx_v2_convert_pdf_to_xlsx_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n \
  \     human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/convert/pdf-to-csv\n  method: post\n  operationId: pdf_to_csv_v2_convert_pdf_to_csv_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/pdf/merge\n  method: post\n  operationId: merge_pdfs_v2_pdf_merge_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/pdf/split\n  method: post\n  operationId: split_pdf_v2_pdf_split_post\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/pdf/compress\n  method: post\n  operationId: compress_pdf_v2_pdf_compress_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/pdf/rotate\n  method: post\n  operationId: rotate_pdf_v2_pdf_rotate_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/pdf/protect\n  method: post\n  operationId:\
  \ protect_pdf_v2_pdf_protect_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/pdf/unlock\n  method: post\n  operationId: unlock_pdf_v2_pdf_unlock_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/pdf/extract-text\n  method: post\n  operationId: extract_text_from_pdf_v2_pdf_extract_text_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v2/convert/jpg-to-png\n  method: post\n  operationId: jpg_to_png_v2_convert_jpg_to_png_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/convert/png-to-jpg\n  method: post\n  operationId: png_to_jpg_v2_convert_png_to_jpg_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/convert/heic-to-jpg\n  method: post\n  operationId: heic_to_jpg_v2_convert_heic_to_jpg_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/convert/heic-to-png\n  method: post\n  operationId: heic_to_png_v2_convert_heic_to_png_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/convert/webp-to-jpg\n  method: post\n  operationId: webp_to_jpg_v2_convert_webp_to_jpg_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/convert/webp-to-png\n  method:\
  \ post\n  operationId: webp_to_png_v2_convert_webp_to_png_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/convert/avif-to-jpg\n  method: post\n  operationId: avif_to_jpg_v2_convert_avif_to_jpg_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/convert/avif-to-png\n  method: post\n  operationId: avif_to_png_v2_convert_avif_to_png_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/convert/svg-to-png\n  method: post\n  operationId: svg_to_png_v2_convert_svg_to_png_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/convert/svg-to-jpg\n  method: post\n  operationId: svg_to_jpg_v2_convert_svg_to_jpg_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/convert/bmp-to-jpg\n  method: post\n  operationId: bmp_to_jpg_v2_convert_bmp_to_jpg_post\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/convert/bmp-to-png\n  method: post\n  operationId: bmp_to_png_v2_convert_bmp_to_png_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/convert/tiff-to-jpg\n  method: post\n  operationId: tiff_to_jpg_v2_convert_tiff_to_jpg_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/convert/tiff-to-png\n\
  \  method: post\n  operationId: tiff_to_png_v2_convert_tiff_to_png_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/convert/jpg-to-webp\n  method: post\n  operationId: jpg_to_webp_v2_convert_jpg_to_webp_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/convert/png-to-webp\n  method: post\n  operationId: png_to_webp_v2_convert_png_to_webp_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/convert/jpg-to-pdf\n  method: post\n  operationId: jpg_to_pdf_v2_convert_jpg_to_pdf_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/convert/png-to-pdf\n  method: post\n  operationId: png_to_pdf_v2_convert_png_to_pdf_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/convert/heic-to-pdf\n  method: post\n  operationId: heic_to_pdf_v2_convert_heic_to_pdf_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/convert/webp-to-pdf\n  method: post\n  operationId: webp_to_pdf_v2_convert_webp_to_pdf_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/convert/avif-to-pdf\n  method: post\n  operationId: avif_to_pdf_v2_convert_avif_to_pdf_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v2/convert/svg-to-pdf\n  method: post\n  operationId: svg_to_pdf_v2_convert_svg_to_pdf_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/convert/bmp-to-pdf\n  method: post\n  operationId: bmp_to_pdf_v2_convert_bmp_to_pdf_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/convert/tiff-to-pdf\n  method: post\n  operationId: tiff_to_pdf_v2_convert_tiff_to_pdf_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/convert/images-to-pdf\n  method: post\n  operationId: images_to_pdf_v2_convert_images_to_pdf_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/image/resize\n  method: post\n  operationId: resize_image_v2_image_resize_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/image/compress\n  method: post\n  operationId: compress_image_v2_image_compress_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/convert/json-to-csv\n  method: post\n  operationId: json_to_csv_v2_convert_json_to_csv_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/convert/csv-to-json\n  method: post\n  operationId: csv_to_json_endpoint_v2_convert_csv_to_json_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /v2/convert/csv-to-xlsx\n  method: post\n  operationId: csv_to_xlsx_endpoint_v2_convert_csv_to_xlsx_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/convert/xlsx-to-csv\n  method: post\n  operationId: xlsx_to_csv_endpoint_v2_convert_xlsx_to_csv_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/feedback\n  method: post\n  operationId: submit_feedback_v2_feedback_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/billing/status\n  method: get\n  operationId: get_billing_status_v2_billing_status_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/billing/checkout/subscription\n  method: post\n  operationId: create_subscription_checkout_v2_billing_checkout_subscription_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/billing/checkout/credits\n  method: post\n  operationId: create_credit_checkout_v2_billing_checkout_credits_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/billing/portal\n  method: post\n  operationId: create_billing_portal_link_v2_billing_portal_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/billing/auto-recharge\n  method: get\n  operationId: get_auto_recharge_status_v2_billing_auto_recharge_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/billing/auto-recharge\n\
  \  method: post\n  operationId: update_auto_recharge_settings_v2_billing_auto_recharge_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /health\n  method: get\n  operationId: health_check_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/info\n  method: get\n  operationId: api_info_v1_info_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/convertfilefast-com/agentic-access/convertfilefast-com-agentic-access.yml
summary_line: 68 operations · 64 acting
tags:
- Company
- File Conversion
- PDF
- Developer Tools
---
