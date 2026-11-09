---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 5
api_specs:
- filename: llmintel-ai-compare-api-openapi.yml
  format: yaml
  label: llmintel-ai Compare API
  slug: llmintel-ai-compare-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/llmintel-ai/openapi/llmintel-ai-compare-api-openapi.yml
- filename: llmintel-ai-events-api-openapi.yml
  format: yaml
  label: llmintel-ai Events API
  slug: llmintel-ai-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/llmintel-ai/openapi/llmintel-ai-events-api-openapi.yml
- filename: llmintel-ai-models-api-openapi.yml
  format: yaml
  label: llmintel-ai Models API
  slug: llmintel-ai-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/llmintel-ai/openapi/llmintel-ai-models-api-openapi.yml
- filename: llmintel-ai-status-api-openapi.yml
  format: yaml
  label: llmintel-ai Status API
  slug: llmintel-ai-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/llmintel-ai/openapi/llmintel-ai-status-api-openapi.yml
- filename: llmintel-ai-telemetry-api-openapi.yml
  format: yaml
  label: llmintel-ai Telemetry API
  slug: llmintel-ai-telemetry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/llmintel-ai/openapi/llmintel-ai-telemetry-api-openapi.yml
consequence_counts:
  read: 5
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Llmintel Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'llmintel-ai exposes 6 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: llmintel-ai
provider_slug: llmintel-ai
slug: llmintel-ai-agentic-access
source_filename: llmintel-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/llmintel-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 5\n    acting: 1\n  by_consequence:\n    read: 5\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/models\n  method: get\n  operationId: listModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/models/{id}\n  method: get\n  operationId: getModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/events\n  method: get\n  operationId: listEvents\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/status\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/compare\n  method: get\n  operationId: compareModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/telemetry\n  method: post\n  operationId: ingestTelemetry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/llmintel-ai/agentic-access/llmintel-ai-agentic-access.yml
summary_line: 6 operations · 1 acting
tags:
- Artificial Intelligence
- Cost
- Observability
- Telemetry
- Generative AI
---
