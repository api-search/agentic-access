---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 2
api_specs:
- filename: nscale-chat-api-openapi.yml
  format: yaml
  label: Nscale Chat API
  slug: nscale-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nscale/refs/heads/main/openapi/nscale-chat-api-openapi.yml
- filename: nscale-completions-api-openapi.yml
  format: yaml
  label: Nscale Completions API
  slug: nscale-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nscale/refs/heads/main/openapi/nscale-completions-api-openapi.yml
- filename: nscale-embeddings-api-openapi.yml
  format: yaml
  label: Nscale Embeddings API
  slug: nscale-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nscale/refs/heads/main/openapi/nscale-embeddings-api-openapi.yml
- filename: nscale-images-api-openapi.yml
  format: yaml
  label: Nscale Images API
  slug: nscale-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nscale/refs/heads/main/openapi/nscale-images-api-openapi.yml
- filename: nscale-models-api-openapi.yml
  format: yaml
  label: Nscale Models API
  slug: nscale-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nscale/refs/heads/main/openapi/nscale-models-api-openapi.yml
consequence_counts:
  read: 2
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Nscale Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Nscale exposes 6 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Nscale
provider_slug: nscale
slug: nscale-agentic-access
source_filename: nscale-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/nscale-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    acting: 4\n    connected: 2\n  by_consequence:\n    write: 4\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /chat/completions\n  method: post\n  operationId: createChatCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /completions\n  method: post\n  operationId: createCompletion\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /embeddings\n  method: post\n  operationId: createEmbedding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /images/generations\n  method: post\n  operationId: createImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /models\n  method: get\n  operationId: listModels\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /models/{model}\n  method: get\n  operationId: retrieveModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nscale/refs/heads/main/agentic-access/nscale-agentic-access.yml
summary_line: 6 operations · 4 acting
tags:
- Artificial Intelligence
- GPU
- Inference
- Serverless
- Cloud Compute
---
