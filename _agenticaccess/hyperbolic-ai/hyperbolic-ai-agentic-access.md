---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 1
api_specs:
- filename: hyperbolic-chat-completions-api-openapi.yml
  format: yaml
  label: Hyperbolic Chat Completions API
  slug: hyperbolic-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperbolic-ai/refs/heads/main/openapi/hyperbolic-chat-completions-api-openapi.yml
- filename: hyperbolic-completions-api-openapi.yml
  format: yaml
  label: Hyperbolic Completions API
  slug: hyperbolic-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperbolic-ai/refs/heads/main/openapi/hyperbolic-completions-api-openapi.yml
- filename: hyperbolic-image-generation-api-openapi.yml
  format: yaml
  label: Hyperbolic Image Generation API
  slug: hyperbolic-image-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperbolic-ai/refs/heads/main/openapi/hyperbolic-image-generation-api-openapi.yml
- filename: hyperbolic-audio-generation-api-openapi.yml
  format: yaml
  label: Hyperbolic Audio Generation API
  slug: hyperbolic-audio-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperbolic-ai/refs/heads/main/openapi/hyperbolic-audio-generation-api-openapi.yml
- filename: hyperbolic-models-api-openapi.yml
  format: yaml
  label: Hyperbolic Models API
  slug: hyperbolic-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperbolic-ai/refs/heads/main/openapi/hyperbolic-models-api-openapi.yml
consequence_counts:
  read: 1
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Hyperbolic Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Hyperbolic exposes 5 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Hyperbolic
provider_slug: hyperbolic-ai
slug: hyperbolic-ai-agentic-access
source_filename: hyperbolic-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/hyperbolic-audio-generation-api-openapi.yml, openapi/hyperbolic-chat-completions-api-openapi.yml,\n  openapi/hyperbolic-completions-api-openapi.yml, openapi/hyperbolic-image-generation-api-openapi.yml,\n  openapi/hyperbolic-models-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    acting: 4\n    connected: 1\n  by_consequence:\n    write: 4\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /audio/generation\n  method: post\n  operationId: generateAudio\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chat/completions\n  method: post\n  operationId: createChatCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /completions\n  method: post\n  operationId: createCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /image/generation\n  method: post\n  operationId: generateImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n    \
  \  max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /models\n  method: get\n  operationId: listModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyperbolic-ai/refs/heads/main/agentic-access/hyperbolic-ai-agentic-access.yml
summary_line: 5 operations · 4 acting
tags:
- AI
- Artificial Intelligence
- Compute
- Decentralized
- DePIN
- GPU
- Image Generation
- Inference
- LLM
- Marketplace
- Open Source
---
