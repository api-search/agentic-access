---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 13
api_specs:
- filename: tickettailor-openapi.yml
  format: yaml
  label: Ticket Tailor Events API
  slug: tickettailor-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tickettailor/refs/heads/main/openapi/tickettailor-openapi.yml
- filename: tickettailor-openapi.yml
  format: yaml
  label: Ticket Tailor Event Series API
  slug: tickettailor-event-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tickettailor/refs/heads/main/openapi/tickettailor-openapi.yml
- filename: tickettailor-openapi.yml
  format: yaml
  label: Ticket Tailor Orders API
  slug: tickettailor-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tickettailor/refs/heads/main/openapi/tickettailor-openapi.yml
- filename: tickettailor-openapi.yml
  format: yaml
  label: Ticket Tailor Issued Tickets API
  slug: tickettailor-issued-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tickettailor/refs/heads/main/openapi/tickettailor-openapi.yml
- filename: tickettailor-openapi.yml
  format: yaml
  label: Ticket Tailor Vouchers API
  slug: tickettailor-vouchers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tickettailor/refs/heads/main/openapi/tickettailor-openapi.yml
- filename: tickettailor-openapi.yml
  format: yaml
  label: Ticket Tailor Check-ins API
  slug: tickettailor-check-ins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tickettailor/refs/heads/main/openapi/tickettailor-openapi.yml
consequence_counts:
  physical: 1
  read: 13
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tickettailor Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /orders/{id}
operation_count: 26
overview: 'Ticket Tailor exposes 26 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read, 12 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Ticket Tailor
provider_slug: tickettailor
slug: tickettailor-agentic-access
source_filename: tickettailor-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/tickettailor-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 26\n  by_action_class:\n    connected: 13\n    acting: 13\n  by_consequence:\n    read: 13\n    write: 12\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /ping\n  method: get\n  operationId: ping\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events\n  method: get\n  operationId: getAllEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{id}\n  method: get\n  operationId:\
  \ getEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /event_series\n  method: get\n  operationId: getAllEventSeries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /event_series\n  method: post\n  operationId: createEventSeries\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /event_series/{id}\n  method: get\n  operationId: getEventSeries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /event_series/{id}\n  method: put\n  operationId:\
  \ updateEventSeries\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /event_series/{id}\n  method: delete\n  operationId: deleteEventSeries\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /event_series/{id}/status\n  method: patch\n  operationId: updateEventSeriesStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /event_series/{id}/ticket_types\n  method: post\n  operationId: createTicketType\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /event_series/{id}/ticket_groups\n  method: post\n  operationId: createTicketGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders\n  method: get\n  operationId: getAllOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{id}\n  method: get\n\
  \  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{id}\n  method: patch\n  operationId: updateOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /issued_tickets\n  method: get\n  operationId: getAllIssuedTickets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /issued_tickets\n  method: post\n  operationId: createIssuedTicket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n    \
  \  max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /issued_tickets/{id}\n  method: get\n  operationId: getIssuedTicket\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /issued_tickets/{id}/void\n  method: post\n  operationId: voidIssuedTicket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vouchers\n  method: get\n  operationId: getAllVouchers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vouchers\n  method: post\n  operationId: createVoucher\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vouchers/{id}\n  method: get\n  operationId: getVoucher\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vouchers/{id}\n  method: put\n  operationId: updateVoucher\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vouchers/{id}\n  method: delete\n  operationId: deleteVoucher\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /voucher-codes\n  method: get\n  operationId: getVoucherCodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /check_ins\n  method: get\n  operationId: getCheckIns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /check_ins\n  method: post\n  operationId: createCheckIn\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tickettailor/refs/heads/main/agentic-access/tickettailor-agentic-access.yml
summary_line: 26 operations · 13 acting
tags:
- Event Ticketing
- Events
- Ticketing
- Box Office
- Payments
- Registration
---
