---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 2
api_specs:
- filename: simplevoip-call-recordings-api-openapi.yml
  format: yaml
  label: SimpleVoIP Call Recordings API
  slug: simplevoip-call-recordings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/simplevoip/openapi/simplevoip-call-recordings-api-openapi.yml
- filename: simplevoip-cdr-api-openapi.yml
  format: yaml
  label: SimpleVoIP CDR API
  slug: simplevoip-cdr-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/simplevoip/openapi/simplevoip-cdr-api-openapi.yml
- filename: simplevoip-music-on-hold-api-openapi.yml
  format: yaml
  label: SimpleVoIP Music on Hold API
  slug: simplevoip-music-on-hold-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/simplevoip/openapi/simplevoip-music-on-hold-api-openapi.yml
- filename: simplevoip-sms-api-openapi.yml
  format: yaml
  label: SimpleVoIP SMS API
  slug: simplevoip-sms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/simplevoip/openapi/simplevoip-sms-api-openapi.yml
- filename: simplevoip-time-of-day-api-openapi.yml
  format: yaml
  label: SimpleVoIP Time of Day API
  slug: simplevoip-time-of-day-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/simplevoip/openapi/simplevoip-time-of-day-api-openapi.yml
consequence_counts:
  physical: 1
  read: 2
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Simplevoip Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sms/send
operation_count: 5
overview: 'SimpleVoIP exposes 5 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read, 2 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SimpleVoIP
provider_slug: simplevoip
slug: simplevoip-agentic-access
source_filename: simplevoip-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: generated\nsource: openapi/simplevoip-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    acting: 3\n    connected: 2\n  by_consequence:\n    physical: 1\n    read: 2\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /sms/send\n  method: post\n  operationId: sendSms\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{parent_id}/tod_rules\n  method: get\n  operationId:\
  \ fetchTodRules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tod_rules\n  method: put\n  operationId: modifyTodRules\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /moh\n  method: put\n  operationId: modifyMusicOnHold\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recording/{account_id}/{recording_id}\n  method: get\n  operationId: fetchCallRecording\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/simplevoip/agentic-access/simplevoip-agentic-access.yml
summary_line: 5 operations · 3 acting
tags:
- VoIP
- Communications
- UCaaS
- Artificial Intelligence
- Small Business
---
