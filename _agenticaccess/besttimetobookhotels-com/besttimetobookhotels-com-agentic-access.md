---
acting_count: 0
action_class_counts:
  connected: 5
api_specs:
- filename: besttimetobookhotels-com-booking-timing-api-openapi.yml
  format: yaml
  label: Best Time To Book Hotels Booking Timing API
  slug: besttimetobookhotels-com-booking-timing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/besttimetobookhotels-com/openapi/besttimetobookhotels-com-booking-timing-api-openapi.yml
- filename: besttimetobookhotels-com-content-api-openapi.yml
  format: yaml
  label: Best Time To Book Hotels Content API
  slug: besttimetobookhotels-com-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/besttimetobookhotels-com/openapi/besttimetobookhotels-com-content-api-openapi.yml
- filename: besttimetobookhotels-com-deals-api-openapi.yml
  format: yaml
  label: Best Time To Book Hotels Deals API
  slug: besttimetobookhotels-com-deals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/besttimetobookhotels-com/openapi/besttimetobookhotels-com-deals-api-openapi.yml
- filename: besttimetobookhotels-com-operations-api-openapi.yml
  format: yaml
  label: Best Time To Book Hotels Operations API
  slug: besttimetobookhotels-com-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/besttimetobookhotels-com/openapi/besttimetobookhotels-com-operations-api-openapi.yml
consequence_counts:
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Besttimetobookhotels Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Best Time To Book Hotels exposes 5 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Best Time To Book Hotels
provider_slug: besttimetobookhotels-com
slug: besttimetobookhotels-com-agentic-access
source_filename: besttimetobookhotels-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/besttimetobookhotels-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 5\n  by_consequence:\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /api/booking-advice\n  method: get\n  operationId: getBookingAdvice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/hotel-booking-lead-time\n  method: get\n  operationId: exploreBookingLeadTime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/last-minute-deal-history\n\
  \  method: get\n  operationId: getLastMinuteDealHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent-markdown\n  method: get\n  operationId: renderPageMarkdown\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/besttimetobookhotels-com/agentic-access/besttimetobookhotels-com-agentic-access.yml
summary_line: 5 operations
tags:
- Travel
- Hotels
- Pricing
- Data
- Multilingual
---
