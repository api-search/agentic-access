---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 5
api_specs:
- filename: keywordsai-openapi.yml
  format: yaml
  label: Keywords AI LLM Proxy (Chat Completions)
  slug: llm-proxy-chat-completions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keywordsai/refs/heads/main/openapi/keywordsai-openapi.yml
- filename: keywordsai-openapi.yml
  format: yaml
  label: Keywords AI Logging API
  slug: logging
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keywordsai/refs/heads/main/openapi/keywordsai-openapi.yml
- filename: keywordsai-openapi.yml
  format: yaml
  label: Keywords AI Prompts API
  slug: prompts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keywordsai/refs/heads/main/openapi/keywordsai-openapi.yml
- filename: keywordsai-openapi.yml
  format: yaml
  label: Keywords AI Threads API
  slug: threads
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keywordsai/refs/heads/main/openapi/keywordsai-openapi.yml
- filename: keywordsai-openapi.yml
  format: yaml
  label: Keywords AI Evaluations API
  slug: evaluations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keywordsai/refs/heads/main/openapi/keywordsai-openapi.yml
- filename: keywordsai-openapi.yml
  format: yaml
  label: Keywords AI Traces API
  slug: traces
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keywordsai/refs/heads/main/openapi/keywordsai-openapi.yml
consequence_counts:
  read: 5
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Keywordsai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 20
overview: 'Keywords AI exposes 20 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 15 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Keywords AI
provider_slug: keywordsai
slug: keywordsai-agentic-access
source_filename: keywordsai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/keywordsai-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    acting: 15\n    connected: 5\n  by_consequence:\n    write: 15\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /chat/completions\n  method: post\n  operationId: createChatCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /request-logs/\n  method: post\n  operationId: createRequestLog\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /prompts/\n  method: post\n  operationId: createPrompt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /prompts/\n  method: get\n  operationId: listPrompts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /prompts/{prompt_id}/\n  method: get\n  operationId: retrievePrompt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /prompts/{prompt_id}/\n  method: patch\n  operationId: updatePrompt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /prompts/{prompt_id}/\n  method: delete\n  operationId: deletePrompt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /prompts/{prompt_id}/versions/\n  method: post\n  operationId: createPromptVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /prompts/{prompt_id}/versions/\n  method: get\n  operationId: listPromptVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /log_threads/\n  method: post\n  operationId: listThreads\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /traces/list/\n  method: post\n  operationId: listTraces\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /traces/{trace_id}/\n  method: get\n  operationId: retrieveTrace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /traces/{trace_id}/\n  method: delete\n  operationId: deleteTrace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /evaluators/\n  method: post\n  operationId: createEvaluator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /evaluators/list/\n  method: post\n  operationId: listEvaluators\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /evaluators/{evaluator_id}/run/\n  method: post\n  operationId: runEvaluator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/list/\n  method: post\n  operationId: listUsers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets/\n  method: post\n  operationId:\
  \ createDataset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets/\n  method: get\n  operationId: listDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /experiments/\n  method: post\n  operationId: createExperiment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keywordsai/refs/heads/main/agentic-access/keywordsai-agentic-access.yml
summary_line: 20 operations · 15 acting
tags:
- AI
- LLM
- Observability
- Gateway
- Monitoring
---
