---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 12
api_specs:
- filename: addevent-calendar-subscribers-api-openapi.yml
  format: yaml
  label: AddEvent Calendar subscribers API
  slug: addevent-calendar-subscribers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addevent/openapi/addevent-calendar-subscribers-api-openapi.yml
- filename: addevent-calendars-api-openapi.yml
  format: yaml
  label: AddEvent Calendars API
  slug: addevent-calendars-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addevent/openapi/addevent-calendars-api-openapi.yml
- filename: addevent-events-api-openapi.yml
  format: yaml
  label: AddEvent Events API
  slug: addevent-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addevent/openapi/addevent-events-api-openapi.yml
- filename: addevent-rsvp-attendees-api-openapi.yml
  format: yaml
  label: AddEvent RSVP attendees API
  slug: addevent-rsvp-attendees-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addevent/openapi/addevent-rsvp-attendees-api-openapi.yml
- filename: addevent-templates-api-openapi.yml
  format: yaml
  label: AddEvent Templates API
  slug: addevent-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addevent/openapi/addevent-templates-api-openapi.yml
- filename: addevent-timezones-api-openapi.yml
  format: yaml
  label: AddEvent Timezones API
  slug: addevent-timezones-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addevent/openapi/addevent-timezones-api-openapi.yml
consequence_counts:
  read: 12
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Addevent Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'AddEvent exposes 22 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read and 10 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AddEvent
provider_slug: addevent
slug: addevent-agentic-access
source_filename: addevent-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: generated\nsource: openapi/addevent-calendar-and-event-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    acting: 10\n    connected: 12\n  by_consequence:\n    write: 10\n    read: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /calendars\n  method: post\n  operationId: create-calendar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calendars\n  method: get\n  operationId: search-calendars\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calendars/templates\n  method: get\n  operationId: list-calendar-templates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calendars/{calendar_id}\n  method: get\n  operationId: retrieve-calendar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calendars/{calendar_id}\n  method: patch\n  operationId: update-calendar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calendars/{calendar_id}\n  method: delete\n  operationId: delete-calendar\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events\n  method: post\n  operationId: create-event\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events\n  method: get\n  operationId: search-events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/rsvp-forms\n  method: get\n  operationId: list-rsvp-forms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /events/templates\n  method: get\n  operationId: list-event-templates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{event_id}\n  method: get\n  operationId: retrieve-event\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{event_id}\n  method: patch\n  operationId: update-event\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/{event_id}\n  method: delete\n  operationId: delete-event\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/{event_id}/rsvps\n  method: post\n  operationId: create-rsvp-attendee\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rsvps\n  method: get\n  operationId: search-rsvp-attendees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rsvps/{attendee_id}\n  method: get\n  operationId: retrieve-rsvp-attendee\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /rsvps/{attendee_id}\n  method: patch\n  operationId: update-rsvp-attendee\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rsvps/{attendee_id}\n  method: delete\n  operationId: delete-rsvp-attendee\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscribers\n  method: get\n  operationId: search-calendar-subscribers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscribers/{subscriber_id}\n  method: get\n\
  \  operationId: retrieve-calendar-subscriber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscribers/{subscriber_id}\n  method: delete\n  operationId: delete-calendar-subscriber\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /timezones\n  method: get\n  operationId: list-timezones\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/addevent/agentic-access/addevent-agentic-access.yml
summary_line: 22 operations · 10 acting
tags:
- Calendar
- Integration
- Marketing
- Software-as-a-Service
- Event
---
