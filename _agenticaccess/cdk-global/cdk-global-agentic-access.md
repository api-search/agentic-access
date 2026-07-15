---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 13
api_specs:
- filename: fortellis-appointments-openapi.yml
  format: yaml
  label: Fortellis Service Appointments API
  slug: fortellis-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdk-global/refs/heads/main/openapi/fortellis-appointments-openapi.yml
- filename: fortellis-user-service-openapi.yml
  format: yaml
  label: Fortellis User / Booking Sessions API
  slug: fortellis-user-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdk-global/refs/heads/main/openapi/fortellis-user-service-openapi.yml
- filename: fortellis-parts-store-openapi.yml
  format: yaml
  label: Fortellis Parts Store API
  slug: fortellis-parts-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdk-global/refs/heads/main/openapi/fortellis-parts-store-openapi.yml
- filename: fortellis-pet-adoption-openapi.yml
  format: yaml
  label: Fortellis Reference Pet Adoption API
  slug: fortellis-pet-adoption-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdk-global/refs/heads/main/openapi/fortellis-pet-adoption-openapi.yml
- filename: fortellis-event-relay-webhook-openapi.yml
  format: yaml
  label: Fortellis Event Relay Webhook
  slug: fortellis-event-relay-webhook
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdk-global/refs/heads/main/openapi/fortellis-event-relay-webhook-openapi.yml
- filename: fortellis-event-relay-data-plane-proxy-asyncapi.yml
  format: yaml
  label: Fortellis Event Relay Data Plane Proxy (AsyncAPI)
  slug: fortellis-event-relay-data-plane
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdk-global/refs/heads/main/asyncapi/fortellis-event-relay-data-plane-proxy-asyncapi.yml
- filename: fortellis-hello-world-asyncapi.yml
  format: yaml
  label: Fortellis AsyncAPI Hello World Reference
  slug: fortellis-async-hello-world
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdk-global/refs/heads/main/asyncapi/fortellis-hello-world-asyncapi.yml
consequence_counts:
  read: 13
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cdk Global Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 25
overview: 'CDK Global exposes 25 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read and 12 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CDK Global
provider_slug: cdk-global
slug: cdk-global-agentic-access
source_filename: cdk-global-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/fortellis-appointments-openapi.yml, openapi/fortellis-event-relay-webhook-openapi.yml,\n  openapi/fortellis-parts-store-openapi.yml, openapi/fortellis-pet-adoption-openapi.yml, openapi/fortellis-user-service-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    connected: 13\n    acting: 12\n  by_consequence:\n    read: 13\n    write: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: queryAppointments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - anonymous\n- path: /\n  method: post\n  operationId:\
  \ createAppointment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - anonymous\n- path: /{appointmentId}\n  method: get\n  operationId: queryAppointment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - anonymous\n- path: /{appointmentId}\n  method: post\n  operationId: updateAppointment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - anonymous\n- path: /{appointmentId}\n  method: delete\n\
  \  operationId: cancelAppointment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - anonymous\n- path: /event/{channel}\n  method: post\n  operationId: postEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /all-product-info\n  method: get\n  operationId: allProductInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - anonymous\n- path: /all-product-info/{productNumber}\n  method: get\n  operationId:\
  \ productInformation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - anonymous\n- path: /all-product-info/{productNumber}/product-size\n  method: get\n  operationId: productDescription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - anonymous\n- path: /ping\n  method: get\n  operationId: healthMonitor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - anonymous\n- path: /pets\n  method: get\n  operationId: queryPets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - anonymous\n- path: /pets\n  method: post\n  operationId: addPet\n \
  \ x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - anonymous\n- path: /pets/{petId}\n  method: get\n  operationId: readPets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - anonymous\n- path: /pets/{petId}\n  method: post\n  operationId: updatePets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - anonymous\n- path: /pets/{petId}\n  method: delete\n  operationId: deletePets\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - anonymous\n- path: /booking-sessions\n  method: post\n  operationId: createBookingSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - anonymous\n- path: /booking-sessions/{bookingSessionId}/items\n  method: post\n  operationId: addBookingSessionItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n    scope:\n    - anonymous\n- path: /booking-sessions/{bookingSessionId}/items\n  method: get\n  operationId: queryBookingSessionItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - anonymous\n- path: /booking-sessions/{bookingSessionId}/items/{itemId}\n  method: post\n  operationId: updateBookingSessionItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - anonymous\n- path: /booking-sessions/{bookingSessionId}/items/{itemId}\n  method: get\n  operationId: queryRequestedServiceItemById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - anonymous\n- path: /booking-sessions/{bookingSessionId}/items/{itemId}\n  method: delete\n  operationId: removeBookingSessionItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - anonymous\n- path: /booking-sessions/{bookingSessionId}/available-stores\n  method: get\n  operationId: queryBookingSessionStoreAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - anonymous\n- path: /booking-sessions/{bookingSessionId}/available-stores/{storeId}/slots\n  method: get\n  operationId: queryBookingSessionsAvailableStoreSlots\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - anonymous\n- path: /booking-sessions/{bookingSessionId}/available-stores/{storeId}/slots/{slotId}\n  method: get\n  operationId: queryBookingSessionsAvailableSlot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - anonymous\n- path: /booking-sessions/{bookingSessionId}/available-stores/{storeId}/slots/{slotId}\n  method: post\n  operationId: bookAppointmentSlot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - anonymous\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cdk-global/refs/heads/main/agentic-access/cdk-global-agentic-access.yml
summary_line: 25 operations · 12 acting
tags:
- Automotive
- Dealer Management
- DMS
- Auto Retail
- F&I
- Fixed Operations
- Parts
- CRM
- Digital Retail
- Marketplace
- Developer Platform
- Events
- Webhooks
- AsyncAPI
---
