---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 11
api_specs:
- filename: eat-app-openapi.yml
  format: yaml
  label: Eat App Partner API
  slug: eat-app-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eat-app/refs/heads/main/openapi/eat-app-openapi.yml
- filename: eat-app-openapi.yml
  format: yaml
  label: Eat App Concierge Reservations API
  slug: eat-app-concierge-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eat-app/refs/heads/main/openapi/eat-app-openapi.yml
- filename: eat-app-openapi.yml
  format: yaml
  label: Eat App Concierge Guests API
  slug: eat-app-concierge-guests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eat-app/refs/heads/main/openapi/eat-app-openapi.yml
- filename: eat-app-openapi.yml
  format: yaml
  label: Eat App Concierge Availability API
  slug: eat-app-concierge-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eat-app/refs/heads/main/openapi/eat-app-openapi.yml
- filename: eat-app-openapi.yml
  format: yaml
  label: Eat App Concierge Restaurants and Groups API
  slug: eat-app-concierge-restaurants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eat-app/refs/heads/main/openapi/eat-app-openapi.yml
- filename: eat-app-openapi.yml
  format: yaml
  label: Eat App Tables and Floorplan API
  slug: eat-app-tables-floorplan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eat-app/refs/heads/main/openapi/eat-app-openapi.yml
consequence_counts:
  read: 11
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Eat App Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'Eat App exposes 15 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Eat App
provider_slug: eat-app
slug: eat-app-agentic-access
source_filename: eat-app-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/eat-app-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 11\n    acting: 4\n  by_consequence:\n    read: 11\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /partners/v2/availability\n  method: get\n  operationId: getPartnerAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /partners/v2/reservations\n  method: post\n  operationId: createPartnerReservation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /concierge/v2/resources\n  method: get\n  operationId: getConciergeResources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /concierge/v2/groups\n  method: get\n  operationId: listConciergeGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /concierge/v2/restaurants\n  method: get\n  operationId: listConciergeRestaurants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /concierge/v2/availability/range\n  method: post\n  operationId: getConciergeAvailabilityRange\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /concierge/v2/reservations\n  method: get\n  operationId: listConciergeReservations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /concierge/v2/reservations\n  method: post\n  operationId: createConciergeReservation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /concierge/v2/reservations/{id_or_key}\n  method: get\n  operationId: getConciergeReservation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /concierge/v2/reservations/{id_or_key}\n  method: patch\n  operationId: updateConciergeReservation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /concierge/v2/guests\n  method: get\n  operationId: searchConciergeGuests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /concierge/v2/guests/{guest_id}\n  method: get\n  operationId: getConciergeGuest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /concierge/v2/tables\n  method: get\n  operationId: listTables\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /concierge/v2/tables/{table_id}\n  method: get\n  operationId: getTable\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /concierge/v2/floor_plans\n  method: get\n  operationId: listFloorPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eat-app/refs/heads/main/agentic-access/eat-app-agentic-access.yml
summary_line: 15 operations · 4 acting
tags:
- Restaurant
- Reservations
- Table Management
- Hospitality
- Bookings
- Guest CRM
- Availability
---
