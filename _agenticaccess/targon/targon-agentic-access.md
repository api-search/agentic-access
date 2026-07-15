---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 2
api_specs:
- filename: targon-openapi.yml
  format: yaml
  label: Targon Chat Completions API
  slug: targon-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/targon/refs/heads/main/openapi/targon-openapi.yml
- filename: targon-openapi.yml
  format: yaml
  label: Targon Completions API
  slug: targon-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/targon/refs/heads/main/openapi/targon-openapi.yml
- filename: targon-openapi.yml
  format: yaml
  label: Targon Models API
  slug: targon-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/targon/refs/heads/main/openapi/targon-openapi.yml
- filename: targon-openapi.yml
  format: yaml
  label: Targon Images API
  slug: targon-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/targon/refs/heads/main/openapi/targon-openapi.yml
- filename: targon-openapi.yml
  format: yaml
  label: Targon Search API
  slug: targon-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/targon/refs/heads/main/openapi/targon-openapi.yml
consequence_counts:
  read: 2
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Targon Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Targon exposes 6 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Targon
provider_slug: targon
slug: targon-agentic-access
source_filename: targon-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/targon-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    acting: 4\n    connected: 2\n  by_consequence:\n    write: 4\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /chat/completions\n  method: post\n  operationId: createChatCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /completions\n  method: post\n  operationId: createCompletion\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /models\n  method: get\n  operationId: listModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /models/{model}\n  method: get\n  operationId: retrieveModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /images/generations\n  method: post\n  operationId: createImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /search\n  method: post\n  operationId: createSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/targon/refs/heads/main/agentic-access/targon-agentic-access.yml
summary_line: 6 operations · 4 acting
tags:
- AI
- LLM
- Inference
- Decentralized
- Bittensor
---
