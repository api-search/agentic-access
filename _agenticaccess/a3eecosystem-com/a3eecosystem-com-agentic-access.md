---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 3
api_specs:
- filename: a3eecosystem-com-audio-api-openapi.yml
  format: yaml
  label: A3E Ecosystem Inc. Audio API
  slug: a3eecosystem-com-audio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/a3eecosystem-com/openapi/a3eecosystem-com-audio-api-openapi.yml
- filename: a3eecosystem-com-auth-api-openapi.yml
  format: yaml
  label: A3E Ecosystem Inc. Auth API
  slug: a3eecosystem-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/a3eecosystem-com/openapi/a3eecosystem-com-auth-api-openapi.yml
- filename: a3eecosystem-com-document-api-openapi.yml
  format: yaml
  label: A3E Ecosystem Inc. Document API
  slug: a3eecosystem-com-document-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/a3eecosystem-com/openapi/a3eecosystem-com-document-api-openapi.yml
- filename: a3eecosystem-com-email-api-openapi.yml
  format: yaml
  label: A3E Ecosystem Inc. Email API
  slug: a3eecosystem-com-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/a3eecosystem-com/openapi/a3eecosystem-com-email-api-openapi.yml
- filename: a3eecosystem-com-qr-api-openapi.yml
  format: yaml
  label: A3E Ecosystem Inc. Qr API
  slug: a3eecosystem-com-qr-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/a3eecosystem-com/openapi/a3eecosystem-com-qr-api-openapi.yml
- filename: a3eecosystem-com-saas-api-openapi.yml
  format: yaml
  label: A3E Ecosystem Inc. Saas API
  slug: a3eecosystem-com-saas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/a3eecosystem-com/openapi/a3eecosystem-com-saas-api-openapi.yml
- filename: a3eecosystem-com-web-api-openapi.yml
  format: yaml
  label: A3E Ecosystem Inc. Web API
  slug: a3eecosystem-com-web-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/a3eecosystem-com/openapi/a3eecosystem-com-web-api-openapi.yml
consequence_counts:
  read: 3
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: A3Eecosystem Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 18
overview: 'A3E Ecosystem Inc. exposes 18 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 15 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: A3E Ecosystem Inc.
provider_slug: a3eecosystem-com
slug: a3eecosystem-com-agentic-access
source_filename: a3eecosystem-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/a3eecosystem-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    acting: 15\n    connected: 3\n  by_consequence:\n    write: 15\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/audio/tts\n  method: post\n  operationId: post_v1_audio_tts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/audio/tts/voices\n  method: get\n  operationId: get_v1_audio_tts_voices\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/auth/signup\n  method: post\n  operationId: post_v1_auth_signup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/document/pdf-compress\n  method: post\n  operationId: post_v1_document_pdf_compress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/document/pdf-merge\n  method: post\n  operationId: post_v1_document_pdf_merge\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/document/pdf-split\n  method: post\n  operationId: post_v1_document_pdf_split\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/document/pdf-to-image\n  method: post\n  operationId: post_v1_document_pdf_to_image\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/email/verify\n  method: post\n  operationId:\
  \ post_v1_email_verify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/qr/generate\n  method: post\n  operationId: post_v1_qr_generate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/saas/monitor/check/{monitor_id}\n  method: post\n  operationId: post_v1_saas_monitor_check_monitor_id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/saas/monitor/create\n  method: post\n  operationId: post_v1_saas_monitor_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/saas/uptime/check/{monitor_id}\n  method: post\n  operationId: post_v1_saas_uptime_check_monitor_id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/saas/uptime/create\n  method: post\n  operationId: post_v1_saas_uptime_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/saas/uptime/list\n  method: get\n  operationId: get_v1_saas_uptime_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/saas/uptime/status/{monitor_id}\n  method: get\n  operationId: get_v1_saas_uptime_status_monitor_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/web/pdf-render\n  method: post\n  operationId: post_v1_web_pdf_render\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/web/screenshot\n  method: post\n  operationId: post_v1_web_screenshot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/web/seo-audit\n  method: post\n  operationId: post_v1_web_seo_audit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/a3eecosystem-com/agentic-access/a3eecosystem-com-agentic-access.yml
summary_line: 18 operations · 15 acting
tags:
- Data
- Artificial Intelligence
- Small Business
- Toronto
- Company
---
