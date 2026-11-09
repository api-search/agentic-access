---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 6
api_specs:
- filename: agendaforge-app-connection-api-openapi.yml
  format: yaml
  label: agendaforge-app Connection API
  slug: agendaforge-app-connection-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agendaforge-app/openapi/agendaforge-app-connection-api-openapi.yml
- filename: agendaforge-app-jobs-api-openapi.yml
  format: yaml
  label: agendaforge-app Jobs API
  slug: agendaforge-app-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agendaforge-app/openapi/agendaforge-app-jobs-api-openapi.yml
- filename: agendaforge-app-records-api-openapi.yml
  format: yaml
  label: agendaforge-app Records API
  slug: agendaforge-app-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agendaforge-app/openapi/agendaforge-app-records-api-openapi.yml
- filename: agendaforge-app-webhooks-api-openapi.yml
  format: yaml
  label: agendaforge-app Webhooks API
  slug: agendaforge-app-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agendaforge-app/openapi/agendaforge-app-webhooks-api-openapi.yml
consequence_counts:
  read: 6
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Agendaforge App Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'agendaforge-app exposes 14 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: agendaforge-app
provider_slug: agendaforge-app
slug: agendaforge-app-agentic-access
source_filename: agendaforge-app-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/agendaforge-app-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 6\n    acting: 8\n  by_consequence:\n    read: 6\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/me\n  method: get\n  operationId: getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - public_api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/hooks\n  method: post\n  operationId: subscribeHook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - public_api\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/hooks/{id}\n  method: delete\n  operationId: unsubscribeHook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - public_api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/triggers/{event}/sample\n  method: get\n  operationId: getTriggerSample\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - public_api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/contacts\n  method: get\n  operationId: listContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - public_api\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /api/v1/contacts\n  method: post\n  operationId: createContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - public_api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/contacts/batch\n  method: post\n  operationId: createContactsBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - public_api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/imports/contacts\n  method: post\n  operationId: importContacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - public_api\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/imports/tickets\n  method: post\n  operationId: importTickets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - tickets:import\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/jobs/{id}\n  method: get\n  operationId: getJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - public_api\n    - tickets:import\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sessions\n  method: get\n  operationId: listSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    scope:\n    - public_api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sessions\n  method: post\n  operationId: createSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - public_api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sponsors\n  method: get\n  operationId: listSponsors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - public_api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sponsors\n  method: post\n  operationId: createSponsor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - public_api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/agendaforge-app/agentic-access/agendaforge-app-agentic-access.yml
summary_line: 14 operations · 8 acting
tags:
- Event Management
- Software-as-a-Service
- AI-native
- Conferences
- Software
---
