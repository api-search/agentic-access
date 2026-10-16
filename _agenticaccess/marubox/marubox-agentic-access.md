---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 7
api_specs:
- filename: marubox-account-api-openapi.yml
  format: yaml
  label: Business Box Account API
  slug: marubox-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marubox/refs/heads/main/openapi/marubox-account-api-openapi.yml
- filename: marubox-bookings-api-openapi.yml
  format: yaml
  label: Business Box Bookings API
  slug: marubox-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marubox/refs/heads/main/openapi/marubox-bookings-api-openapi.yml
- filename: marubox-event-types-api-openapi.yml
  format: yaml
  label: Business Box Event types API
  slug: marubox-event-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marubox/refs/heads/main/openapi/marubox-event-types-api-openapi.yml
- filename: marubox-invites-api-openapi.yml
  format: yaml
  label: Business Box Invites API
  slug: marubox-invites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marubox/refs/heads/main/openapi/marubox-invites-api-openapi.yml
- filename: marubox-webhooks-api-openapi.yml
  format: yaml
  label: Business Box Webhooks API
  slug: marubox-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marubox/refs/heads/main/openapi/marubox-webhooks-api-openapi.yml
consequence_counts:
  read: 7
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Marubox Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Business Box exposes 12 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Business Box
provider_slug: marubox
slug: marubox-agentic-access
source_filename: marubox-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: generated\nsource: openapi/marubox-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 7\n    acting: 5\n  by_consequence:\n    read: 7\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /me\n  method: get\n  operationId: getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /event-types\n  method: get\n  operationId: listEventTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /event-types/{id}/slots\n  method: get\n  operationId:\
  \ listAvailableSlots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bookings\n  method: get\n  operationId: listBookings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bookings\n  method: post\n  operationId: createBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bookings/{id}\n  method: get\n  operationId: getBooking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bookings/{id}/cancel\n  method: post\n  operationId: cancelBooking\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invites\n  method: post\n  operationId: createInviteLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks\n  method: get\n \
  \ operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/{id}\n  method: get\n  operationId: getWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/{id}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marubox/refs/heads/main/agentic-access/marubox-agentic-access.yml
summary_line: 12 operations · 5 acting
tags:
- Company
- Booking
- Payments
- Calendar
- Japan
---
