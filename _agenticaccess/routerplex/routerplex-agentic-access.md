---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 1
api_specs:
- filename: routerplex-chat-api-openapi.yml
  format: yaml
  label: RouterPlex Chat API
  slug: routerplex-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routerplex/refs/heads/main/openapi/routerplex-chat-api-openapi.yml
- filename: routerplex-images-api-openapi.yml
  format: yaml
  label: RouterPlex Images API
  slug: routerplex-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routerplex/refs/heads/main/openapi/routerplex-images-api-openapi.yml
- filename: routerplex-messages-api-openapi.yml
  format: yaml
  label: RouterPlex Messages API
  slug: routerplex-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routerplex/refs/heads/main/openapi/routerplex-messages-api-openapi.yml
- filename: routerplex-models-api-openapi.yml
  format: yaml
  label: RouterPlex Models API
  slug: routerplex-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routerplex/refs/heads/main/openapi/routerplex-models-api-openapi.yml
- filename: routerplex-responses-api-openapi.yml
  format: yaml
  label: RouterPlex Responses API
  slug: routerplex-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routerplex/refs/heads/main/openapi/routerplex-responses-api-openapi.yml
consequence_counts:
  read: 1
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Routerplex Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'RouterPlex exposes 5 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: RouterPlex
provider_slug: routerplex
slug: routerplex-agentic-access
source_filename: routerplex-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: generated\nsource: openapi/routerplex-inference-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    acting: 4\n    connected: 1\n  by_consequence:\n    write: 4\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /chat/completions\n  method: post\n  operationId: createChatCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /images/generations\n  method: post\n  operationId: createImageGeneration\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /responses\n  method: post\n  operationId: createCodexResponse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages\n  method: post\n  operationId: createMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /models\n  method: get\n  operationId: listModels\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/routerplex/refs/heads/main/agentic-access/routerplex-agentic-access.yml
summary_line: 5 operations · 4 acting
tags:
- LLM
- Artificial Intelligence
- AI Gateway
- Inference
- Model Router
- OpenAI-Compatible
- Anthropic Compatible
- Claude
- GPT
- Gemini
- API Gateway
- Agent Infrastructure
- Developer Tools
- MCP
- LLMOps
---
