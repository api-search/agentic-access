---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 1
api_specs:
- filename: ratehawk-openapi.yml
  format: yaml
  label: RateHawk Hotel Search API
  slug: hotel-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ratehawk/refs/heads/main/openapi/ratehawk-openapi.yml
- filename: ratehawk-openapi.yml
  format: yaml
  label: RateHawk Hotel Page / Prebook API
  slug: hotel-page-prebook
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ratehawk/refs/heads/main/openapi/ratehawk-openapi.yml
- filename: ratehawk-openapi.yml
  format: yaml
  label: RateHawk Order Booking API
  slug: order-booking
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ratehawk/refs/heads/main/openapi/ratehawk-openapi.yml
- filename: ratehawk-openapi.yml
  format: yaml
  label: RateHawk Hotel Content / Static API
  slug: hotel-content-static
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ratehawk/refs/heads/main/openapi/ratehawk-openapi.yml
- filename: ratehawk-openapi.yml
  format: yaml
  label: RateHawk Webhooks
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ratehawk/refs/heads/main/openapi/ratehawk-openapi.yml
consequence_counts:
  physical: 5
  read: 1
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ratehawk Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /hotel/order/booking/finish/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /hotel/order/booking/finish/status/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /hotel/order/booking/form/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /hotel/order/cancel/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /hotel/order/info/
operation_count: 13
overview: 'RateHawk exposes 13 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read, 7 write, and 5 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: RateHawk
provider_slug: ratehawk
slug: ratehawk-agentic-access
source_filename: ratehawk-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/ratehawk-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 1\n    acting: 12\n  by_consequence:\n    read: 1\n    write: 7\n    physical: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /overview/\n  method: get\n  operationId: getOverview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/serp/region/\n  method: post\n  operationId: searchRegion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /search/serp/hotels/\n  method: post\n  operationId: searchHotels\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /search/serp/geo/\n  method: post\n  operationId: searchGeo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /search/hp/\n  method: post\n  operationId: searchHotelPage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hotel/prebook/\n  method: post\n  operationId: hotelPrebook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hotel/order/booking/form/\n  method: post\n  operationId: orderBookingForm\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hotel/order/booking/finish/\n  method: post\n  operationId: orderBookingFinish\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hotel/order/booking/finish/status/\n  method: post\n  operationId: orderBookingFinishStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hotel/order/info/\n  method: post\n  operationId: orderInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hotel/order/cancel/\n  method: post\n  operationId: orderCancel\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hotel/info/\n  method: post\n  operationId: hotelInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hotel/info/dump/\n  method: post\n  operationId: hotelInfoDump\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ratehawk/refs/heads/main/agentic-access/ratehawk-agentic-access.yml
summary_line: 13 operations · 12 acting
tags:
- Travel
- Hotels
- Booking
- B2B
- Reservations
---
