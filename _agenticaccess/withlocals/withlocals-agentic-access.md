---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 7
api_specs:
- filename: withlocals-availability-api-openapi.yml
  format: yaml
  label: Withlocals Availability API
  slug: withlocals-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withlocals/refs/heads/main/openapi/withlocals-availability-api-openapi.yml
- filename: withlocals-bookings-api-openapi.yml
  format: yaml
  label: Withlocals Bookings API
  slug: withlocals-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withlocals/refs/heads/main/openapi/withlocals-bookings-api-openapi.yml
- filename: withlocals-products-api-openapi.yml
  format: yaml
  label: Withlocals Products API
  slug: withlocals-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withlocals/refs/heads/main/openapi/withlocals-products-api-openapi.yml
- filename: withlocals-supplier-api-openapi.yml
  format: yaml
  label: Withlocals Supplier API
  slug: withlocals-supplier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withlocals/refs/heads/main/openapi/withlocals-supplier-api-openapi.yml
- filename: withlocals-webhooks-api-openapi.yml
  format: yaml
  label: Withlocals Webhooks API
  slug: withlocals-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withlocals/refs/heads/main/openapi/withlocals-webhooks-api-openapi.yml
consequence_counts:
  read: 7
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Withlocals Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Withlocals exposes 12 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Withlocals
provider_slug: withlocals
slug: withlocals-agentic-access
source_filename: withlocals-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: generated\nsource: openapi/withlocals-partner-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 7\n    acting: 5\n  by_consequence:\n    read: 7\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: getSupplier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products\n  method: get\n  operationId: listProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/{productId}\n  method: get\n  operationId:\
  \ getProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /availability/calendar\n  method: post\n  operationId: availabilityCalendar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bookings\n  method: get\n  operationId: listBookings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bookings\n  method: post\n  operationId: createBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bookings/{bookingId}\n  method: get\n  operationId:\
  \ getBooking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bookings/{bookingId}\n  method: patch\n  operationId: amendBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bookings/{bookingId}\n  method: delete\n  operationId: cancelBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks\n  method: get\n  operationId: getWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: put\n  operationId: setWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/withlocals/refs/heads/main/agentic-access/withlocals-agentic-access.yml
summary_line: 12 operations · 5 acting
tags:
- Company
- Travel
- Tours
- Experiences
- Tourism
- Marketplace
- Partner API
---
