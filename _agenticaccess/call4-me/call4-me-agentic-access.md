---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 9
api_specs:
- filename: call4-me-balance-api-openapi.yml
  format: yaml
  label: call4me Balance API
  slug: call4-me-balance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/call4-me/openapi/call4-me-balance-api-openapi.yml
- filename: call4-me-call4me-api-api-openapi.yml
  format: yaml
  label: call4me Call4me API
  slug: call4-me-call4me-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/call4-me/openapi/call4-me-call4me-api-api-openapi.yml
- filename: call4-me-calls-api-openapi.yml
  format: yaml
  label: call4me Calls API
  slug: call4-me-calls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/call4-me/openapi/call4-me-calls-api-openapi.yml
- filename: call4-me-numbers-api-openapi.yml
  format: yaml
  label: call4me Numbers API
  slug: call4-me-numbers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/call4-me/openapi/call4-me-numbers-api-openapi.yml
- filename: call4-me-profile-api-openapi.yml
  format: yaml
  label: call4me Profile API
  slug: call4-me-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/call4-me/openapi/call4-me-profile-api-openapi.yml
- filename: call4-me-requirements-api-openapi.yml
  format: yaml
  label: call4me Requirements API
  slug: call4-me-requirements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/call4-me/openapi/call4-me-requirements-api-openapi.yml
- filename: call4-me-scheduled-calls-api-openapi.yml
  format: yaml
  label: call4me Scheduled Calls API
  slug: call4-me-scheduled-calls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/call4-me/openapi/call4-me-scheduled-calls-api-openapi.yml
- filename: call4-me-x402-api-openapi.yml
  format: yaml
  label: call4me X402 API
  slug: call4-me-x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/call4-me/openapi/call4-me-x402-api-openapi.yml
consequence_counts:
  physical: 1
  read: 9
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Call4 Me Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/numbers/own
operation_count: 22
overview: 'call4me exposes 22 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 12 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: call4me
provider_slug: call4-me
slug: call4-me-agentic-access
source_filename: call4-me-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/call4-me-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 9\n    acting: 13\n  by_consequence:\n    read: 9\n    write: 12\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api\n  method: get\n  operationId: buyCredits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/x402/calls\n  method: post\n  operationId: placePaidCall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/balance\n  method: get\n  operationId: getBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/requirements\n  method: get\n  operationId: listCallCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/requirements/{category}\n  method: get\n  operationId: getCallRequirements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/profile\n  method: get\n  operationId: getProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/profile\n  method:\
  \ patch\n  operationId: saveProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/calls\n  method: get\n  operationId: listCalls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/calls\n  method: post\n  operationId: placeCall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/calls/{call_id}\n  method: get\n  operationId: getCall\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/calls/{call_id}/answer\n  method: post\n  operationId: answerQuestion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/calls/{call_id}/connect\n  method: post\n  operationId: connectUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/calls/{call_id}/hang-up\n  method: post\n  operationId: hangUp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n  \
  \    max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/scheduled-calls\n  method: post\n  operationId: scheduleCall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/scheduled-calls/{scheduled_id}\n  method: delete\n  operationId: cancelScheduledCall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/numbers\n  method: get\n  operationId: listNumbers\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/numbers\n  method: post\n  operationId: buyNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/numbers/{number}\n  method: delete\n  operationId: releaseNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/numbers/own\n  method: post\n  operationId: sendNumberVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/numbers/own/{number}/verify\n  method: post\n  operationId: confirmNumberVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/numbers/own/{number}\n  method: delete\n  operationId: removeOwnNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/calls/{call_id}/recordings\n  method: get\n  operationId:\
  \ getCallRecordings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/call4-me/agentic-access/call4-me-agentic-access.yml
summary_line: 22 operations · 13 acting
tags:
- Artificial Intelligence
- Telephony
- Automation
- Software-as-a-Service
- Call4me
---
