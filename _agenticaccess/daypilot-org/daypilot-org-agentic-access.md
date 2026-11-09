---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 16
api_specs:
- filename: daypilot-org-discovery-api-openapi.yml
  format: yaml
  label: DayPilot Discovery API
  slug: daypilot-org-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daypilot-org/openapi/daypilot-org-discovery-api-openapi.yml
- filename: daypilot-org-generation-api-openapi.yml
  format: yaml
  label: DayPilot Generation API
  slug: daypilot-org-generation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daypilot-org/openapi/daypilot-org-generation-api-openapi.yml
consequence_counts:
  read: 16
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Daypilot Org Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 18
overview: 'DayPilot exposes 18 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: DayPilot
provider_slug: daypilot-org
slug: daypilot-org-agentic-access
source_filename: daypilot-org-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/daypilot-org-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    connected: 16\n    acting: 2\n  by_consequence:\n    read: 16\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1\n  method: get\n  operationId: getBuilderServiceIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1\n  method: head\n  operationId: headBuilderServiceIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1\n  method: options\n\
  \  operationId: optionsBuilderServiceIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/components\n  method: get\n  operationId: listBuilderComponents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/components\n  method: head\n  operationId: headBuilderComponents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/components\n  method: options\n  operationId: optionsBuilderComponents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/components/{component}/targets\n  method: get\n  operationId: listBuilderComponentTargets\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/components/{component}/targets\n  method: head\n  operationId: headBuilderComponentTargets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/components/{component}/targets\n  method: options\n  operationId: optionsBuilderComponentTargets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/components/{component}/settings\n  method: get\n  operationId: listBuilderComponentSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/components/{component}/settings\n  method: head\n  operationId: headBuilderComponentSettings\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/components/{component}/settings\n  method: options\n  operationId: optionsBuilderComponentSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/configurations/validate\n  method: post\n  operationId: validateBuilderConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/configurations/validate\n  method: head\n  operationId: headBuilderConfigurationValidationNotAllowed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/configurations/validate\n  method: options\n  operationId: optionsBuilderConfigurationValidation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/project-archives\n  method: post\n  operationId: generateBuilderProjectArchive\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/project-archives\n  method: head\n  operationId: headBuilderProjectArchiveNotAllowed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/project-archives\n  method: options\n  operationId:\
  \ optionsBuilderProjectArchive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/daypilot-org/agentic-access/daypilot-org-agentic-access.yml
summary_line: 18 operations · 2 acting
tags:
- Calendar
- Scheduler
- Gantt Chart
- UI Components
- Open Source
---
