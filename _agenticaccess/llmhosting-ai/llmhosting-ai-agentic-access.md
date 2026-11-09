---
acting_count: 0
action_class_counts:
  connected: 4
api_specs:
- filename: llmhosting-ai-gpu-history-csv-api-openapi.yml
  format: yaml
  label: llmhosting-ai Gpu History.csv API
  slug: llmhosting-ai-gpu-history-csv-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/llmhosting-ai/openapi/llmhosting-ai-gpu-history-csv-api-openapi.yml
- filename: llmhosting-ai-gpu-history-json-api-openapi.yml
  format: yaml
  label: llmhosting-ai Gpu History.json API
  slug: llmhosting-ai-gpu-history-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/llmhosting-ai/openapi/llmhosting-ai-gpu-history-json-api-openapi.yml
- filename: llmhosting-ai-gpu-prices-json-api-openapi.yml
  format: yaml
  label: llmhosting-ai Gpu Prices.json API
  slug: llmhosting-ai-gpu-prices-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/llmhosting-ai/openapi/llmhosting-ai-gpu-prices-json-api-openapi.yml
- filename: llmhosting-ai-prices-json-api-openapi.yml
  format: yaml
  label: llmhosting-ai Prices.json API
  slug: llmhosting-ai-prices-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/llmhosting-ai/openapi/llmhosting-ai-prices-json-api-openapi.yml
consequence_counts:
  read: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Llmhosting Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'llmhosting-ai exposes 4 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: llmhosting-ai
provider_slug: llmhosting-ai
slug: llmhosting-ai-agentic-access
source_filename: llmhosting-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/llmhosting-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    connected: 4\n  by_consequence:\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /api/prices.json\n  method: get\n  operationId: getLlmPrices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpu-prices.json\n  method: get\n  operationId: getGpuPrices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpu-history.json\n  method: get\n  operationId:\
  \ getGpuHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/gpu-history.csv\n  method: get\n  operationId: getGpuHistoryCsv\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/llmhosting-ai/agentic-access/llmhosting-ai-agentic-access.yml
summary_line: 4 operations
tags:
- Company
- LLM
- Pricing
- GPU
- Comparison
---
