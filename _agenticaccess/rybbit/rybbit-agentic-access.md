---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 9
api_specs:
- filename: rybbit-openapi.yml
  format: yaml
  label: Rybbit Event Tracking API
  slug: rybbit-event-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rybbit/refs/heads/main/openapi/rybbit-openapi.yml
- filename: rybbit-openapi.yml
  format: yaml
  label: Rybbit Sites API
  slug: rybbit-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rybbit/refs/heads/main/openapi/rybbit-openapi.yml
- filename: rybbit-openapi.yml
  format: yaml
  label: Rybbit Analytics Stats API
  slug: rybbit-analytics-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rybbit/refs/heads/main/openapi/rybbit-openapi.yml
- filename: rybbit-openapi.yml
  format: yaml
  label: Rybbit Sessions & Retention API
  slug: rybbit-sessions-retention-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rybbit/refs/heads/main/openapi/rybbit-openapi.yml
consequence_counts:
  physical: 1
  read: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Rybbit Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/track
operation_count: 10
overview: 'Rybbit exposes 10 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Rybbit
provider_slug: rybbit
slug: rybbit-agentic-access
source_filename: rybbit-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/rybbit-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    acting: 1\n    connected: 9\n  by_consequence:\n    physical: 1\n    read: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /api/track\n  method: post\n  operationId: trackEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/sites/{site}/sessions\n  method: get\n  operationId: listSessions\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/sites/{site}/sessions/{sessionId}\n  method: get\n  operationId: getSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/sites/{site}/session-locations\n  method: get\n  operationId: listSessionLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/sites/{site}/users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/sites/{site}/users/{userId}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/sites/{site}/users/{userId}/sessions\n  method: get\n  operationId: listUserSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/sites/{site}/users/session-count\n  method: get\n  operationId: getUserSessionCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/sites/{site}/retention\n  method: get\n  operationId: getRetention\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/sites/{site}/journeys\n  method: get\n  operationId: getJourneys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n \
  \   audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rybbit/refs/heads/main/agentic-access/rybbit-agentic-access.yml
summary_line: 10 operations · 1 acting
tags:
- Analytics
- Web Analytics
- Product Analytics
- Privacy
- Open Source
- Cookieless
---
