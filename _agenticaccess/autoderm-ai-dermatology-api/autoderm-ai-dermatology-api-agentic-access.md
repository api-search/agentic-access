---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 12
api_specs:
- filename: autoderm-ai-dermatology-api-device-api-openapi.yml
  format: yaml
  label: Autoderm – AI Dermatology API Device API
  slug: autoderm-ai-dermatology-api-device-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autoderm-ai-dermatology-api/refs/heads/main/openapi/autoderm-ai-dermatology-api-device-api-openapi.yml
- filename: autoderm-ai-dermatology-api-inference-api-openapi.yml
  format: yaml
  label: Autoderm – AI Dermatology API Inference API
  slug: autoderm-ai-dermatology-api-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autoderm-ai-dermatology-api/refs/heads/main/openapi/autoderm-ai-dermatology-api-inference-api-openapi.yml
- filename: autoderm-ai-dermatology-api-system-api-openapi.yml
  format: yaml
  label: Autoderm – AI Dermatology API System API
  slug: autoderm-ai-dermatology-api-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autoderm-ai-dermatology-api/refs/heads/main/openapi/autoderm-ai-dermatology-api-system-api-openapi.yml
- filename: autoderm-ai-dermatology-api-utils-api-openapi.yml
  format: yaml
  label: Autoderm – AI Dermatology API Utils API
  slug: autoderm-ai-dermatology-api-utils-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autoderm-ai-dermatology-api/refs/heads/main/openapi/autoderm-ai-dermatology-api-utils-api-openapi.yml
consequence_counts:
  read: 12
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Autoderm Ai Dermatology Api Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'Autoderm – AI Dermatology API exposes 17 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Autoderm – AI Dermatology API
provider_slug: autoderm-ai-dermatology-api
slug: autoderm-ai-dermatology-api-agentic-access
source_filename: autoderm-ai-dermatology-api-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: generated\nsource: openapi/autoderm-ai-dermatology-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 12\n    acting: 5\n  by_consequence:\n    read: 12\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /healthz\n  method: get\n  operationId: get_health_healthz_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /healthz\n  method: head\n  operationId: get_health_healthz_head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n\
  \  method: get\n  operationId: get_health_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: head\n  operationId: get_health_health_head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /version\n  method: get\n  operationId: get_version_version_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/system/healthz\n  method: get\n  operationId: get_health_v1_system_healthz_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/system/healthz\n  method: head\n  operationId: get_health_v1_system_healthz_head\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/system/health\n  method: get\n  operationId: get_health_v1_system_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/system/health\n  method: head\n  operationId: get_health_v1_system_health_head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/system/version\n  method: get\n  operationId: get_version_v1_system_version_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/label\n  method: get\n  operationId: get_label_v1_label_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/utils/detect-blur\n  method: post\n  operationId: detect_blur_v1_utils_detect_blur_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/infer-genitals/v1\n  method: post\n  operationId: infer_genitals_v1_v1_infer_genitals_v1_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/infer-age/v1\n  method: post\n  operationId: infer_age_v1_v1_infer_age_v1_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/infer-diseases/v1\n  method: post\n  operationId: infer_diseases_v1_v1_infer_diseases_v1_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/infer-diseases/v1/diseases\n  method: get\n  operationId: get_disease_catalog_v1_v1_infer_diseases_v1_diseases_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/infer-skin-tone/v1\n  method: post\n  operationId: infer_skin_tone_v1_v1_infer_skin_tone_v1_post\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autoderm-ai-dermatology-api/refs/heads/main/agentic-access/autoderm-ai-dermatology-api-agentic-access.yml
summary_line: 17 operations · 5 acting
tags:
- dermatology-api
- ai-dermatology
- Medical Imaging
- Telemedicine
- skin-analysis
- REST API
- OpenAPI
- llms-txt
- ce-marked
- White Label
- Healthcare
- Medical AI
- Computer-Vision
- Medical Device
- ICD-10
- image-classification
- Clinical Decision Support
- triage
---
