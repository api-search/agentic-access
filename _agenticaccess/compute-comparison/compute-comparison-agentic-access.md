---
acting_count: 0
action_class_counts:
  connected: 6
api_specs:
- filename: compute-comparison-prices-api-openapi.yml
  format: yaml
  label: Compute Comparison Prices API
  slug: compute-comparison-prices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compute-comparison/openapi/compute-comparison-prices-api-openapi.yml
- filename: compute-comparison-status-api-openapi.yml
  format: yaml
  label: Compute Comparison Status API
  slug: compute-comparison-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compute-comparison/openapi/compute-comparison-status-api-openapi.yml
consequence_counts:
  read: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Compute Comparison Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Compute Comparison exposes 6 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Compute Comparison
provider_slug: compute-comparison
slug: compute-comparison-agentic-access
source_filename: compute-comparison-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/compute-comparison-openapi-gpu.yml, openapi/compute-comparison-openapi-llm.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 6\n  by_consequence:\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /prices\n  method: get\n  operationId: listGpuPrices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /prices/gpus\n  method: get\n  operationId: listGpuModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /prices/providers\n\
  \  method: get\n  operationId: listGpuProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /prices/history\n  method: get\n  operationId: getGpuPriceHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status\n  method: get\n  operationId: getApiStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llm/history\n  method: get\n  operationId: getLlmPriceHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/compute-comparison/agentic-access/compute-comparison-agentic-access.yml
summary_line: 6 operations
tags:
- Company
- GPU
- LLM
- Cloud
- Pricing
- Comparison
---
