---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 6
api_specs:
- filename: demio-events-api-openapi.yml
  format: yaml
  label: Demio Events API
  slug: demio-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demio/refs/heads/main/openapi/demio-events-api-openapi.yml
- filename: demio-intro-api-openapi.yml
  format: yaml
  label: Demio Intro API
  slug: demio-intro-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demio/refs/heads/main/openapi/demio-intro-api-openapi.yml
- filename: demio-reports-api-openapi.yml
  format: yaml
  label: Demio Reports API
  slug: demio-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demio/refs/heads/main/openapi/demio-reports-api-openapi.yml
consequence_counts:
  read: 6
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Demio Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Demio exposes 7 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Demio
provider_slug: demio
slug: demio-agentic-access
source_filename: demio-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: generated\nsource: openapi/demio-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 6\n    acting: 1\n  by_consequence:\n    read: 6\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /ping\n  method: get\n  operationId: pingViaHeaders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ping/query\n  method: get\n  operationId: pingViaQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events\n  method: get\n  operationId: listEvents\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /event/{id}\n  method: get\n  operationId: getEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /event/{id}/date/{date_id}\n  method: get\n  operationId: getEventSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /event/register\n  method: put\n  operationId: registerForEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /report/{date_id}/participants\n  method: get\n  operationId:\
  \ listSessionParticipants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/demio/refs/heads/main/agentic-access/demio-agentic-access.yml
summary_line: 7 operations · 1 acting
tags:
- Company
- Webinars
- Virtual Events
- Event Management
- Marketing
- Marketing Technology
- Demand Generation
- Video
- Engagement Marketing
- Lead Generation
- Software-as-a-Service
---
