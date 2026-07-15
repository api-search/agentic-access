---
acting_count: 4
action_class_counts:
  acting: 4
api_specs:
- filename: microsoft-azure-openai-openapi.yml
  format: yaml
  label: Azure OpenAI Service API
  slug: azure-openai-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-openai/refs/heads/main/openapi/microsoft-azure-openai-openapi.yml
consequence_counts:
  physical: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Microsoft Azure Openai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /openai/deployments/{deployment-id}/chat/completions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /openai/deployments/{deployment-id}/completions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /openai/deployments/{deployment-id}/embeddings
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /openai/deployments/{deployment-id}/images/generations
operation_count: 4
overview: 'Azure OpenAI Service exposes 4 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Azure OpenAI Service
provider_slug: microsoft-azure-openai
slug: microsoft-azure-openai-agentic-access
source_filename: microsoft-azure-openai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/microsoft-azure-openai-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    acting: 4\n  by_consequence:\n    physical: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /openai/deployments/{deployment-id}/completions\n  method: post\n  operationId: createCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - user_impersonation\n- path: /openai/deployments/{deployment-id}/chat/completions\n\
  \  method: post\n  operationId: createChatCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - user_impersonation\n- path: /openai/deployments/{deployment-id}/embeddings\n  method: post\n  operationId: createEmbedding\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - user_impersonation\n- path: /openai/deployments/{deployment-id}/images/generations\n  method: post\n  operationId: createImage\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - user_impersonation\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-openai/refs/heads/main/agentic-access/microsoft-azure-openai-agentic-access.yml
summary_line: 4 operations · 4 acting
tags:
- AI
- Embeddings
- GPT
- Generative AI
- Large Language Models
- OpenAI
---
