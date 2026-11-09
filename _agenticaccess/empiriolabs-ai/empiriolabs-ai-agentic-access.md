---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 2
api_specs:
- filename: empiriolabs-ai-chatcompletions-api-openapi.yml
  format: yaml
  label: EmpirioLabs AI Chat Completions API
  slug: empiriolabs-ai-chatcompletions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/empiriolabs-ai/openapi/empiriolabs-ai-chatcompletions-api-openapi.yml
- filename: empiriolabs-ai-completions-api-openapi.yml
  format: yaml
  label: EmpirioLabs AI Completions API
  slug: empiriolabs-ai-completions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/empiriolabs-ai/openapi/empiriolabs-ai-completions-api-openapi.yml
- filename: empiriolabs-ai-gemini-api-openapi.yml
  format: yaml
  label: EmpirioLabs AI Gemini API
  slug: empiriolabs-ai-gemini-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/empiriolabs-ai/openapi/empiriolabs-ai-gemini-api-openapi.yml
- filename: empiriolabs-ai-messages-api-openapi.yml
  format: yaml
  label: EmpirioLabs AI Messages API
  slug: empiriolabs-ai-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/empiriolabs-ai/openapi/empiriolabs-ai-messages-api-openapi.yml
- filename: empiriolabs-ai-models-api-openapi.yml
  format: yaml
  label: EmpirioLabs AI Models API
  slug: empiriolabs-ai-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/empiriolabs-ai/openapi/empiriolabs-ai-models-api-openapi.yml
- filename: empiriolabs-ai-responses-api-openapi.yml
  format: yaml
  label: EmpirioLabs AI Responses API
  slug: empiriolabs-ai-responses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/empiriolabs-ai/openapi/empiriolabs-ai-responses-api-openapi.yml
consequence_counts:
  read: 2
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Empiriolabs Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'EmpirioLabs AI exposes 7 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: EmpirioLabs AI
provider_slug: empiriolabs-ai
slug: empiriolabs-ai-agentic-access
source_filename: empiriolabs-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: generated\nsource: openapi/empiriolabs-ai-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 2\n    acting: 5\n  by_consequence:\n    read: 2\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/models\n  method: get\n  operationId: models_listModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/models/{model_id}\n  method: get\n  operationId: models_retrieveModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chat/completions\n\
  \  method: post\n  operationId: chatCompletions_createChatCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/completions\n  method: post\n  operationId: completions_createCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/responses\n  method: post\n  operationId: responses_createResponse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/messages\n  method: post\n  operationId: messages_createMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1beta/models/{model}:generateContent\n  method: post\n  operationId: gemini_generateContent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/empiriolabs-ai/agentic-access/empiriolabs-ai-agentic-access.yml
summary_line: 7 operations · 5 acting
tags:
- Company
- Artificial Intelligence
- Inference
- Cloud
- Platform
---
