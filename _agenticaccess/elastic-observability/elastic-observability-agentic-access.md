---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 3
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
  read: 3
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Elastic Observability Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'Elastic Observability exposes 14 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 11 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Elastic Observability
provider_slug: elastic-observability
slug: elastic-observability-agentic-access
source_filename: elastic-observability-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: generated\nsource: openapi/elastic-observability-agent-config-api-openapi.yml, openapi/elastic-observability-event-intake-api-openapi.yml,\n  openapi/elastic-observability-opentelemetry-intake-api-openapi.yml, openapi/elastic-observability-server-info-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI.\n  A governance starting point for exposing this API to AI agents — review and bind audience per deployment.\n  See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 3\n    acting: 11\n  by_consequence:\n    read: 3\n    write: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /config/v1/agents\n  method: get\n  operationId: getAgentConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /config/v1/agents\n  method:\
  \ post\n  operationId: postAgentConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /config/v1/rum/agents\n  method: get\n  operationId: getRumAgentConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /intake/v2/events\n  method: post\n  operationId: postEventIntake\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    x-corrected: consequence lowered from physical to write — see corrections\n\
  - path: /intake/v2/rum/events\n  method: post\n  operationId: postRumEventIntakeV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    x-corrected: consequence lowered from physical to write — see corrections\n- path: /intake/v3/rum/events\n  method: post\n  operationId: postRumEventIntakeV3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    x-corrected: consequence lowered from physical to write — see corrections\n- path: /opentelemetry.proto.collector.metrics.v1.MetricsService/Export\n\
  \  method: post\n  operationId: postOtlpGrpcMetrics\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    x-corrected: consequence lowered from physical to write — see corrections\n- path: /opentelemetry.proto.collector.trace.v1.TraceService/Export\n  method: post\n  operationId: postOtlpGrpcTraces\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    x-corrected: consequence lowered from physical to write — see corrections\n- path: /opentelemetry.proto.collector.logs.v1.LogsService/Export\n\
  \  method: post\n  operationId: postOtlpGrpcLogs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    x-corrected: consequence lowered from physical to write — see corrections\n- path: /v1/metrics\n  method: post\n  operationId: postOtlpHttpMetrics\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    x-corrected: consequence lowered from physical to write — see corrections\n- path: /v1/traces\n  method: post\n  operationId: postOtlpHttpTraces\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    x-corrected: consequence lowered from physical to write — see corrections\n- path: /v1/logs\n  method: post\n  operationId: postOtlpHttpLogs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    x-corrected: consequence lowered from physical to write — see corrections\n- path: /\n  method: get\n  operationId: getServerHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /\n  method: post\n  operationId: postServerHealth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\ncorrections:\n- date: '2026-08-29'\n  applied_to:\n  - postEventIntake\n  - postRumEventIntakeV2\n  - postRumEventIntakeV3\n  - postOtlpGrpcMetrics\n  - postOtlpGrpcTraces\n  - postOtlpGrpcLogs\n  - postOtlpHttpMetrics\n  - postOtlpHttpTraces\n  - postOtlpHttpLogs\n  from: physical\n  to: write\n  reason: The derive heuristic raises consequence to `physical` on payment/order/transfer style keywords,\n    and it fired on the telemetry intake and OTLP *Export* operation names. Writing a span, a metric\n    sample or a log line into an observability store moves no money and touches no physical system —\n    it is an ordinary append. Left uncorrected\
  \ this file would tell an agent it needs token exchange\n    and a stated purpose to emit a log, which is both wrong and the kind of false ceiling that gets\n    governance guidance ignored wholesale.\n  residual_risk: 'These operations remain `acting`/`write` with audit: required, which is correct: the\n    writes are irreversible and un-deduplicated. See conventions/elastic-observability-conventions.yml\n    reversibility.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elastic-observability/refs/heads/main/agentic-access/elastic-observability-agentic-access.yml
summary_line: 14 operations · 11 acting
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
