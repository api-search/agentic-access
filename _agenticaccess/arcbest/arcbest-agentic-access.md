---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 6
api_specs:
- filename: arcbest-pickups-api-openapi.yml
  format: yaml
  label: ArcBest Pickups API
  slug: arcbest-pickups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcbest/refs/heads/main/openapi/arcbest-pickups-api-openapi.yml
- filename: arcbest-rates-api-openapi.yml
  format: yaml
  label: ArcBest Rates API
  slug: arcbest-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcbest/refs/heads/main/openapi/arcbest-rates-api-openapi.yml
- filename: arcbest-shipments-api-openapi.yml
  format: yaml
  label: ArcBest Shipments API
  slug: arcbest-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcbest/refs/heads/main/openapi/arcbest-shipments-api-openapi.yml
- filename: arcbest-tracking-api-openapi.yml
  format: yaml
  label: ArcBest Tracking API
  slug: arcbest-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcbest/refs/heads/main/openapi/arcbest-tracking-api-openapi.yml
- filename: arcbest-authorize-api-openapi.yml
  format: yaml
  label: ArcBest Authorize API
  slug: arcbest-authorize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcbest/refs/heads/main/openapi/arcbest-authorize-api-openapi.yml
- filename: arcbest-booking-api-openapi.yml
  format: yaml
  label: ArcBest Booking API
  slug: arcbest-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcbest/refs/heads/main/openapi/arcbest-booking-api-openapi.yml
- filename: arcbest-order-api-openapi.yml
  format: yaml
  label: ArcBest Order API
  slug: arcbest-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcbest/refs/heads/main/openapi/arcbest-order-api-openapi.yml
- filename: arcbest-quote-api-openapi.yml
  format: yaml
  label: ArcBest Quote API
  slug: arcbest-quote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcbest/refs/heads/main/openapi/arcbest-quote-api-openapi.yml
- filename: arcbest-quotes-api-openapi.yml
  format: yaml
  label: ArcBest Quotes API
  slug: arcbest-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcbest/refs/heads/main/openapi/arcbest-quotes-api-openapi.yml
consequence_counts:
  physical: 3
  read: 6
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Arcbest Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /order/refs/{arcbOrderNo}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /shipments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /shipments/search
operation_count: 17
overview: 'ArcBest exposes 17 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 8 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ArcBest
provider_slug: arcbest
slug: arcbest-agentic-access
source_filename: arcbest-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: generated\nsource: openapi/arcbest-authorize-api-openapi.yml, openapi/arcbest-booking-api-openapi.yml,\n  openapi/arcbest-order-api-openapi.yml, openapi/arcbest-pickups-api-openapi.yml, openapi/arcbest-quote-api-openapi.yml,\n  openapi/arcbest-quotes-api-openapi.yml, openapi/arcbest-rates-api-openapi.yml, openapi/arcbest-shipments-api-openapi.yml,\n  openapi/arcbest-tracking-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    acting: 11\n    connected: 6\n  by_consequence:\n    write: 8\n    read: 6\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /authorize\n  method: post\n  operationId: authorizePost\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /booking\n  method: put\n  operationId: bookingCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /booking/status\n  method: get\n  operationId: bookingGetStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /order/bol/{expediteOrderNo}\n  method: get\n  operationId: orderBol\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /order/refs/{arcbOrderNo}\n  method: post\n  operationId: orderUpdateRefs\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pickups\n  method: post\n  operationId: schedulePickup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /quote\n  method: post\n  operationId: quoteCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n   \
  \   human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /quotes\n  method: post\n  operationId: quotesSubmitQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /quotes/booking-request/expedite\n  method: post\n  operationId: quotesBookExpediteQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /quotes/booking-request/time-critical-forwarding\n  method: post\n  operationId: quotesBookTimeCriticalForwardingQuote\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /quotes/booking-request/status\n  method: get\n  operationId: quotesGetBookingStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rates/ltl\n  method: post\n  operationId: getLTLRate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shipments\n  method: post\n  operationId: createShipment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shipments\n  method: get\n  operationId: listShipments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shipments/status-codes\n  method: get\n  operationId: shipmentsGetShipmentStatusCodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shipments/search\n  method: post\n  operationId: shipmentsGetShipmentsByReferenceNumbers\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tracking/{proNumber}\n  method: get\n  operationId: trackShipment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arcbest/refs/heads/main/agentic-access/arcbest-agentic-access.yml
summary_line: 17 operations · 11 acting
tags:
- Logistics
- Freight
- LTL
- Supply Chain
- Shipping
- Transportation
- Expedite
- Truckload
- EDI
- Bill of Lading
- Rate Quote
- Shipment Tracking
---
