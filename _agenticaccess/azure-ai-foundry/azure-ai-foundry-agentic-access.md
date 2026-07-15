---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 1
api_specs:
- filename: azure-ai-foundry-openapi.yml
  format: yaml
  label: Azure AI Foundry REST API
  slug: foundry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ai-foundry/refs/heads/main/openapi/azure-ai-foundry-openapi.yml
consequence_counts:
  physical: 4
  read: 1
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Azure Ai Foundry Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /deployments/{deployment-id}/chat/completions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /deployments/{deployment-id}/completions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /deployments/{deployment-id}/embeddings
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /deployments/{deployment-id}/images/generations
operation_count: 7
overview: 'Microsoft Azure AI Foundry exposes 7 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read, 2 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Microsoft Azure AI Foundry
provider_slug: azure-ai-foundry
slug: azure-ai-foundry-agentic-access
source_filename: azure-ai-foundry-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/azure-ai-foundry-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    acting: 6\n    connected: 1\n  by_consequence:\n    physical: 4\n    write: 2\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /deployments/{deployment-id}/chat/completions\n  method: post\n  operationId: createChatCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deployments/{deployment-id}/completions\n\
  \  method: post\n  operationId: createCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deployments/{deployment-id}/embeddings\n  method: post\n  operationId: createEmbeddings\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deployments/{deployment-id}/images/generations\n  method: post\n  operationId: generateImages\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chat/completions\n  method: post\n  operationId: createChatCompletionV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/embeddings\n  method: post\n  operationId: createEmbeddingsV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /models\n  method: get\n  operationId:\
  \ listModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-ai-foundry/refs/heads/main/agentic-access/azure-ai-foundry-agentic-access.yml
summary_line: 7 operations · 6 acting
tags:
- Artificial Intelligence
- Generative AI
- AI Agents
- Foundation Models
- Machine Learning
- Cloud
- Azure
---
