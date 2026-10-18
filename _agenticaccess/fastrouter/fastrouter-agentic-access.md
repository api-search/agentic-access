---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 6
api_specs:
- filename: fastrouter-audio-api-openapi.yml
  format: yaml
  label: Fastrouter Audio API
  slug: fastrouter-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastrouter/refs/heads/main/openapi/fastrouter-audio-api-openapi.yml
- filename: fastrouter-batches-api-openapi.yml
  format: yaml
  label: Fastrouter Batches API
  slug: fastrouter-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastrouter/refs/heads/main/openapi/fastrouter-batches-api-openapi.yml
- filename: fastrouter-embeddings-api-openapi.yml
  format: yaml
  label: Fastrouter Embeddings API
  slug: fastrouter-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastrouter/refs/heads/main/openapi/fastrouter-embeddings-api-openapi.yml
- filename: fastrouter-files-api-openapi.yml
  format: yaml
  label: Fastrouter Files API
  slug: fastrouter-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastrouter/refs/heads/main/openapi/fastrouter-files-api-openapi.yml
- filename: fastrouter-generation-api-openapi.yml
  format: yaml
  label: Fastrouter Generation API
  slug: fastrouter-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastrouter/refs/heads/main/openapi/fastrouter-generation-api-openapi.yml
- filename: fastrouter-getasyncresponse-api-openapi.yml
  format: yaml
  label: Fastrouter Get Async Response API
  slug: fastrouter-getasyncresponse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastrouter/refs/heads/main/openapi/fastrouter-getasyncresponse-api-openapi.yml
- filename: fastrouter-getprompttoaudioresponse-api-openapi.yml
  format: yaml
  label: Fastrouter Get Prompt To Audio Response API
  slug: fastrouter-getprompttoaudioresponse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastrouter/refs/heads/main/openapi/fastrouter-getprompttoaudioresponse-api-openapi.yml
- filename: fastrouter-images-api-openapi.yml
  format: yaml
  label: Fastrouter Images API
  slug: fastrouter-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastrouter/refs/heads/main/openapi/fastrouter-images-api-openapi.yml
- filename: fastrouter-model-api-openapi.yml
  format: yaml
  label: Fastrouter Model API
  slug: fastrouter-model-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastrouter/refs/heads/main/openapi/fastrouter-model-api-openapi.yml
- filename: fastrouter-models-api-openapi.yml
  format: yaml
  label: Fastrouter Models API
  slug: fastrouter-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastrouter/refs/heads/main/openapi/fastrouter-models-api-openapi.yml
- filename: fastrouter-moderations-api-openapi.yml
  format: yaml
  label: Fastrouter Moderations API
  slug: fastrouter-moderations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastrouter/refs/heads/main/openapi/fastrouter-moderations-api-openapi.yml
- filename: fastrouter-responses-api-openapi.yml
  format: yaml
  label: Fastrouter Responses API
  slug: fastrouter-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastrouter/refs/heads/main/openapi/fastrouter-responses-api-openapi.yml
- filename: fastrouter-videos-api-openapi.yml
  format: yaml
  label: Fastrouter Videos API
  slug: fastrouter-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastrouter/refs/heads/main/openapi/fastrouter-videos-api-openapi.yml
- filename: fastrouter-chat-completions-api-openapi.yml
  format: yaml
  label: Fastrouter Chat Completions API
  slug: fastrouter-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fastrouter/refs/heads/main/openapi/fastrouter-chat-completions-api-openapi.yml
consequence_counts:
  read: 6
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Fastrouter Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 19
overview: 'Fastrouter exposes 19 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 13 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Fastrouter
provider_slug: fastrouter
slug: fastrouter-agentic-access
source_filename: fastrouter-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: generated\nsource: openapi/fastrouter-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    acting: 13\n    connected: 6\n  by_consequence:\n    write: 13\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/chat/completions\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/responses\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n   \
  \ audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/model/selection\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/model/selection\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/embeddings\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/moderations\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/images/generations\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/images/edits\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/videos\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/getAsyncResponse\n  method: post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/getPromptToAudioResponse\n  method: post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/audio/transcriptions\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/audio/translations\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/generation\n  method: post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/files\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /v1/batches\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/batches/{batch_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/files/{file_id}/content\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/models\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fastrouter/refs/heads/main/agentic-access/fastrouter-agentic-access.yml
summary_line: 19 operations · 13 acting
tags:
- Company
- Artificial Intelligence
- API Gateway
- LLM
- Enterprise
---
