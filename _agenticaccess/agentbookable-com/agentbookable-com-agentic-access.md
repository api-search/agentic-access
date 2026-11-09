---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 5
api_specs:
- filename: agentbookable-com-availability-api-openapi.yml
  format: yaml
  label: Agentbookable Availability API
  slug: agentbookable-com-availability-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentbookable-com/openapi/agentbookable-com-availability-api-openapi.yml
- filename: agentbookable-com-bookings-api-openapi.yml
  format: yaml
  label: Agentbookable Bookings API
  slug: agentbookable-com-bookings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentbookable-com/openapi/agentbookable-com-bookings-api-openapi.yml
- filename: agentbookable-com-discovery-api-openapi.yml
  format: yaml
  label: Agentbookable Discovery API
  slug: agentbookable-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentbookable-com/openapi/agentbookable-com-discovery-api-openapi.yml
- filename: agentbookable-com-mandates-api-openapi.yml
  format: yaml
  label: Agentbookable Mandates API
  slug: agentbookable-com-mandates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentbookable-com/openapi/agentbookable-com-mandates-api-openapi.yml
- filename: agentbookable-com-services-api-openapi.yml
  format: yaml
  label: Agentbookable Services API
  slug: agentbookable-com-services-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentbookable-com/openapi/agentbookable-com-services-api-openapi.yml
consequence_counts:
  read: 5
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Agentbookable Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'Agentbookable exposes 11 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Agentbookable
provider_slug: agentbookable-com
slug: agentbookable-com-agentic-access
source_filename: agentbookable-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/agentbookable-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 5\n    acting: 6\n  by_consequence:\n    read: 5\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /businesses\n  method: get\n  operationId: searchBusinesses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /businesses/{businessId}\n  method: get\n  operationId: getBusiness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /businesses/{businessId}/services\n\
  \  method: get\n  operationId: listServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /businesses/{businessId}/availability\n  method: post\n  operationId: findAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /booking-drafts\n  method: post\n  operationId: createBookingDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mandates\n  method: post\n  operationId: createMandate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n  \
  \  escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mandates/for-draft\n  method: post\n  operationId: createMandateForDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bookings\n  method: post\n  operationId: createBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bookings/{bookingId}\n  method: get\n  operationId: getBooking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /bookings/{bookingId}/reschedule\n  method: post\n  operationId: rescheduleBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bookings/{bookingId}/cancel\n  method: post\n  operationId: cancelBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/agentbookable-com/agentic-access/agentbookable-com-agentic-access.yml
summary_line: 11 operations · 6 acting
tags:
- Booking
- Artificial Intelligence
- Scheduling
- Integration
- Automation
- Company
---
