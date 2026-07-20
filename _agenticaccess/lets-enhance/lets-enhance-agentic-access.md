---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 8
api_specs:
- filename: lets-enhance-claid-openapi.json
  format: json
  label: Claid API
  slug: claid
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lets-enhance/refs/heads/main/openapi/lets-enhance-claid-openapi.json
consequence_counts:
  read: 8
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Lets Enhance Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 20
overview: 'Let''s Enhance exposes 20 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 12 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Let's Enhance
provider_slug: lets-enhance
slug: lets-enhance-agentic-access
source_filename: lets-enhance-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/lets-enhance-claid-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    acting: 12\n    connected: 8\n  by_consequence:\n    write: 12\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/scene/create\n  method: post\n  operationId: create_scene_api_v1_scene_create_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - image_generation\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/image/ai-fashion-models\n  method: post\n\
  \  operationId: async_try_on_generation_api_v1_image_ai_fashion_models_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - image_editing\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/image/ai-fashion-models/{processing_request_id}\n  method: get\n  operationId: async_try_on_generation_async_status_v1_image_ai_fashion_models__processing_request_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - image_editing\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/image/ai-edit\n  method: post\n  operationId: async_ai_edit_generation_api_v1_image_ai_edit_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - image_editing\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/image/ai-edit/{ai_edit_id}\n  method: get\n  operationId: async_ai_edit_generation_api_status_v1_image_ai_edit__ai_edit_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - image_editing\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/image/edit\n  method: post\n  operationId: image_edit_v1_image_edit_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - image_editing\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/image/edit/async\n  method: post\n  operationId: async_image_edit_v1_image_edit_async_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - image_editing\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/image/edit/async/{task_id}\n  method: get\n  operationId: async_image_edit_result_v1_image_edit_async__task_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - image_editing\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/image/edit/batch\n  method: post\n  operationId: process_batch_image_edit_v1_image_edit_batch_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - image_editing\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/image/edit/batch/{task_id}\n  method: get\n  operationId: image_edit_batch_async_results_v1_image_edit_batch__task_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - image_editing\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/image/edit/upload\n  method: post\n  operationId: image_edit_upload_v1_image_edit_upload_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - image_editing\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/image/generate\n  method: post\n  operationId: image_generate_v1_image_generate_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - image_editing\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/video/generate\n  method: post\n  operationId: video_generate_api_v1_video_generate_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - video_generation\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/video/generate/{animation_id}\n  method: get\n  operationId: video_generate_api_status_v1_video_generate__animation_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - video_generation\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/storage/storage-types\n  method: get\n  operationId: list_storage_types_v1_storage_storage_types_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - storage\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/storage/storages\n  method: get\n  operationId: list_storages_v1_storage_storages_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - storage\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/storage/storages\n  method: post\n  operationId: create_storage_v1_storage_storages_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - storage\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/storage/storages/{storage_id}\n  method: get\n  operationId: get_storage_v1_storage_storages__storage_id__get\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - storage\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/storage/storages/{storage_id}\n  method: delete\n  operationId: delete_storage_v1_storage_storages__storage_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - storage\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/storage/storages/{storage_id}\n  method: patch\n  operationId: patch_storage_v1_storage_storages__storage_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - storage\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lets-enhance/refs/heads/main/agentic-access/lets-enhance-agentic-access.yml
summary_line: 20 operations · 12 acting
tags:
- Company
- Artificial Intelligence
- Image Processing
- Image Enhancement
- Image Generation
- Computer Vision
- Ecommerce
- Media
- Photography
- Video Generation
---
