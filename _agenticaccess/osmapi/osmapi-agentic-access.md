---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 2
api_specs:
- filename: osmapi-chat-completions-openapi.yml
  format: yaml
  label: osmAPI Chat Completions API
  slug: osmapi-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osmapi/refs/heads/main/openapi/osmapi-chat-completions-openapi.yml
- filename: osmapi-anthropic-messages-openapi.yml
  format: yaml
  label: osmAPI Anthropic Messages API
  slug: osmapi-anthropic-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osmapi/refs/heads/main/openapi/osmapi-anthropic-messages-openapi.yml
- filename: osmapi-models-openapi.yml
  format: yaml
  label: osmAPI Models API
  slug: osmapi-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osmapi/refs/heads/main/openapi/osmapi-models-openapi.yml
- filename: osmapi-health-openapi.yml
  format: yaml
  label: osmAPI Health API
  slug: osmapi-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osmapi/refs/heads/main/openapi/osmapi-health-openapi.yml
consequence_counts:
  read: 2
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Osmapi Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'osmAPI exposes 4 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: osmAPI
provider_slug: osmapi
slug: osmapi-agentic-access
source_filename: osmapi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/osmapi-anthropic-messages-openapi.yml, openapi/osmapi-chat-completions-openapi.yml,\n  openapi/osmapi-health-openapi.yml, openapi/osmapi-models-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    acting: 2\n    connected: 2\n  by_consequence:\n    write: 2\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /messages\n  method: post\n  operationId: createMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /chat/completions\n  method: post\n  operationId: createChatCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /\n  method: get\n  operationId: healthCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /models\n  method: get\n  operationId: listModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/osmapi/refs/heads/main/agentic-access/osmapi-agentic-access.yml
summary_line: 4 operations · 2 acting
tags:
- AI
- Anthropic
- Gateway
- LLM
- OpenAI
- Routing
---
