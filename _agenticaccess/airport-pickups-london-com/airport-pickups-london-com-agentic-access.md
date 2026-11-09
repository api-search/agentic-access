---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 2
api_specs:
- filename: airport-pickups-london-com-amend-booking-api-openapi.yml
  format: yaml
  label: Airport Pickups London Amend Booking API
  slug: airport-pickups-london-com-amend-booking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airport-pickups-london-com/openapi/airport-pickups-london-com-amend-booking-api-openapi.yml
- filename: airport-pickups-london-com-book-api-openapi.yml
  format: yaml
  label: Airport Pickups London Book API
  slug: airport-pickups-london-com-book-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airport-pickups-london-com/openapi/airport-pickups-london-com-book-api-openapi.yml
- filename: airport-pickups-london-com-cancel-booking-api-openapi.yml
  format: yaml
  label: Airport Pickups London Cancel Booking API
  slug: airport-pickups-london-com-cancel-booking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airport-pickups-london-com/openapi/airport-pickups-london-com-cancel-booking-api-openapi.yml
- filename: airport-pickups-london-com-lookup-booking-api-openapi.yml
  format: yaml
  label: Airport Pickups London Lookup Booking API
  slug: airport-pickups-london-com-lookup-booking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airport-pickups-london-com/openapi/airport-pickups-london-com-lookup-booking-api-openapi.yml
- filename: airport-pickups-london-com-quote-api-openapi.yml
  format: yaml
  label: Airport Pickups London Quote API
  slug: airport-pickups-london-com-quote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airport-pickups-london-com/openapi/airport-pickups-london-com-quote-api-openapi.yml
- filename: airport-pickups-london-com-track-api-openapi.yml
  format: yaml
  label: Airport Pickups London Track API
  slug: airport-pickups-london-com-track-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airport-pickups-london-com/openapi/airport-pickups-london-com-track-api-openapi.yml
- filename: airport-pickups-london-com-validate-flight-api-openapi.yml
  format: yaml
  label: Airport Pickups London Validate Flight API
  slug: airport-pickups-london-com-validate-flight-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airport-pickups-london-com/openapi/airport-pickups-london-com-validate-flight-api-openapi.yml
consequence_counts:
  physical: 4
  read: 2
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Airport Pickups London Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/book
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/book
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/quote
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/quote
operation_count: 14
overview: 'Airport Pickups London exposes 14 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read, 8 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Airport Pickups London
provider_slug: airport-pickups-london-com
slug: airport-pickups-london-com-agentic-access
source_filename: airport-pickups-london-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/airport-pickups-london-com-openapi.yml, openapi/mcp-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    acting: 12\n    connected: 2\n  by_consequence:\n    physical: 4\n    write: 8\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/quote\n  method: post\n  operationId: getTransferQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/validate-flight\n\
  \  method: post\n  operationId: validateFlight\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/book\n  method: post\n  operationId: createTransferBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/lookup-booking\n  method: post\n  operationId: lookupBooking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/amend-booking\n  method: post\n  operationId:\
  \ amendBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/cancel-booking\n  method: post\n  operationId: cancelBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/track\n  method: post\n  operationId: trackDriver\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/quote\n\
  \  method: post\n  operationId: getTransferQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/validate-flight\n  method: post\n  operationId: validateFlight\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/book\n  method: post\n  operationId: createTransferBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/lookup-booking\n  method: post\n  operationId: lookupBooking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/amend-booking\n  method: post\n  operationId: amendBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/cancel-booking\n  method: post\n  operationId: cancelBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/track\n  method: post\n  operationId: trackDriver\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/airport-pickups-london-com/agentic-access/airport-pickups-london-com-agentic-access.yml
summary_line: 14 operations · 12 acting
tags:
- Company
- Airport
- Transport
- Taxi
- London
---
