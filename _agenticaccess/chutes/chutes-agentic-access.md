---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 9
api_specs:
- filename: chutes-openapi.yml
  format: yaml
  label: Chutes LLM Inference (Chat Completions) API
  slug: chutes-llm-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chutes/refs/heads/main/openapi/chutes-openapi.yml
- filename: chutes-openapi.yml
  format: yaml
  label: Chutes Image / Other Models API
  slug: chutes-image-other-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chutes/refs/heads/main/openapi/chutes-openapi.yml
- filename: chutes-openapi.yml
  format: yaml
  label: Chutes Management (Deploy / List) API
  slug: chutes-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chutes/refs/heads/main/openapi/chutes-openapi.yml
- filename: chutes-openapi.yml
  format: yaml
  label: Chutes Images API
  slug: chutes-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chutes/refs/heads/main/openapi/chutes-openapi.yml
consequence_counts:
  physical: 3
  read: 9
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Chutes Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /chutes/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /chutes/diffusion
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /chutes/vllm
operation_count: 17
overview: 'Chutes exposes 17 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 5 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Chutes
provider_slug: chutes
slug: chutes-agentic-access
source_filename: chutes-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/chutes-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    acting: 8\n    connected: 9\n  by_consequence:\n    write: 5\n    read: 9\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /chat/completions\n  method: post\n  operationId: createChatCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /models\n  method: get\n  operationId: listModels\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chutes/\n  method: get\n  operationId: listChutes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chutes/\n  method: post\n  operationId: deployChute\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chutes/{chute_id_or_name}\n  method: get\n  operationId: getChute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chutes/{chute_id_or_name}\n  method: put\n  operationId: updateChute\n \
  \ x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chutes/{chute_id}\n  method: delete\n  operationId: deleteChute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chutes/code/{chute_id}\n  method: get\n  operationId: getChuteCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chutes/{chute_id}/hf_info\n  method: get\n  operationId: getChuteHfInfo\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chutes/warmup/{chute_id_or_name}\n  method: get\n  operationId: warmupChute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chutes/utilization\n  method: get\n  operationId: getChutesUtilization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chutes/vllm\n  method: post\n  operationId: deployVllmChute\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chutes/diffusion\n  method: post\n  operationId:\
  \ deployDiffusionChute\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /images/\n  method: get\n  operationId: listImages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /images/\n  method: post\n  operationId: createImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /images/{image_id_or_name}\n  method: get\n  operationId: getImage\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /images/{image_id_or_name}\n  method: delete\n  operationId: deleteImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chutes/refs/heads/main/agentic-access/chutes-agentic-access.yml
summary_line: 17 operations · 8 acting
tags:
- AI
- LLM
- Inference
- Serverless
- GPU
- Bittensor
---
