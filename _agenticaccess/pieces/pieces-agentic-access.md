---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 14
api_specs:
- filename: pieces-openapi.yml
  format: yaml
  label: Pieces Assets API
  slug: pieces-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pieces/refs/heads/main/openapi/pieces-openapi.yml
- filename: pieces-openapi.yml
  format: yaml
  label: Pieces Copilot (QGPT) API
  slug: pieces-copilot-qgpt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pieces/refs/heads/main/openapi/pieces-openapi.yml
- filename: pieces-openapi.yml
  format: yaml
  label: Pieces Conversations API
  slug: pieces-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pieces/refs/heads/main/openapi/pieces-openapi.yml
- filename: pieces-openapi.yml
  format: yaml
  label: Pieces Models API
  slug: pieces-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pieces/refs/heads/main/openapi/pieces-openapi.yml
- filename: pieces-openapi.yml
  format: yaml
  label: Pieces Formats API
  slug: pieces-formats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pieces/refs/heads/main/openapi/pieces-openapi.yml
- filename: pieces-openapi.yml
  format: yaml
  label: Pieces Applications & Workspace API
  slug: pieces-applications-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pieces/refs/heads/main/openapi/pieces-openapi.yml
consequence_counts:
  read: 14
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Pieces Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 28
overview: 'Pieces exposes 28 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read and 14 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Pieces
provider_slug: pieces
slug: pieces-agentic-access
source_filename: pieces-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/pieces-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 28\n  by_action_class:\n    connected: 14\n    acting: 14\n  by_consequence:\n    read: 14\n    write: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /.well-known/health\n  method: get\n  operationId: getWellKnownHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/version\n  method: get\n  operationId: getWellKnownVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets\n \
  \ method: get\n  operationId: getAssetsSnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/create\n  method: post\n  operationId: createAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/search\n  method: post\n  operationId: searchAssets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asset/{asset}\n  method: get\n  operationId: getAsset\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset/update\n  method: post\n  operationId: updateAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/{asset}/delete\n  method: post\n  operationId: deleteAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /formats\n  method: get\n  operationId: getFormatsSnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /format/{format}\n  method: get\n  operationId: getFormat\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /qgpt/question\n  method: post\n  operationId: qgptQuestion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /qgpt/relevance\n  method: post\n  operationId: qgptRelevance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /qgpt/reprompt\n  method: post\n  operationId: qgptReprompt\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /qgpt/stream\n  method: get\n  operationId: qgptStream\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversations\n  method: get\n  operationId: getConversationsSnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversations/create\n  method: post\n  operationId: createConversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /conversation/{conversation}\n  method: get\n  operationId: getConversation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversation/{conversation}/messages\n  method: get\n  operationId: getConversationMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /models\n  method: get\n  operationId: getModelsSnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /model/{model}\n  method: get\n  operationId: getModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /model/{model}/download\n  method: post\n\
  \  operationId: downloadModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /model/{model}/load\n  method: post\n  operationId: loadModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /model/{model}/unload\n  method: post\n  operationId: unloadModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /applications\n  method: get\n  operationId: getApplicationsSnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/register\n  method: post\n  operationId: registerApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/session/open\n  method: post\n  operationId: openApplicationSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/session/close\n  method:\
  \ post\n  operationId: closeApplicationSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pieces/refs/heads/main/agentic-access/pieces-agentic-access.yml
summary_line: 28 operations · 14 acting
tags:
- AI
- Developer Tools
- On-Device
- Local API
- Long-Term Memory
---
