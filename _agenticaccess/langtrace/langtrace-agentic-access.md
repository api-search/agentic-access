---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 1
api_specs:
- filename: langtrace-openapi.yml
  format: yaml
  label: Langtrace Trace Ingestion (OTEL)
  slug: trace-ingestion-otel
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langtrace/refs/heads/main/openapi/langtrace-openapi.yml
- filename: langtrace-openapi.yml
  format: yaml
  label: Langtrace Projects and API Keys
  slug: projects-api-keys
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langtrace/refs/heads/main/openapi/langtrace-openapi.yml
- filename: langtrace-openapi.yml
  format: yaml
  label: Langtrace Prompt Registry
  slug: prompt-registry
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langtrace/refs/heads/main/openapi/langtrace-openapi.yml
- filename: langtrace-openapi.yml
  format: yaml
  label: Langtrace Trace Retrieval and Metrics
  slug: trace-retrieval
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langtrace/refs/heads/main/openapi/langtrace-openapi.yml
consequence_counts:
  physical: 1
  read: 1
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Langtrace Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /trace
operation_count: 5
overview: 'Langtrace AI exposes 5 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read, 3 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Langtrace AI
provider_slug: langtrace
slug: langtrace-agentic-access
source_filename: langtrace-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/langtrace-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    acting: 4\n    connected: 1\n  by_consequence:\n    physical: 1\n    write: 3\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /trace\n  method: post\n  operationId: sendTrace\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /project\n  method: post\n  operationId: createProject\n \
  \ x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api-key\n  method: post\n  operationId: createProjectApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /promptset\n  method: get\n  operationId: getPromptFromRegistry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /traces\n  method: post\n  operationId: downloadTraces\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/langtrace/refs/heads/main/agentic-access/langtrace-agentic-access.yml
summary_line: 5 operations · 4 acting
tags:
- AI
- LLM
- Observability
- OpenTelemetry
- Tracing
- Open Source
---
