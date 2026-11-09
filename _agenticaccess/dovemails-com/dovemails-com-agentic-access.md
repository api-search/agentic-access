---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 1
api_specs:
- filename: dovemails-com-send-api-openapi.yml
  format: yaml
  label: dovemails-com Send API
  slug: dovemails-com-send-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dovemails-com/openapi/dovemails-com-send-api-openapi.yml
- filename: dovemails-com-status-api-openapi.yml
  format: yaml
  label: dovemails-com Status API
  slug: dovemails-com-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dovemails-com/openapi/dovemails-com-status-api-openapi.yml
consequence_counts:
  physical: 2
  read: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Dovemails Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/send/batch
operation_count: 3
overview: 'dovemails-com exposes 3 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: dovemails-com
provider_slug: dovemails-com
slug: dovemails-com-agentic-access
source_filename: dovemails-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/dovemails-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 3\n  by_action_class:\n    connected: 1\n    acting: 2\n  by_consequence:\n    read: 1\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /healthz\n  method: get\n  operationId: healthz_healthz_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/send\n  method: post\n  operationId: send_api_v1_send_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n  \
  \    purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/send/batch\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/dovemails-com/agentic-access/dovemails-com-agentic-access.yml
summary_line: 3 operations · 2 acting
tags:
- Company
- Email
- Software-as-a-Service
- Marketing
---
