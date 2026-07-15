---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 1
api_specs:
- filename: cover-genius-openapi.yml
  format: yaml
  label: XCover Offers API
  slug: xcover-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cover-genius/refs/heads/main/openapi/cover-genius-openapi.yml
- filename: cover-genius-openapi.yml
  format: yaml
  label: XCover Bookings and Policies API
  slug: xcover-bookings-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cover-genius/refs/heads/main/openapi/cover-genius-openapi.yml
- filename: cover-genius-openapi.yml
  format: yaml
  label: XClaim Claims API
  slug: xclaim-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cover-genius/refs/heads/main/openapi/cover-genius-openapi.yml
consequence_counts:
  read: 1
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cover Genius Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Cover Genius exposes 8 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cover Genius
provider_slug: cover-genius
slug: cover-genius-agentic-access
source_filename: cover-genius-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/cover-genius-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 7\n    connected: 1\n  by_consequence:\n    write: 7\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /partners/{partner_code}/offers/\n  method: post\n  operationId: createOffer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partners/{partner_code}/offers/{offer_id}/opt_out/\n  method: post\n  operationId: optOutOffer\n \
  \ x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partners/{partner_code}/offers/{offer_id}/confirm/\n  method: post\n  operationId: confirmOffer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partners/{partner_code}/bookings/{booking_id}/\n  method: get\n  operationId: getBooking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /partners/{partner_code}/bookings/{booking_id}/\n  method: patch\n  operationId: modifyBooking\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partners/{partner_code}/bookings/{booking_id}/quote_for_update\n  method: patch\n  operationId: quoteForUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partners/{partner_code}/bookings/{booking_id}/confirm_update/{update_id}/\n  method: post\n  operationId: confirmBookingUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partners/{partner_code}/bookings/{booking_id}/cancel\n  method: post\n  operationId: cancelBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cover-genius/refs/heads/main/agentic-access/cover-genius-agentic-access.yml
summary_line: 8 operations · 7 acting
tags:
- Insurance
- Insurtech
- Embedded Insurance
- Protection
- Claims
---
