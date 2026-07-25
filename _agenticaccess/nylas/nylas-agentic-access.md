---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 14
api_specs:
- filename: nylas-admin-api-openapi.yml
  format: yaml
  label: Nylas Admin API
  slug: nylas-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nylas/refs/heads/main/openapi/nylas-admin-api-openapi.yml
- filename: nylas-auth-api-openapi.yml
  format: yaml
  label: Nylas Auth API
  slug: nylas-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nylas/refs/heads/main/openapi/nylas-auth-api-openapi.yml
- filename: nylas-calendars-api-openapi.yml
  format: yaml
  label: Nylas Calendars API
  slug: nylas-calendars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nylas/refs/heads/main/openapi/nylas-calendars-api-openapi.yml
- filename: nylas-contacts-api-openapi.yml
  format: yaml
  label: Nylas Contacts API
  slug: nylas-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nylas/refs/heads/main/openapi/nylas-contacts-api-openapi.yml
- filename: nylas-drafts-api-openapi.yml
  format: yaml
  label: Nylas Drafts API
  slug: nylas-drafts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nylas/refs/heads/main/openapi/nylas-drafts-api-openapi.yml
- filename: nylas-events-api-openapi.yml
  format: yaml
  label: Nylas Events API
  slug: nylas-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nylas/refs/heads/main/openapi/nylas-events-api-openapi.yml
- filename: nylas-grants-api-openapi.yml
  format: yaml
  label: Nylas Grants API
  slug: nylas-grants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nylas/refs/heads/main/openapi/nylas-grants-api-openapi.yml
- filename: nylas-messages-api-openapi.yml
  format: yaml
  label: Nylas Messages API
  slug: nylas-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nylas/refs/heads/main/openapi/nylas-messages-api-openapi.yml
- filename: nylas-scheduling-api-openapi.yml
  format: yaml
  label: Nylas Scheduling API
  slug: nylas-scheduling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nylas/refs/heads/main/openapi/nylas-scheduling-api-openapi.yml
- filename: nylas-threads-api-openapi.yml
  format: yaml
  label: Nylas Threads API
  slug: nylas-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nylas/refs/heads/main/openapi/nylas-threads-api-openapi.yml
consequence_counts:
  physical: 1
  read: 14
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Nylas Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/grants/{grant_id}/messages
operation_count: 22
overview: 'Nylas exposes 22 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read, 7 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Nylas
provider_slug: nylas
slug: nylas-agentic-access
source_filename: nylas-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/nylas-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    acting: 8\n    connected: 14\n  by_consequence:\n    write: 7\n    read: 14\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v3/connect/custom\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/connect/auth\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/connect/token\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/grants\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/grants/{grant_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/grants/{grant_id}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n     \
  \ triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/grants/{grant_id}/messages\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/grants/{grant_id}/messages\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/grants/{grant_id}/threads\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/grants/{grant_id}/drafts\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/grants/{grant_id}/drafts\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/grants/{grant_id}/calendars\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/grants/{grant_id}/events\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/grants/{grant_id}/events\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/grants/{grant_id}/contacts\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/scheduling/configurations\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/scheduling/bookings\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/scheduling/availability\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v3/applications\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/connectors\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/webhooks\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/webhooks\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nylas/refs/heads/main/agentic-access/nylas-agentic-access.yml
summary_line: 22 operations · 8 acting
tags:
- Calendar
- Communication
- Contacts
- Email
- Messaging
- Scheduling
---
