---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 3
api_specs:
- filename: octen-ai-answer-api-openapi.yml
  format: yaml
  label: Octen Answer API
  slug: octen-ai-answer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-answer-api-openapi.yml
- filename: octen-ai-broad-search-api-openapi.yml
  format: yaml
  label: Octen Broad Search API
  slug: octen-ai-broad-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-broad-search-api-openapi.yml
- filename: octen-ai-business-search-api-openapi.yml
  format: yaml
  label: Octen Business Search API
  slug: octen-ai-business-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-business-search-api-openapi.yml
- filename: octen-ai-embedding-api-openapi.yml
  format: yaml
  label: Octen Embedding API
  slug: octen-ai-embedding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-embedding-api-openapi.yml
- filename: octen-ai-extract-api-openapi.yml
  format: yaml
  label: Octen Extract API
  slug: octen-ai-extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-extract-api-openapi.yml
- filename: octen-ai-grounded-generation-api-openapi.yml
  format: yaml
  label: Octen Grounded Generation API
  slug: octen-ai-grounded-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-grounded-generation-api-openapi.yml
- filename: octen-ai-image-search-api-openapi.yml
  format: yaml
  label: Octen Image Search API
  slug: octen-ai-image-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-image-search-api-openapi.yml
- filename: octen-ai-images-api-openapi.yml
  format: yaml
  label: Octen Images API
  slug: octen-ai-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-images-api-openapi.yml
- filename: octen-ai-messages-api-openapi.yml
  format: yaml
  label: Octen Messages API
  slug: octen-ai-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-messages-api-openapi.yml
- filename: octen-ai-news-search-api-openapi.yml
  format: yaml
  label: Octen News Search API
  slug: octen-ai-news-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-news-search-api-openapi.yml
- filename: octen-ai-research-api-openapi.yml
  format: yaml
  label: Octen Research API
  slug: octen-ai-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-research-api-openapi.yml
- filename: octen-ai-search-api-openapi.yml
  format: yaml
  label: Octen Search API
  slug: octen-ai-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-search-api-openapi.yml
- filename: octen-ai-video-search-api-openapi.yml
  format: yaml
  label: Octen Video Search API
  slug: octen-ai-video-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-video-search-api-openapi.yml
- filename: octen-ai-videos-api-openapi.yml
  format: yaml
  label: Octen Videos API
  slug: octen-ai-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-videos-api-openapi.yml
- filename: octen-ai-vl-embedding-api-openapi.yml
  format: yaml
  label: Octen Vl Embedding API
  slug: octen-ai-vl-embedding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-vl-embedding-api-openapi.yml
- filename: octen-ai-chat-completions-api-openapi.yml
  format: yaml
  label: Octen Chat Completions API
  slug: octen-ai-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/openapi/octen-ai-chat-completions-api-openapi.yml
consequence_counts:
  read: 3
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Octen Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 18
overview: 'Octen exposes 18 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 15 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Octen
provider_slug: octen-ai
slug: octen-ai-agentic-access
source_filename: octen-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: generated\nsource: openapi/octen-ai-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    connected: 3\n    acting: 15\n  by_consequence:\n    read: 3\n    write: 15\n  human_in_the_loop_required: 0\noperations:\n- path: /search\n  method: post\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /news-search\n  method: post\n  operationId: news-search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n \
  \     triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /business-search\n  method: post\n  operationId: business-search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /image-search\n  method: post\n  operationId: image-search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /video-search\n  method: post\n  operationId: video-search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /extract\n  method: post\n  operationId: extract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /embedding\n  method: post\n  operationId: embedding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vl-embedding\n  method: post\n  operationId: vl-embedding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chat/completions\n  method: post\n  operationId: chat-completions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /answer\n  method: post\n  operationId: answer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /broad-search\n  method: post\n  operationId: broad-search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/research\n  method: post\n  operationId: deep-research\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/messages\n  method: post\n  operationId: messages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/images/generations\n  method: post\n  operationId: images-generations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos\n  method: post\n  operationId: post-video\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos/{id}\n  method: get\n  operationId: get-video\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/grounded-generation\n  method: post\n  operationId: post-grounded-generation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/grounded-generation/{generation_id}\n  method: get\n  operationId: get-grounded-generation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/octen-ai/refs/heads/main/agentic-access/octen-ai-agentic-access.yml
summary_line: 18 operations · 15 acting
tags:
- Search
- Web Search
- AI
- LLM
- Embeddings
- Content Extraction
- Model Gateway
- MCP
- Agents
- Deep Research
- Company
---
