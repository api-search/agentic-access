---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 3
api_specs:
- filename: handlediq-com-booking-status-api-openapi.yml
  format: yaml
  label: handlediq-com Booking Status API
  slug: handlediq-com-booking-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/handlediq-com/openapi/handlediq-com-booking-status-api-openapi.yml
- filename: handlediq-com-cancel-booking-api-openapi.yml
  format: yaml
  label: handlediq-com Cancel Booking API
  slug: handlediq-com-cancel-booking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/handlediq-com/openapi/handlediq-com-cancel-booking-api-openapi.yml
- filename: handlediq-com-find-help-api-openapi.yml
  format: yaml
  label: handlediq-com Find Help API
  slug: handlediq-com-find-help-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/handlediq-com/openapi/handlediq-com-find-help-api-openapi.yml
- filename: handlediq-com-get-quote-api-openapi.yml
  format: yaml
  label: handlediq-com Get Quote API
  slug: handlediq-com-get-quote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/handlediq-com/openapi/handlediq-com-get-quote-api-openapi.yml
- filename: handlediq-com-hold-time-api-openapi.yml
  format: yaml
  label: handlediq-com Hold Time API
  slug: handlediq-com-hold-time-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/handlediq-com/openapi/handlediq-com-hold-time-api-openapi.yml
- filename: handlediq-com-move-booking-api-openapi.yml
  format: yaml
  label: handlediq-com Move Booking API
  slug: handlediq-com-move-booking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/handlediq-com/openapi/handlediq-com-move-booking-api-openapi.yml
- filename: handlediq-com-request-service-api-openapi.yml
  format: yaml
  label: handlediq-com Request Service API
  slug: handlediq-com-request-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/handlediq-com/openapi/handlediq-com-request-service-api-openapi.yml
- filename: handlediq-com-verify-record-api-openapi.yml
  format: yaml
  label: handlediq-com Verify Record API
  slug: handlediq-com-verify-record-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/handlediq-com/openapi/handlediq-com-verify-record-api-openapi.yml
consequence_counts:
  read: 3
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Handlediq Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'handlediq-com exposes 8 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: handlediq-com
provider_slug: handlediq-com
slug: handlediq-com-agentic-access
source_filename: handlediq-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/handlediq-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 3\n    acting: 5\n  by_consequence:\n    read: 3\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /api/find_help\n  method: post\n  operationId: find_help\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/hold_time\n  method: post\n  operationId: hold_time\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/booking_status\n  method: post\n  operationId: booking_status\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/move_booking\n  method: post\n  operationId: move_booking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/cancel_booking\n  method: post\n  operationId: cancel_booking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/request_service\n  method: post\n  operationId: request_service\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/get_quote\n  method: post\n  operationId: get_quote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/verify_record\n  method: post\n  operationId: verify_record\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/handlediq-com/agentic-access/handlediq-com-agentic-access.yml
summary_line: 8 operations · 5 acting
tags:
- Field Service Management
- Software-as-a-Service
- Home Services
- Scheduling
- Payments
- Artificial Intelligence
---
