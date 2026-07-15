---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 6
api_specs:
- filename: agenta-openapi.yml
  format: yaml
  label: Agenta Apps and Variants API
  slug: agenta-apps-variants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agenta/refs/heads/main/openapi/agenta-openapi.yml
- filename: agenta-openapi.yml
  format: yaml
  label: Agenta Configs and Prompts API
  slug: agenta-configs-prompts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agenta/refs/heads/main/openapi/agenta-openapi.yml
- filename: agenta-openapi.yml
  format: yaml
  label: Agenta Evaluations and Evaluators API
  slug: agenta-evaluations-evaluators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agenta/refs/heads/main/openapi/agenta-openapi.yml
- filename: agenta-openapi.yml
  format: yaml
  label: Agenta Testsets API
  slug: agenta-testsets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agenta/refs/heads/main/openapi/agenta-openapi.yml
- filename: agenta-openapi.yml
  format: yaml
  label: Agenta Observability and Traces API
  slug: agenta-observability-traces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agenta/refs/heads/main/openapi/agenta-openapi.yml
consequence_counts:
  physical: 1
  read: 6
  write: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Agenta Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /applications/revisions/deploy
operation_count: 25
overview: 'Agenta exposes 25 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 18 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Agenta
provider_slug: agenta
slug: agenta-agentic-access
source_filename: agenta-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/agenta-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    acting: 19\n    connected: 6\n  by_consequence:\n    write: 18\n    read: 6\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /simple/applications/\n  method: post\n  operationId: createSimpleApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /simple/applications/query\n  method: post\n  operationId: querySimpleApplications\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /simple/applications/{application_id}\n  method: get\n  operationId: fetchSimpleApplication\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /simple/applications/{application_id}\n  method: put\n  operationId: editSimpleApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/variants/query\n  method: post\n  operationId: queryApplicationVariants\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/variants/{application_variant_id}\n  method: get\n  operationId: fetchApplicationVariant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/revisions/commit\n  method: post\n  operationId: commitApplicationRevision\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/revisions/deploy\n  method: post\n  operationId: deployApplicationRevision\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /variants/configs/fetch\n  method: post\n  operationId: fetchConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /testsets/\n  method: post\n  operationId: createTestset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /testsets/query\n  method: post\n  operationId: queryTestsets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /testsets/{testset_id}\n  method: get\n  operationId: fetchTestset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /simple/testsets/upload\n  method: post\n  operationId: createTestsetFromFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /evaluators/query\n  method: post\n  operationId: queryEvaluators\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /evaluators/\n  method: post\n  operationId: createEvaluator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /evaluators/catalog/templates/\n  method: get\n  operationId: listEvaluatorCatalogTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /evaluations/runs/query\n  method: post\n  operationId: queryEvaluationRuns\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /evaluations/runs/\n  method: post\n  operationId: createEvaluationRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /evaluations/results/query\n  method: post\n  operationId: queryEvaluationResults\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /evaluations/metrics/query\n  method:\
  \ post\n  operationId: queryEvaluationMetrics\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /traces/\n  method: get\n  operationId: fetchTraces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spans/query\n  method: post\n  operationId: querySpans\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spans/analytics/query\n  method: post\n  operationId: querySpanAnalytics\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /otlp/v1/traces\n  method: post\n  operationId: ingestOtlpTraces\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /otlp/v1/traces\n  method: get\n  operationId: otlpStatusCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agenta/refs/heads/main/agentic-access/agenta-agentic-access.yml
summary_line: 25 operations · 19 acting
tags:
- AI
- LLMOps
- Prompt Management
- LLM Evaluation
- Observability
---
