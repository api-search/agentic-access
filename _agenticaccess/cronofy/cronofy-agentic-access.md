---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 6
api_specs:
- filename: cronofy-openapi.yml
  format: yaml
  label: Cronofy Calendars API
  slug: calendars
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cronofy/refs/heads/main/openapi/cronofy-openapi.yml
- filename: cronofy-openapi.yml
  format: yaml
  label: Cronofy Events API
  slug: events
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cronofy/refs/heads/main/openapi/cronofy-openapi.yml
- filename: cronofy-openapi.yml
  format: yaml
  label: Cronofy Availability API
  slug: availability
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cronofy/refs/heads/main/openapi/cronofy-openapi.yml
- filename: cronofy-openapi.yml
  format: yaml
  label: Cronofy Smart Invites API
  slug: smart-invites
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cronofy/refs/heads/main/openapi/cronofy-openapi.yml
- filename: cronofy-openapi.yml
  format: yaml
  label: Cronofy Scheduling Links API
  slug: scheduling-links
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cronofy/refs/heads/main/openapi/cronofy-openapi.yml
- filename: cronofy-openapi.yml
  format: yaml
  label: Cronofy Push Notifications API
  slug: push-notifications
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cronofy/refs/heads/main/openapi/cronofy-openapi.yml
consequence_counts:
  read: 6
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cronofy Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'Cronofy exposes 16 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 10 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cronofy
provider_slug: cronofy
slug: cronofy-agentic-access
source_filename: cronofy-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/cronofy-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 6\n    acting: 10\n  by_consequence:\n    read: 6\n    write: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /userinfo\n  method: get\n  operationId: getUserInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calendars\n  method: get\n  operationId: listCalendars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calendars\n  method: post\n  operationId: createCalendar\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events\n  method: get\n  operationId: readEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /free_busy\n  method: get\n  operationId: readFreeBusy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calendars/{calendar_id}/events\n  method: post\n  operationId: upsertEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /calendars/{calendar_id}/events\n  method: delete\n  operationId: deleteEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /availability\n  method: post\n  operationId: availabilityQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sequenced_availability\n  method: post\n  operationId: sequencedAvailability\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /real_time_scheduling\n  method: post\n  operationId: realTimeScheduling\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /real_time_sequencing\n  method: post\n  operationId: realTimeSequencing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /smart_invites\n  method: post\n  operationId: upsertSmartInvite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /smart_invites\n  method: get\n  operationId: getSmartInvite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /channels\n  method: post\n  operationId: createChannel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /channels\n  method: get\n  operationId: listChannels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /channels/{channel_id}\n  method:\
  \ delete\n  operationId: closeChannel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cronofy/refs/heads/main/agentic-access/cronofy-agentic-access.yml
summary_line: 16 operations · 10 acting
tags:
- Scheduling
- Calendar
- Availability
- Booking
- Productivity
---
