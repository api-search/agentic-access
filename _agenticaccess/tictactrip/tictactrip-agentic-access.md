---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 14
api_specs:
- filename: tictactrip-openapi-original.json
  format: json
  label: Tictactrip API
  slug: tictactrip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tictactrip/refs/heads/main/openapi/tictactrip-openapi-original.json
consequence_counts:
  physical: 3
  read: 14
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tictactrip Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /booking/v3/orderTickets/{orderTicketId}/cancellation
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /booking/v3/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /booking/v3/orders/{orderId}/book
operation_count: 20
overview: 'TicTacTrip exposes 20 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read, 3 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: TicTacTrip
provider_slug: tictactrip
slug: tictactrip-agentic-access
source_filename: tictactrip-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/tictactrip-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    connected: 14\n    acting: 6\n  by_consequence:\n    read: 14\n    write: 3\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/segmentProviders\n  method: get\n  operationId: GetSegmentProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - admin\n    - bookPartner\n    - searchPartner\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/stopGroups\n  method: get\n  operationId: GetAllStopGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    scope:\n    - admin\n    - bookPartner\n    - searchPartner\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/stopGroups/{stopGroupGpuid}\n  method: get\n  operationId: GetStopGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - admin\n    - bookPartner\n    - searchPartner\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/stopClusters\n  method: get\n  operationId: GetAllStopClusters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - admin\n    - bookPartner\n    - searchPartner\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/stopClusters/{stopClusterGpuid}\n  method: get\n  operationId: GetStopCluster\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - admin\n    - bookPartner\n    - searchPartner\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v2/autocomplete\n  method: get\n  operationId: GetAutocomplete\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - admin\n    - bookPartner\n    - searchPartner\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/cities/popular/{limit}\n  method: get\n  operationId: GetPopularCities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - admin\n    - bookPartner\n    - searchPartner\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/cities/popular/{direction}/{uniqueName}/{limit}\n  method: get\n  operationId: GetPopularCitiesFromTo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - admin\n    - bookPartner\n    - searchPartner\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/results\n  method: post\n  operationId: GetResults\n  x-agentic-access:\n \
  \   action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - admin\n    - bookPartner\n    - searchPartner\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /booking/v3/carts/{cartId}\n  method: get\n  operationId: GetCart\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - admin\n    - bookPartner\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /booking/v3/carts/{cartId}\n  method: patch\n  operationId: UpdateCart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - admin\n    - bookPartner\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /booking/v3/carts\n\
  \  method: post\n  operationId: CreateCart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - admin\n    - bookPartner\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /booking/v3/orders\n  method: get\n  operationId: GetOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - admin\n    - bookPartner\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /booking/v3/orders\n  method: post\n  operationId: CreateOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - admin\n    - bookPartner\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n   \
  \   triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /booking/v3/orders/{orderId}\n  method: get\n  operationId: GetOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - admin\n    - bookPartner\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /booking/v3/discountCards\n  method: get\n  operationId: GetDiscountCards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /booking/v3/orders/{orderId}/book\n  method: post\n  operationId: CreateBook\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - admin\n    - bookPartner\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /booking/v3/orders/{orderId}/ticket\n  method: get\n  operationId: DownloadTicket\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - admin\n    - bookPartner\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /booking/v3/orderTickets/{orderTicketId}/cancellation/conditions\n  method: get\n  operationId: PartnerCancellationConditions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - admin\n    - bookPartner\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /booking/v3/orderTickets/{orderTicketId}/cancellation\n  method: put\n  operationId: PartnerCancelBooking\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - admin\n    - bookPartner\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tictactrip/refs/heads/main/agentic-access/tictactrip-agentic-access.yml
summary_line: 20 operations · 6 acting
tags:
- Company
- Travel
- Transportation
- Trains
- Buses
- Booking
- Mobility
- Multimodal
- Ticketing
---
