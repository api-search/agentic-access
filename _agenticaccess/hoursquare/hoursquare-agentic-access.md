---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 3
api_specs:
- filename: hoursquare-attendance-api-openapi.yml
  format: yaml
  label: HourSquare Attendance API
  slug: hoursquare-attendance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hoursquare/openapi/hoursquare-attendance-api-openapi.yml
- filename: hoursquare-employees-api-openapi.yml
  format: yaml
  label: HourSquare Employees API
  slug: hoursquare-employees-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hoursquare/openapi/hoursquare-employees-api-openapi.yml
- filename: hoursquare-me-api-openapi.yml
  format: yaml
  label: HourSquare Me API
  slug: hoursquare-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hoursquare/openapi/hoursquare-me-api-openapi.yml
- filename: hoursquare-oauth-api-openapi.yml
  format: yaml
  label: HourSquare OAuth API
  slug: hoursquare-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hoursquare/openapi/hoursquare-oauth-api-openapi.yml
consequence_counts:
  read: 3
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Hoursquare Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'HourSquare exposes 7 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: HourSquare
provider_slug: hoursquare
slug: hoursquare-agentic-access
source_filename: hoursquare-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/hoursquare-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 3\n    acting: 4\n  by_consequence:\n    read: 3\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /api/public/v1/employees\n  method: get\n  operationId: Employees_List\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - employees.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/public/v1/employees/{id}/external-id\n  method: put\n  operationId: Employees_SetExternalId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n\
  \    - attendance.record\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/public/v1/me\n  method: get\n  operationId: Me_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/public/v1/time-clock/events\n  method: post\n  operationId: TimeClock_RecordEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - attendance.record\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/public/v1/time-entries\n  method: post\n  operationId: TimeEntries_Create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    scope:\n    - attendance.record\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/public/v1/time-entries\n  method: get\n  operationId: TimeEntries_List\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - attendance.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/public/v1/oauth/token\n  method: post\n  operationId: OAuth_Token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/hoursquare/agentic-access/hoursquare-agentic-access.yml
summary_line: 7 operations · 4 acting
tags:
- Human Resources
- Payroll
- Time Tracking
- Workforce Management
- Software-as-a-Service
---
