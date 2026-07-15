---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 8
api_specs:
- filename: accelevents-openapi.yml
  format: yaml
  label: Accelevents Events API
  slug: accelevents-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelevents/refs/heads/main/openapi/accelevents-openapi.yml
- filename: accelevents-openapi.yml
  format: yaml
  label: Accelevents Attendees API
  slug: accelevents-attendees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelevents/refs/heads/main/openapi/accelevents-openapi.yml
- filename: accelevents-openapi.yml
  format: yaml
  label: Accelevents Ticketing Orders API
  slug: accelevents-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelevents/refs/heads/main/openapi/accelevents-openapi.yml
- filename: accelevents-openapi.yml
  format: yaml
  label: Accelevents Tickets API
  slug: accelevents-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelevents/refs/heads/main/openapi/accelevents-openapi.yml
- filename: accelevents-openapi.yml
  format: yaml
  label: Accelevents Sessions API
  slug: accelevents-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelevents/refs/heads/main/openapi/accelevents-openapi.yml
consequence_counts:
  read: 8
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Accelevents Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Accelevents exposes 12 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Accelevents
provider_slug: accelevents
slug: accelevents-agentic-access
source_filename: accelevents-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/accelevents-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 8\n    acting: 4\n  by_consequence:\n    read: 8\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /host/event/{eventUrl}/eventDetails\n  method: get\n  operationId: getEventDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /host/event/{eventUrl}/recurringStatus\n  method: get\n  operationId: getRecurringEventStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /events/{eventUrl}/staff/allAttendees\n  method: get\n  operationId: getAllAttendees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{eventUrl}/staff/people\n  method: get\n  operationId: getPeopleList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{eventUrl}/staff/orders\n  method: get\n  operationId: getTicketingOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{eventUrl}/staff/salesData\n  method: get\n  operationId: getTicketingSalesData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{eventUrl}/staff/ticketHolders/{barcodeId}\n\
  \  method: patch\n  operationId: updateTicketHolderByBarcode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/{eventUrl}/staff/exchangeTicketType\n  method: post\n  operationId: exchangeTicketType\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/{eventUrl}/staff/sessions\n  method: get\n  operationId: getSessionsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{eventUrl}/staff/sessions/{sessionId}\n\
  \  method: patch\n  operationId: updateSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/{eventUrl}/staff/speakers\n  method: get\n  operationId: getSpeakersList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{eventUrl}/staff/speakers\n  method: post\n  operationId: createSpeaker\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accelevents/refs/heads/main/agentic-access/accelevents-agentic-access.yml
summary_line: 12 operations · 4 acting
tags:
- Event Management
- Ticketing
- Events
- Registration
- Virtual Events
- Sessions
---
