---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 4
api_specs:
- filename: spurwing-openapi.yml
  format: yaml
  label: Spurwing Providers API
  slug: providers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spurwing/refs/heads/main/openapi/spurwing-openapi.yml
- filename: spurwing-openapi.yml
  format: yaml
  label: Spurwing Availability API
  slug: availability
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spurwing/refs/heads/main/openapi/spurwing-openapi.yml
- filename: spurwing-openapi.yml
  format: yaml
  label: Spurwing Appointments API
  slug: appointments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spurwing/refs/heads/main/openapi/spurwing-openapi.yml
- filename: spurwing-openapi.yml
  format: yaml
  label: Spurwing Services API
  slug: services
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spurwing/refs/heads/main/openapi/spurwing-openapi.yml
consequence_counts:
  read: 4
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Spurwing Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Spurwing exposes 7 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Spurwing
provider_slug: spurwing
slug: spurwing-agentic-access
source_filename: spurwing-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/spurwing-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 4\n    acting: 3\n  by_consequence:\n    read: 4\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /appointment_types.json\n  method: get\n  operationId: getAppointmentTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bookings/days_available.json\n  method: get\n  operationId: getDaysAvailable\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bookings/slots_available.json\n\
  \  method: get\n  operationId: getSlotsAvailable\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bookings/complete_booking.json\n  method: post\n  operationId: completeBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /appointments\n  method: get\n  operationId: listAppointments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /appointments\n  method: post\n  operationId: createGroupAppointment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /appointments/{appointment_id}\n  method: delete\n  operationId: deleteAppointment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spurwing/refs/heads/main/agentic-access/spurwing-agentic-access.yml
summary_line: 7 operations · 3 acting
tags:
- Scheduling
- Appointments
- Booking
- Calendar
- Availability
---
