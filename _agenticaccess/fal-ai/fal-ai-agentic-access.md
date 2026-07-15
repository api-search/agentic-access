---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 6
api_specs:
- filename: fal-model-apis-openapi.yml
  format: yaml
  label: fal Model APIs
  slug: fal-model-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fal-ai/refs/heads/main/openapi/fal-model-apis-openapi.yml
- filename: fal-ai-asyncapi.yml
  format: yaml
  label: fal Realtime API
  slug: fal-realtime-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/fal-ai/refs/heads/main/asyncapi/fal-ai-asyncapi.yml
- filename: fal-ai-asyncapi.yml
  format: yaml
  label: fal Streaming API
  slug: fal-streaming-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/fal-ai/refs/heads/main/asyncapi/fal-ai-asyncapi.yml
- filename: fal-storage-api-openapi.yml
  format: yaml
  label: fal Storage API
  slug: fal-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fal-ai/refs/heads/main/openapi/fal-storage-api-openapi.yml
- filename: fal-serverless-platform-api-openapi.yml
  format: yaml
  label: fal Serverless Platform API
  slug: fal-serverless-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fal-ai/refs/heads/main/openapi/fal-serverless-platform-api-openapi.yml
consequence_counts:
  read: 6
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Fal Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'fal exposes 11 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: fal
provider_slug: fal-ai
slug: fal-ai-agentic-access
source_filename: fal-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/fal-model-apis-openapi.yml, openapi/fal-serverless-platform-api-openapi.yml,\n  openapi/fal-storage-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    acting: 5\n    connected: 6\n  by_consequence:\n    write: 5\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /{model_owner}/{model_name}\n  method: post\n  operationId: submitRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{model_owner}/{model_name}/requests/{request_id}/status\n\
  \  method: get\n  operationId: getRequestStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{model_owner}/{model_name}/requests/{request_id}\n  method: get\n  operationId: getRequestResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{model_owner}/{model_name}/requests/{request_id}/cancel\n  method: put\n  operationId: cancelRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{model_owner}/{model_name}/stream\n  method: post\n  operationId: streamRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n  \
  \  subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /serverless/apps\n  method: get\n  operationId: listApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /serverless/apps/{app_id}\n  method: get\n  operationId: getApp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /serverless/secrets\n  method: get\n  operationId: listSecrets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /serverless/secrets\n  method: post\n  operationId: setSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n   \
  \ subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /serverless/files\n  method: get\n  operationId: listFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /storage/upload/initiate\n  method: post\n  operationId: initiateUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fal-ai/refs/heads/main/agentic-access/fal-ai-agentic-access.yml
summary_line: 11 operations · 5 acting
tags:
- AI
- Artificial Intelligence
- Generative AI
- Generative Media
- Image Generation
- Video Generation
- Audio Generation
- Inference
- Serverless
- GPU
- MCP
---
