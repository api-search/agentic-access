---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 6
api_specs:
- filename: swarmia-openapi.yml
  format: yaml
  label: Swarmia Metrics Export API
  slug: metrics-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swarmia/refs/heads/main/openapi/swarmia-openapi.yml
- filename: swarmia-openapi.yml
  format: yaml
  label: Swarmia Deployments & Events Ingestion API
  slug: deployments-events-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swarmia/refs/heads/main/openapi/swarmia-openapi.yml
- filename: swarmia-openapi.yml
  format: yaml
  label: Swarmia Investment Categories API
  slug: investment-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swarmia/refs/heads/main/openapi/swarmia-openapi.yml
- filename: swarmia-openapi.yml
  format: yaml
  label: Swarmia Webhooks & Notifications API
  slug: webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swarmia/refs/heads/main/openapi/swarmia-openapi.yml
consequence_counts:
  physical: 1
  read: 6
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Swarmia Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /deployments
operation_count: 12
overview: 'Swarmia exposes 12 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 5 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Swarmia
provider_slug: swarmia
slug: swarmia-agentic-access
source_filename: swarmia-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/swarmia-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 6\n    acting: 6\n  by_consequence:\n    read: 6\n    write: 5\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /reports/metrics/code\n  method: get\n  operationId: getReportsMetricsCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/metrics/dora\n  method: get\n  operationId: getReportsMetricsDora\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /reports/ai/adoption/users-and-licenses\n  method: get\n  operationId: getReportsAiAdoptionUsersAndLicenses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/custom/{id}\n  method: get\n  operationId: getReportsCustomById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ingest/ai-usage\n  method: post\n  operationId: postUsage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deployments\n  method: post\n  operationId: createDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /teams\n  method: get\n  operationId: listTeams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /teams\n  method: put\n  operationId: updateTeams\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /time-offs\n  method: post\n  operationId: createTimeOff\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /time-offs/{id}\n  method: get\n  operationId: getTimeOff\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /time-offs/{id}\n  method: put\n  operationId: updateTimeOff\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /time-offs/{id}\n  method: delete\n  operationId: deleteTimeOff\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swarmia/refs/heads/main/agentic-access/swarmia-agentic-access.yml
summary_line: 12 operations · 6 acting
tags:
- Engineering Effectiveness
- Developer Productivity
- DORA
- Software Delivery
- Analytics
---
