---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 7
api_specs:
- filename: kimi-ai-batch-api-openapi.yml
  format: yaml
  label: Moonshot AI Batch API
  slug: kimi-ai-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kimi-ai/openapi/kimi-ai-batch-api-openapi.yml
- filename: kimi-ai-billing-api-openapi.yml
  format: yaml
  label: Moonshot AI Billing API
  slug: kimi-ai-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kimi-ai/openapi/kimi-ai-billing-api-openapi.yml
- filename: kimi-ai-files-api-openapi.yml
  format: yaml
  label: Moonshot AI Files API
  slug: kimi-ai-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kimi-ai/openapi/kimi-ai-files-api-openapi.yml
- filename: kimi-ai-models-api-openapi.yml
  format: yaml
  label: Moonshot AI Models API
  slug: kimi-ai-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kimi-ai/openapi/kimi-ai-models-api-openapi.yml
- filename: kimi-ai-utilities-api-openapi.yml
  format: yaml
  label: Moonshot AI Utilities API
  slug: kimi-ai-utilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kimi-ai/openapi/kimi-ai-utilities-api-openapi.yml
- filename: kimi-ai-responses-api-openapi.yml
  format: yaml
  label: Moonshot AI Responses API
  slug: kimi-ai-responses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kimi-ai/openapi/kimi-ai-responses-api-openapi.yml
- filename: kimi-ai-tools-api-openapi.yml
  format: yaml
  label: Moonshot AI Tools API
  slug: kimi-ai-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kimi-ai/openapi/kimi-ai-tools-api-openapi.yml
- filename: kimi-ai-messages-api-openapi.yml
  format: yaml
  label: Kimi (Moonshot AI) Messages API
  slug: kimi-ai-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kimi-ai/openapi/kimi-ai-messages-api-openapi.yml
- filename: kimi-ai-chat-completions-api-openapi.yml
  format: yaml
  label: Kimi (Moonshot AI) Chat Completions API
  slug: kimi-ai-chat-completions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kimi-ai/openapi/kimi-ai-chat-completions-api-openapi.yml
consequence_counts:
  read: 7
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Kimi Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'Kimi (Moonshot AI) exposes 13 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Kimi (Moonshot AI)
provider_slug: kimi-ai
slug: kimi-ai-agentic-access
source_filename: kimi-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/kimi-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 7\n    acting: 6\n  by_consequence:\n    read: 7\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/models\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/me/balance\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/files\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/files\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/files/{file_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/files/{file_id}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/files/{file_id}/content\n  method: get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chat/completions\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tokenizers/estimate-token-count\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/batches\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n   \
  \   triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/batches\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/batches/{batch_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/batches/{batch_id}/cancel\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/kimi-ai/agentic-access/kimi-ai-agentic-access.yml
summary_line: 13 operations · 6 acting
tags:
- Artificial Intelligence
- LLM
- Inference
- Long Context
- Kimi
- Foundation Models
---
