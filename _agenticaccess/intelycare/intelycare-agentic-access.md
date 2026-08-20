---
acting_count: 6
action_class_counts:
  acting: 6
api_specs:
- filename: intelycare-external-scheduling-openapi.yml
  format: yaml
  label: IntelyCare External Scheduling API
  slug: intelycare-external-scheduling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelycare/refs/heads/main/openapi/intelycare-external-scheduling-openapi.yml
consequence_counts:
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Intelycare Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'IntelyCare exposes 6 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: IntelyCare
provider_slug: intelycare
slug: intelycare-agentic-access
source_filename: intelycare-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: generated\nsource: openapi/intelycare-external-scheduling-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    acting: 6\n  by_consequence:\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /api/shifts\n  method: post\n  operationId: shift_create_api_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/shifts/{shiftId}\n  method: put\n  operationId: shift_update_api_v1\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/shifts/{shiftId}\n  method: delete\n  operationId: shift_delete_api_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/timecards\n  method: post\n  operationId: timecard_create_api_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/timecards\n  method: put\n  operationId:\
  \ update_timecard_api_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/clockinout/{platform_type}\n  method: post\n  operationId: check_in_out_api_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intelycare/refs/heads/main/agentic-access/intelycare-agentic-access.yml
summary_line: 6 operations · 6 acting
tags:
- Healthcare
- Healthcare Staffing
- Nursing
- Workforce Management
- Scheduling
- Shift Management
- Timekeeping
- Marketplace
- Webhook
- Per Diem
- Credentialing
- Post-Acute Care
---
