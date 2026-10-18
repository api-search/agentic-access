---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 5
api_specs:
- filename: azure-ai-foundry-chat-completions-api-openapi.yml
  format: yaml
  label: Microsoft Azure AI Foundry Chat Completions API
  slug: azure-ai-foundry-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ai-foundry/refs/heads/main/openapi/azure-ai-foundry-chat-completions-api-openapi.yml
- filename: azure-ai-foundry-completions-api-openapi.yml
  format: yaml
  label: Microsoft Azure AI Foundry Completions API
  slug: azure-ai-foundry-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ai-foundry/refs/heads/main/openapi/azure-ai-foundry-completions-api-openapi.yml
- filename: azure-ai-foundry-embeddings-api-openapi.yml
  format: yaml
  label: Microsoft Azure AI Foundry Embeddings API
  slug: azure-ai-foundry-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ai-foundry/refs/heads/main/openapi/azure-ai-foundry-embeddings-api-openapi.yml
- filename: azure-ai-foundry-images-api-openapi.yml
  format: yaml
  label: Microsoft Azure AI Foundry Images API
  slug: azure-ai-foundry-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ai-foundry/refs/heads/main/openapi/azure-ai-foundry-images-api-openapi.yml
- filename: azure-ai-foundry-models-api-openapi.yml
  format: yaml
  label: Microsoft Azure AI Foundry Models API
  slug: azure-ai-foundry-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ai-foundry/refs/heads/main/openapi/azure-ai-foundry-models-api-openapi.yml
- filename: azure-ai-foundry-operations-api-openapi.yml
  format: yaml
  label: Microsoft Azure AI Foundry Operations API
  slug: microsoft-azure-ai-foundry-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ai-foundry/refs/heads/main/openapi/azure-ai-foundry-operations-api-openapi.yml
- filename: azure-ai-foundry-workspaces-api-openapi.yml
  format: yaml
  label: Microsoft Azure AI Foundry Workspaces API
  slug: microsoft-azure-ai-foundry-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ai-foundry/refs/heads/main/openapi/azure-ai-foundry-workspaces-api-openapi.yml
- filename: azure-ai-foundry-decisions-api-openapi.yml
  format: yaml
  label: Microsoft Azure AI Foundry Decisions API
  slug: azure-ai-foundry-decisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ai-foundry/refs/heads/main/openapi/azure-ai-foundry-decisions-api-openapi.yml
consequence_counts:
  physical: 4
  read: 5
  write: 6
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
operation_count: 15
overview: 'Microsoft Azure AI Foundry exposes 15 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read, 6 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Microsoft Azure AI Foundry
provider_slug: azure-ai-foundry
slug: azure-ai-foundry-agentic-access
source_filename: azure-ai-foundry-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-17'\nmethod: generated\nsource: openapi/azure-ai-foundry-chat-completions-api-openapi.yml, openapi/azure-ai-foundry-completions-api-openapi.yml,\n  openapi/azure-ai-foundry-decisions-api-openapi.yml, openapi/azure-ai-foundry-embeddings-api-openapi.yml,\n  openapi/azure-ai-foundry-images-api-openapi.yml, openapi/azure-ai-foundry-models-api-openapi.yml,\n  openapi/azure-ai-foundry-operations-api-openapi.yml, openapi/azure-ai-foundry-workspaces-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    acting: 10\n    connected: 5\n  by_consequence:\n    physical: 4\n    write: 6\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /deployments/{deployment-id}/chat/completions\n\
  \  method: post\n  operationId: createChatCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chat/completions\n  method: post\n  operationId: createChatCompletionV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deployments/{deployment-id}/completions\n  method: post\n  operationId: createCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n   \
  \   exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /providers/microsoft/v1/systemone\n  method: post\n  operationId: createDecision\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deployments/{deployment-id}/embeddings\n  method: post\n  operationId: createEmbeddings\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/embeddings\n\
  \  method: post\n  operationId: createEmbeddingsV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deployments/{deployment-id}/images/generations\n  method: post\n  operationId: generateImages\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /models\n  method: get\n  operationId: listModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /providers/Microsoft.MachineLearningServices/operations\n\
  \  method: get\n  operationId: listOperations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/providers/Microsoft.MachineLearningServices/workspaces\n  method: get\n  operationId: listWorkspacesBySubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MachineLearningServices/workspaces\n  method: get\n  operationId: listWorkspacesByResourceGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MachineLearningServices/workspaces/{name}\n\
  \  method: get\n  operationId: getWorkspaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MachineLearningServices/workspaces/{name}\n  method: put\n  operationId: createOrUpdateWorkspaces\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MachineLearningServices/workspaces/{name}\n  method: patch\n  operationId: updateWorkspaces\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n \
  \   subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MachineLearningServices/workspaces/{name}\n  method: delete\n  operationId: deleteWorkspaces\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - user_impersonation\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-ai-foundry/refs/heads/main/agentic-access/azure-ai-foundry-agentic-access.yml
summary_line: 15 operations · 10 acting
tags:
- Artificial Intelligence
- Generative AI
- AI Agents
- Foundation Models
- Machine Learning
- Cloud
- Microsoft Azure
- A2A
---
