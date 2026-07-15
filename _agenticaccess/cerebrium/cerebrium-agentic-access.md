---
acting_count: 3
action_class_counts:
  acting: 3
api_specs:
- filename: cerebrium-openapi.yml
  format: yaml
  label: Cerebrium Inference / Run Endpoints API
  slug: cerebrium-inference-run-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cerebrium/refs/heads/main/openapi/cerebrium-openapi.yml
- filename: cerebrium-openapi.yml
  format: yaml
  label: Cerebrium Streaming Endpoints API
  slug: cerebrium-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cerebrium/refs/heads/main/openapi/cerebrium-openapi.yml
- filename: cerebrium-openapi.yml
  format: yaml
  label: Cerebrium Async Requests API
  slug: cerebrium-async-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cerebrium/refs/heads/main/openapi/cerebrium-openapi.yml
- filename: cerebrium-openapi.yml
  format: yaml
  label: Cerebrium App Deployment / Management API
  slug: cerebrium-app-deployment-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cerebrium/refs/heads/main/openapi/cerebrium-openapi.yml
consequence_counts:
  physical: 1
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cerebrium Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v4/{projectId}/{appName}/{functionName}
operation_count: 3
overview: 'Cerebrium exposes 3 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 write and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cerebrium
provider_slug: cerebrium
slug: cerebrium-agentic-access
source_filename: cerebrium-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/cerebrium-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 3\n  by_action_class:\n    acting: 3\n  by_consequence:\n    physical: 1\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /v4/{projectId}/{appName}/{functionName}\n  method: post\n  operationId: runFunction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/{projectId}/{appName}/{functionName}/chat/completions\n\
  \  method: post\n  operationId: openaiChatCompletions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/{projectId}/{appName}/{functionName}/embedding\n  method: post\n  operationId: openaiEmbedding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cerebrium/refs/heads/main/agentic-access/cerebrium-agentic-access.yml
summary_line: 3 operations · 3 acting
tags:
- AI
- GPU
- Serverless
- Inference
- ML Infrastructure
---
