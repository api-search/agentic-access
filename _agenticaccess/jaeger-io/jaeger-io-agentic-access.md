---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 7
api_specs:
- filename: jaeger-query-api-openapi.yml
  format: yaml
  label: Jaeger Query API
  slug: jaeger-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaeger-io/refs/heads/main/openapi/jaeger-query-api-openapi.yml
- filename: jaeger-collector-api-openapi.yml
  format: yaml
  label: Jaeger Collector API
  slug: jaeger-collector-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaeger-io/refs/heads/main/openapi/jaeger-collector-api-openapi.yml
- filename: jaeger-sampling-api-openapi.yml
  format: yaml
  label: Jaeger Sampling Manager API
  slug: jaeger-sampling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaeger-io/refs/heads/main/openapi/jaeger-sampling-api-openapi.yml
consequence_counts:
  read: 7
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Jaeger Io Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'Jaeger exposes 11 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Jaeger
provider_slug: jaeger-io
slug: jaeger-io-agentic-access
source_filename: jaeger-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/jaeger-collector-api-openapi.yml, openapi/jaeger-query-api-openapi.yml, openapi/jaeger-sampling-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    acting: 4\n    connected: 7\n  by_consequence:\n    write: 4\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v2/spans\n  method: post\n  operationId: postSpans\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v3/dependencies\n  method:\
  \ get\n  operationId: QueryService_GetDependencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/operations\n  method: get\n  operationId: QueryService_GetOperations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/services\n  method: get\n  operationId: QueryService_GetServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/trace-summaries\n  method: get\n  operationId: QueryService_FindTraceSummaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/trace-summaries\n  method: post\n  operationId: QueryService_FindTraceSummaries\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v3/traces\n  method: get\n  operationId: QueryService_FindTraces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/traces\n  method: post\n  operationId: QueryService_FindTracesPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v3/traces/{traceId}\n  method: get\n  operationId: QueryService_GetTrace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/samplingStrategy\n  method: post\n  operationId: getSamplingStrategy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sampling\n  method: get\n  operationId: getSamplingStrategyLegacy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jaeger-io/refs/heads/main/agentic-access/jaeger-io-agentic-access.yml
summary_line: 11 operations · 4 acting
tags:
- Observability
- Distributed Tracing
- APM
- OpenTelemetry
- CNCF
- Cloud Native
- Microservices
- Open Source
---
