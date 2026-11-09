---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 8
api_specs:
- filename: fluxaipro-art-agent-integration-api-openapi.yml
  format: yaml
  label: Flux AI Agent Integration API
  slug: fluxaipro-art-agent-integration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluxaipro-art/openapi/fluxaipro-art-agent-integration-api-openapi.yml
- filename: fluxaipro-art-ai-generations-api-openapi.yml
  format: yaml
  label: Flux AI AI Generations API
  slug: fluxaipro-art-ai-generations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluxaipro-art/openapi/fluxaipro-art-ai-generations-api-openapi.yml
- filename: fluxaipro-art-models-api-openapi.yml
  format: yaml
  label: Flux AI Models API
  slug: fluxaipro-art-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluxaipro-art/openapi/fluxaipro-art-models-api-openapi.yml
consequence_counts:
  read: 8
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Fluxaipro Art Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 18
overview: 'Flux AI exposes 18 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 10 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Flux AI
provider_slug: fluxaipro-art
slug: fluxaipro-art-agentic-access
source_filename: fluxaipro-art-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: generated\nsource: openapi/fluxaipro-art-openapi.json, openapi/fluxaipro-art-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    connected: 8\n    acting: 10\n  by_consequence:\n    read: 8\n    write: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/ai/models\n  method: get\n  operationId: listAiModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/ai/pricing/estimate\n  method: post\n  operationId: estimateCredits\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/ai/generations\n  method: post\n  operationId: createGenerationTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/ai/generations\n  method: get\n  operationId: listGenerationTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/ai/generations/{taskId}\n  method: get\n  operationId: getGenerationTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/ai/generations/{taskId}/events\n\
  \  method: get\n  operationId: getGenerationTaskEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/ai/generations/{taskId}/cancel\n  method: post\n  operationId: cancelGenerationTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/ai/generations/{taskId}/retry\n  method: post\n  operationId: retryGenerationTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp\n  method: post\n  operationId:\
  \ callMcpTool\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/ai/models\n  method: get\n  operationId: listAiModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/ai/pricing/estimate\n  method: post\n  operationId: estimateCredits\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/ai/generations\n  method: post\n  operationId: createGenerationTask\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/ai/generations\n  method: get\n  operationId: listGenerationTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/ai/generations/{taskId}\n  method: get\n  operationId: getGenerationTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/ai/generations/{taskId}/events\n  method: get\n  operationId: getGenerationTaskEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/ai/generations/{taskId}/cancel\n  method:\
  \ post\n  operationId: cancelGenerationTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/ai/generations/{taskId}/retry\n  method: post\n  operationId: retryGenerationTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp\n  method: post\n  operationId: callMcpTool\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n   \
  \   - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/fluxaipro-art/agentic-access/fluxaipro-art-agentic-access.yml
summary_line: 18 operations · 10 acting
tags:
- AI
- Image Generation
- Creative Tools
- Prompt Engineering
- Company
---
