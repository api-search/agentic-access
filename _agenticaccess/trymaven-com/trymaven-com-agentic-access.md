---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 6
api_specs:
- filename: trymaven-com-health-api-openapi.yml
  format: yaml
  label: Maven Health API
  slug: trymaven-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trymaven-com/openapi/trymaven-com-health-api-openapi.yml
- filename: trymaven-com-public-api-v1-api-openapi.yml
  format: yaml
  label: Maven Public API (v1) API
  slug: trymaven-com-public-api-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trymaven-com/openapi/trymaven-com-public-api-v1-api-openapi.yml
- filename: trymaven-com-retell-api-openapi.yml
  format: yaml
  label: Maven Retell API
  slug: trymaven-com-retell-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trymaven-com/openapi/trymaven-com-retell-api-openapi.yml
- filename: trymaven-com-vapi-api-openapi.yml
  format: yaml
  label: Maven VAPI API
  slug: trymaven-com-vapi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trymaven-com/openapi/trymaven-com-vapi-api-openapi.yml
- filename: trymaven-com-widget-sessions-api-openapi.yml
  format: yaml
  label: Maven Widget Sessions API
  slug: trymaven-com-widget-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trymaven-com/openapi/trymaven-com-widget-sessions-api-openapi.yml
consequence_counts:
  physical: 1
  read: 6
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Trymaven Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/widget-sessions
operation_count: 11
overview: 'Maven exposes 11 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 4 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Maven
provider_slug: trymaven-com
slug: trymaven-com-agentic-access
source_filename: trymaven-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: generated\nsource: openapi/trymaven-com-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 6\n    acting: 5\n  by_consequence:\n    read: 6\n    write: 4\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /health\n  method: get\n  operationId: health_check_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/auth/check\n  method: get\n  operationId: check_auth_v1_auth_check_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/projects\n  method: get\n  operationId: list_projects_v1_projects_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sessions\n  method: post\n  operationId: create_session_v1_sessions_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sessions\n  method: get\n  operationId: get_session_by_caller_v1_sessions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sessions/{session_id}\n  method: get\n  operationId: get_session_v1_sessions__session_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sessions/{session_id}/stream\n  method: get\n  operationId: stream_session_v1_sessions__session_id__stream_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sessions/{session_id}/cancel\n  method: post\n  operationId: cancel_session_v1_sessions__session_id__cancel_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/widget-sessions\n  method: post\n  operationId: create_widget_session_v1_widget_sessions_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n\
  \      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integrations/vapi/webhook\n  method: post\n  operationId: vapi_webhook_integrations_vapi_webhook_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integrations/retell/webhook\n  method: post\n  operationId: retell_webhook_integrations_retell_webhook_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/trymaven-com/agentic-access/trymaven-com-agentic-access.yml
summary_line: 11 operations · 5 acting
tags:
- Payments
- Voice AI
- Chatbots
- Fintech
- Y Combinator
---
