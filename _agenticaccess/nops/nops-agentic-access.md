---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 8
api_specs:
- filename: nops-nops-openapi.yml
  format: yaml
  label: nOps
  slug: nops
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nops/refs/heads/main/openapi/nops-nops-openapi.yml
consequence_counts:
  read: 8
  safety-critical: 1
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Nops Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /svc/notifications/scheduler/{id}/disable
operation_count: 12
overview: 'nOps exposes 12 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 3 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: nOps
provider_slug: nops
slug: nops-agentic-access
source_filename: nops-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/nops-nops-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 8\n    acting: 4\n  by_consequence:\n    read: 8\n    write: 3\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /c/v3/map-migration/\n  method: get\n  operationId: listMapMigrationProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /c/v3/map-migration/{id}/\n  method: get\n  operationId: getMapMigrationProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /c/v3/map-migration/{id}/products/\n  method: get\n  operationId: listMapMigrationProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /c/v3/map-migration/{id}/resources/\n  method: get\n  operationId: listMapMigrationResources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /svc/k8s_cost/recommendations/essentials/scheduler/workload/\n  method: get\n  operationId: getSchedulerWorkloadRecommendations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /svc/k8s_cost/recommendations/essentials/scheduler/workload/summary/\n  method: get\n  operationId: getSchedulerWorkloadSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /svc/k8s_cost/recommendations/essentials/scheduler/utilization/\n  method: get\n  operationId: getSchedulerUtilizationRecommendations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /svc/k8s_cost/recommendations/essentials/scheduler/utilization/summary/\n  method: get\n  operationId: getSchedulerUtilizationSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /svc/notifications/scheduler/nops_scheduler\n  method: post\n  operationId: createScheduler\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /svc/notifications/scheduler/{id}/trigger\n  method: post\n  operationId: triggerScheduler\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /svc/notifications/scheduler/{id}/enable\n  method: post\n  operationId: enableScheduler\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /svc/notifications/scheduler/{id}/disable\n  method: post\n  operationId: disableScheduler\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nops/refs/heads/main/agentic-access/nops-agentic-access.yml
summary_line: 12 operations · 4 acting · 1 human-in-the-loop
tags:
- Costs
- FinOps
---
