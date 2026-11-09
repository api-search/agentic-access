---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 9
api_specs:
- filename: evergreen-marine-an-publisher-endpoints-api-openapi.yml
  format: yaml
  label: Evergreen Marine Corp. AN Publisher Endpoints API
  slug: evergreen-marine-an-publisher-endpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evergreen-marine/openapi/evergreen-marine-an-publisher-endpoints-api-openapi.yml
- filename: evergreen-marine-an-subscriber-endpoints-api-openapi.yml
  format: yaml
  label: Evergreen Marine Corp. AN Subscriber Endpoints API
  slug: evergreen-marine-an-subscriber-endpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evergreen-marine/openapi/evergreen-marine-an-subscriber-endpoints-api-openapi.yml
- filename: evergreen-marine-booking-api-openapi.yml
  format: yaml
  label: Evergreen Marine Corp. Booking API
  slug: evergreen-marine-booking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evergreen-marine/openapi/evergreen-marine-booking-api-openapi.yml
- filename: evergreen-marine-events-api-openapi.yml
  format: yaml
  label: Evergreen Marine Corp. Events API
  slug: evergreen-marine-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evergreen-marine/openapi/evergreen-marine-events-api-openapi.yml
- filename: evergreen-marine-issuance-response-api-openapi.yml
  format: yaml
  label: Evergreen Marine Corp. Issuance Response API
  slug: evergreen-marine-issuance-response-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evergreen-marine/openapi/evergreen-marine-issuance-response-api-openapi.yml
- filename: evergreen-marine-notifications-api-openapi.yml
  format: yaml
  label: Evergreen Marine Corp. Notifications API
  slug: evergreen-marine-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evergreen-marine/openapi/evergreen-marine-notifications-api-openapi.yml
- filename: evergreen-marine-point-to-point-api-openapi.yml
  format: yaml
  label: Evergreen Marine Corp. Point To Point API
  slug: evergreen-marine-point-to-point-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evergreen-marine/openapi/evergreen-marine-point-to-point-api-openapi.yml
- filename: evergreen-marine-port-schedule-api-openapi.yml
  format: yaml
  label: Evergreen Marine Corp. Port Schedule API
  slug: evergreen-marine-port-schedule-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evergreen-marine/openapi/evergreen-marine-port-schedule-api-openapi.yml
- filename: evergreen-marine-shipping-instructions-api-openapi.yml
  format: yaml
  label: Evergreen Marine Corp. Shipping Instructions API
  slug: evergreen-marine-shipping-instructions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evergreen-marine/openapi/evergreen-marine-shipping-instructions-api-openapi.yml
- filename: evergreen-marine-subscriptions-api-openapi.yml
  format: yaml
  label: Evergreen Marine Corp. Subscriptions API
  slug: evergreen-marine-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evergreen-marine/openapi/evergreen-marine-subscriptions-api-openapi.yml
- filename: evergreen-marine-surrender-requests-api-openapi.yml
  format: yaml
  label: Evergreen Marine Corp. Surrender Requests API
  slug: evergreen-marine-surrender-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evergreen-marine/openapi/evergreen-marine-surrender-requests-api-openapi.yml
- filename: evergreen-marine-transport-document-api-openapi.yml
  format: yaml
  label: Evergreen Marine Corp. Transport Document API
  slug: evergreen-marine-transport-document-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evergreen-marine/openapi/evergreen-marine-transport-document-api-openapi.yml
- filename: evergreen-marine-vessel-schedule-api-openapi.yml
  format: yaml
  label: Evergreen Marine Corp. Vessel Schedule API
  slug: evergreen-marine-vessel-schedule-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evergreen-marine/openapi/evergreen-marine-vessel-schedule-api-openapi.yml
consequence_counts:
  physical: 5
  read: 9
  safety-critical: 1
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Evergreen Marine Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /tnt/v2/event-subscriptions/{subscriptionID}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /arrival-notice-notifications
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /arrival-notices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /booking-notifications
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/shipping-instructions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v3/shipping-instructions/{documentReference}
operation_count: 22
overview: 'Evergreen Marine Corp. exposes 22 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 7 write, 5 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Evergreen Marine Corp.
provider_slug: evergreen-marine
slug: evergreen-marine-agentic-access
source_filename: evergreen-marine-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: generated\nsource: openapi/evergreen-marine-arrival-notice-openapi.yml, openapi/evergreen-marine-booking-openapi.yml,\n  openapi/evergreen-marine-commercial-schedules-openapi.yml, openapi/evergreen-marine-ebl-issuance-openapi.yml,\n  openapi/evergreen-marine-ebl-surrender-openapi.yml, openapi/evergreen-marine-shipping-instructions-openapi.yml,\n  openapi/evergreen-marine-track-and-trace-openapi.yml, openapi/evergreen-marine-transport-document-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 9\n    acting: 13\n  by_consequence:\n    read: 9\n    physical: 5\n    write: 7\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /arrival-notices\n\
  \  method: get\n  operationId: get-arrival-notices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /arrival-notices\n  method: post\n  operationId: post-arrival-notices\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /arrival-notice-notifications\n  method: post\n  operationId: post-arrival-notice-notifications\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /dcsa/bookings\n  method: post\n  operationId: create-bookings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dcsa/bookings/{bookingReference}\n  method: get\n  operationId: get-bookings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dcsa/bookings/{bookingReference}\n  method: put\n  operationId: update-bookings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dcsa/bookings/{bookingReference}\n\
  \  method: patch\n  operationId: cancel-booking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /booking-notifications\n  method: post\n  operationId: booking-notifications\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /server/sol/route/commercial/v1/point-to-point-routes\n  method: get\n  operationId: get-v1-point-to-point\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /server/sol/mvs1api/commSch/v1/port\n  method: get\n  operationId: get-v1-port-schedules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /server/sol/mvs1api/commSch/v1/vessel\n  method: get\n  operationId: get-v1-vessel-schedule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/ebl-issuance-responses\n  method: post\n  operationId: create-ebl-issuance-response\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/ebl-surrender-requests\n  method: post\n  operationId: create-surrender-request\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/shipping-instructions\n  method: post\n  operationId: create-shipping-instructions\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/shipping-instructions/{documentReference}\n  method: put\n  operationId: update-shipping-instructions\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tnt/v2/event-subscriptions\n  method: get\n  operationId: subscriptionsGetUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tnt/v2/event-subscriptions/{subscriptionID}\n  method: get\n  operationId: subscriptionsGetIDUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tnt/v2/event-subscriptions/{subscriptionID}\n  method: put\n  operationId: subscriptionsPutIDUsingPUT\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /tnt/v2/event-subscriptions/{subscriptionID}\n  method: delete\n  operationId: subscriptionsDeleteIDUsingDELETE\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /tnt/v2/events\n  method: get\n  operationId: eventGetUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/transport-documents/{transportDocumentReference}\n  method: get\n  operationId: get-transport-document\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/transport-documents/{transportDocumentReference}\n  method: patch\n  operationId:\
  \ approve-transport-document\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/evergreen-marine/agentic-access/evergreen-marine-agentic-access.yml
summary_line: 22 operations · 13 acting · 1 human-in-the-loop
tags:
- Company
- Container Shipping
- Logistics
- Maritime
- Shipping
- Supply Chain
- Track and Trace
- Taiwan
---
