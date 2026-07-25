---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 3
api_specs:
- filename: perplexity-asyncapi.yml
  format: yaml
  label: Perplexity Async Chat Completions API
  slug: async-chat-completions-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/perplexity/refs/heads/main/asyncapi/perplexity-asyncapi.yml
- filename: perplexity-asyncapi.yml
  format: yaml
  label: Perplexity Responses API
  slug: responses-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/perplexity/refs/heads/main/asyncapi/perplexity-asyncapi.yml
- filename: perplexity-agent-api-openapi.yml
  format: yaml
  label: Perplexity Agent API
  slug: perplexity-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perplexity/refs/heads/main/openapi/perplexity-agent-api-openapi.yml
- filename: perplexity-async-api-openapi.yml
  format: yaml
  label: Perplexity Async API
  slug: perplexity-async-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perplexity/refs/heads/main/openapi/perplexity-async-api-openapi.yml
- filename: perplexity-contextualizedembeddings-api-openapi.yml
  format: yaml
  label: Perplexity Contextualizedembeddings API
  slug: perplexity-contextualizedembeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perplexity/refs/heads/main/openapi/perplexity-contextualizedembeddings-api-openapi.yml
- filename: perplexity-embeddings-api-openapi.yml
  format: yaml
  label: Perplexity Embeddings API
  slug: perplexity-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perplexity/refs/heads/main/openapi/perplexity-embeddings-api-openapi.yml
- filename: perplexity-models-api-openapi.yml
  format: yaml
  label: Perplexity Models API
  slug: perplexity-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perplexity/refs/heads/main/openapi/perplexity-models-api-openapi.yml
- filename: perplexity-search-api-openapi.yml
  format: yaml
  label: Perplexity Search API
  slug: perplexity-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perplexity/refs/heads/main/openapi/perplexity-search-api-openapi.yml
- filename: perplexity-sonar-api-openapi.yml
  format: yaml
  label: Perplexity Sonar API
  slug: perplexity-sonar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perplexity/refs/heads/main/openapi/perplexity-sonar-api-openapi.yml
consequence_counts:
  read: 3
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Perplexity Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Perplexity exposes 9 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Perplexity
provider_slug: perplexity
slug: perplexity-agentic-access
source_filename: perplexity-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/perplexity-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    acting: 6\n    connected: 3\n  by_consequence:\n    write: 6\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/sonar\n  method: post\n  operationId: chat_completions_chat_completions_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /search\n  method: post\n  operationId: search_search_post\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/embeddings\n  method: post\n  operationId: embeddings_v1_embeddings_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/contextualizedembeddings\n  method: post\n  operationId: contextualized_embeddings_v1_contextualizedembeddings_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/async/sonar/{api_request}\n  method: get\n  operationId: get_async_chat_completion_response_async_chat_completions__api_request__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/async/sonar\n  method: get\n  operationId: list_async_chat_completions_async_chat_completions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/async/sonar\n  method: post\n  operationId: create_async_chat_completions_async_chat_completions_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent\n  method: post\n  operationId: createAgent\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/models\n  method: get\n  operationId: listModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/perplexity/refs/heads/main/agentic-access/perplexity-agentic-access.yml
summary_line: 9 operations · 6 acting
tags: []
---
