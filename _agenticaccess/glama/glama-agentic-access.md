---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 3
api_specs:
- filename: glama-auth-api-openapi.yml
  format: yaml
  label: Glama AI Auth API
  slug: glama-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glama/refs/heads/main/openapi/glama-auth-api-openapi.yml
- filename: glama-chat-completions-api-openapi.yml
  format: yaml
  label: Glama AI Chat Completions API
  slug: glama-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glama/refs/heads/main/openapi/glama-chat-completions-api-openapi.yml
- filename: glama-models-api-openapi.yml
  format: yaml
  label: Glama AI Models API
  slug: glama-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glama/refs/heads/main/openapi/glama-models-api-openapi.yml
- filename: glama-observability-api-openapi.yml
  format: yaml
  label: Glama AI Observability API
  slug: glama-observability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glama/refs/heads/main/openapi/glama-observability-api-openapi.yml
- filename: glama-responses-api-openapi.yml
  format: yaml
  label: Glama AI Responses API
  slug: glama-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glama/refs/heads/main/openapi/glama-responses-api-openapi.yml
consequence_counts:
  read: 3
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Glama Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Glama AI exposes 6 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Glama AI
provider_slug: glama
slug: glama-agentic-access
source_filename: glama-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/glama-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    acting: 3\n    connected: 3\n  by_consequence:\n    write: 3\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /openai/v1/chat/completions\n  method: post\n  operationId: createChatCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openai/v1/responses\n  method: post\n  operationId: createResponse\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openai/v1/models\n  method: get\n  operationId: listModelsOpenAi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/models\n  method: get\n  operationId: listModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/auth/exchange-code\n  method: post\n  operationId: exchangeAuthCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/completion-requests/{id}\n  method: get\n  operationId: getCompletionRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glama/refs/heads/main/agentic-access/glama-agentic-access.yml
summary_line: 6 operations · 3 acting
tags:
- MCP
- MCP Marketplace
- MCP Gateway
- MCP Hosting
- MCP Inspector
- AI Gateway
- LLM Gateway
- Connectors
- Authentication
- Observability
- Multi-Provider
---
