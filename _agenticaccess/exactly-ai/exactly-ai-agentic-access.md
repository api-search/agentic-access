---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 8
api_specs:
- filename: exactly-ai-public-openapi-original.json
  format: json
  label: Exactly Public API
  slug: exactly-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exactly-ai/refs/heads/main/openapi/exactly-ai-public-openapi-original.json
consequence_counts:
  read: 8
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Exactly Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 20
overview: 'Exactly Ai exposes 20 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 12 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Exactly Ai
provider_slug: exactly-ai
slug: exactly-ai-agentic-access
source_filename: exactly-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/exactly-ai-public-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    acting: 12\n    connected: 8\n  by_consequence:\n    write: 12\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /public/v1/models/\n  method: post\n  operationId: durer_backend_public_api_api_routes_models_create_model\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v1/models/\n  method: get\n  operationId: durer_backend_public_api_api_routes_models_list_models\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v1/models/{uid}/\n  method: get\n  operationId: durer_backend_public_api_api_routes_models_get_model\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v1/models/{uid}/\n  method: delete\n  operationId: durer_backend_public_api_api_routes_models_delete_model\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v1/models/{uid}/draft/\n  method: post\n  operationId: durer_backend_public_api_api_routes_models_make_model_draft\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v1/models/{uid}/train_images/\n  method: post\n  operationId: durer_backend_public_api_api_routes_models_add_train_image\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v1/models/{uid}/train_images/\n  method: get\n  operationId: durer_backend_public_api_api_routes_models_list_train_images\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v1/models/{uid}/train_images/{image_uid}/\n  method: delete\n  operationId:\
  \ durer_backend_public_api_api_routes_models_delete_item\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v1/models/{uid}/train/\n  method: post\n  operationId: durer_backend_public_api_api_routes_models_run_model_training\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v1/models/{uid}/cancel/\n  method: post\n  operationId: durer_backend_public_api_api_routes_models_cancel_model_training\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v1/models/{uid}/train/progress/\n  method: get\n  operationId: durer_backend_public_api_api_routes_models_get_model_training_progress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v1/models/{uid}/enhance_prompt/\n  method: post\n  operationId: durer_backend_public_api_api_routes_models_enhance_prompt_for_model\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v1/images/\n  method: post\n  operationId: durer_backend_public_api_api_routes_images_generate_images\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v1/images/{uid}/\n  method: get\n  operationId: durer_backend_public_api_api_routes_images_get_image\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v1/images/{uid}/upscales/\n  method: post\n  operationId: durer_backend_public_api_api_routes_images_upscale_image\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v1/images/{uid}/upscales/{scale}/\n\
  \  method: get\n  operationId: durer_backend_public_api_api_routes_images_get_image_upscale\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v1/images/{uid}/vectors/\n  method: post\n  operationId: durer_backend_public_api_api_routes_images_vectorize_image\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v1/images/{uid}/vectors/\n  method: get\n  operationId: durer_backend_public_api_api_routes_images_get_image_vector\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v1/images/{uid}/remove-bg/\n  method: post\n  operationId:\
  \ durer_backend_public_api_api_routes_images_remove_bg_image\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v1/images/{uid}/remove-bg/\n  method: get\n  operationId: durer_backend_public_api_api_routes_images_get_removed_bg_image\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exactly-ai/refs/heads/main/agentic-access/exactly-ai-agentic-access.yml
summary_line: 20 operations · 12 acting
tags:
- Company
- Artificial Intelligence
- Image Generation
- Generative AI
- Creative Tools
- Brand
- Machine Learning
- Media
---
