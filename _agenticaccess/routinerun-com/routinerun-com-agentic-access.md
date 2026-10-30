---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 6
api_specs:
- filename: routinerun-com-commands-api-openapi.yml
  format: yaml
  label: routinerun-com Commands API
  slug: routinerun-com-commands-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/routinerun-com/openapi/routinerun-com-commands-api-openapi.yml
- filename: routinerun-com-events-api-openapi.yml
  format: yaml
  label: routinerun-com Events API
  slug: routinerun-com-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/routinerun-com/openapi/routinerun-com-events-api-openapi.yml
- filename: routinerun-com-history-api-openapi.yml
  format: yaml
  label: routinerun-com History API
  slug: routinerun-com-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/routinerun-com/openapi/routinerun-com-history-api-openapi.yml
- filename: routinerun-com-pagerduty-api-openapi.yml
  format: yaml
  label: routinerun-com Pagerduty API
  slug: routinerun-com-pagerduty-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/routinerun-com/openapi/routinerun-com-pagerduty-api-openapi.yml
- filename: routinerun-com-routines-api-openapi.yml
  format: yaml
  label: routinerun-com Routines API
  slug: routinerun-com-routines-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/routinerun-com/openapi/routinerun-com-routines-api-openapi.yml
- filename: routinerun-com-runs-api-openapi.yml
  format: yaml
  label: routinerun-com Runs API
  slug: routinerun-com-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/routinerun-com/openapi/routinerun-com-runs-api-openapi.yml
consequence_counts:
  read: 6
  safety-critical: 1
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Routinerun Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /runs/{run}/stop
operation_count: 18
overview: 'routinerun-com exposes 18 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 11 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: routinerun-com
provider_slug: routinerun-com
slug: routinerun-com-agentic-access
source_filename: routinerun-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/routinerun-com-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    acting: 12\n    connected: 6\n  by_consequence:\n    write: 11\n    read: 6\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /events\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /runs\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /runs\n  method: get\n  operationId: listRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /runs/{run}/next\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /runs/{run}/notes\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /runs/{run}/values/{key}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /routines/{routine}/steps\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pagerduty\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commands/{command}\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /runs/{run}/pause\n  method: post\n  operationId: pauseRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /runs/{run}/resume\n  method: post\n  operationId: resumeRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /runs/{run}/stop\n  method: post\n  operationId: stopRun\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /runs/{run}/later\n  method: post\n  operationId: putLater\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /runs/{run}/last\n  method: post\n  operationId: putLast\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /routines\n  method: get\n  operationId: listRoutines\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /routines/{routine}\n  method: get\n  operationId: getRoutine\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /runs/{run}\n  method: get\n  operationId: getRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /history\n  method: get\n  operationId: getHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/routinerun-com/agentic-access/routinerun-com-agentic-access.yml
summary_line: 18 operations · 12 acting · 1 human-in-the-loop
tags:
- Automation
- Scheduling
- Cloud
- DevOps
- API
---
