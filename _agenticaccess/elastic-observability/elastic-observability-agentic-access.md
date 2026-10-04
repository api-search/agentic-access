---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 5
api_specs:
- filename: elastic-observability-server-info-api-openapi.yml
  format: yaml
  label: Elastic Observability Server Info API
  slug: elastic-observability-server-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic-observability/refs/heads/main/openapi/elastic-observability-server-info-api-openapi.yml
- filename: elastic-observability-agent-config-api-openapi.yml
  format: yaml
  label: Elastic Observability agent config API
  slug: elastic-observability-agent-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic-observability/refs/heads/main/openapi/elastic-observability-agent-config-api-openapi.yml
- filename: elastic-observability-event-intake-api-openapi.yml
  format: yaml
  label: Elastic Observability event intake API
  slug: elastic-observability-event-intake-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic-observability/refs/heads/main/openapi/elastic-observability-event-intake-api-openapi.yml
- filename: elastic-observability-opentelemetry-intake-api-openapi.yml
  format: yaml
  label: Elastic Observability opentelemetry intake API
  slug: elastic-observability-opentelemetry-intake-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic-observability/refs/heads/main/openapi/elastic-observability-opentelemetry-intake-api-openapi.yml
consequence_counts:
  physical: 9
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Elastic Observability Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /intake/v2/events
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /intake/v2/rum/events
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /intake/v3/rum/events
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /opentelemetry.proto.collector.logs.v1.LogsService/Export
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /opentelemetry.proto.collector.metrics.v1.MetricsService/Export
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /opentelemetry.proto.collector.trace.v1.TraceService/Export
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/logs
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/metrics
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/traces
operation_count: 14
overview: 'Elastic Observability exposes 14 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 9 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Elastic Observability
provider_slug: elastic-observability
slug: elastic-observability-agentic-access
source_filename: elastic-observability-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/elastic-observability-agent-config-api-openapi.yml, openapi/elastic-observability-event-intake-api-openapi.yml,\n  openapi/elastic-observability-opentelemetry-intake-api-openapi.yml, openapi/elastic-observability-server-info-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 5\n    acting: 9\n  by_consequence:\n    read: 5\n    physical: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /config/v1/agents\n  method: get\n  operationId: getAgentConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /config/v1/agents\n  method:\
  \ post\n  operationId: postAgentConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /config/v1/rum/agents\n  method: get\n  operationId: getRumAgentConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /intake/v2/events\n  method: post\n  operationId: postEventIntake\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /intake/v2/rum/events\n  method: post\n  operationId: postRumEventIntakeV2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /intake/v3/rum/events\n  method: post\n  operationId: postRumEventIntakeV3\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /opentelemetry.proto.collector.metrics.v1.MetricsService/Export\n  method: post\n  operationId: postOtlpGrpcMetrics\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n    \
  \  human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /opentelemetry.proto.collector.trace.v1.TraceService/Export\n  method: post\n  operationId: postOtlpGrpcTraces\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /opentelemetry.proto.collector.logs.v1.LogsService/Export\n  method: post\n  operationId: postOtlpGrpcLogs\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v1/metrics\n  method: post\n  operationId: postOtlpHttpMetrics\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/traces\n  method: post\n  operationId: postOtlpHttpTraces\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/logs\n  method: post\n  operationId: postOtlpHttpLogs\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /\n  method: get\n  operationId: getServerHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: post\n  operationId: postServerHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elastic-observability/refs/heads/main/agentic-access/elastic-observability-agentic-access.yml
summary_line: 14 operations · 9 acting
tags:
- AIOps
- Observability
- APM
- Logging
- Metrics
- Tracing
- OpenTelemetry
- Monitoring
- Telemetry
---
