---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 16
api_specs:
- filename: freighthub-com-booking-request-api-openapi.yml
  format: yaml
  label: Forto Booking Request API
  slug: freighthub-com-booking-request-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freighthub-com/openapi/freighthub-com-booking-request-api-openapi.yml
- filename: freighthub-com-reports-api-openapi.yml
  format: yaml
  label: Forto Reports API
  slug: freighthub-com-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freighthub-com/openapi/freighthub-com-reports-api-openapi.yml
- filename: freighthub-com-shipment-api-openapi.yml
  format: yaml
  label: Forto Shipment API
  slug: freighthub-com-shipment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freighthub-com/openapi/freighthub-com-shipment-api-openapi.yml
- filename: freighthub-com-subscriptions-api-openapi.yml
  format: yaml
  label: Forto Subscriptions API
  slug: freighthub-com-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freighthub-com/openapi/freighthub-com-subscriptions-api-openapi.yml
- filename: freighthub-com-tokens-api-openapi.yml
  format: yaml
  label: Forto Tokens API
  slug: freighthub-com-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freighthub-com/openapi/freighthub-com-tokens-api-openapi.yml
consequence_counts:
  physical: 1
  read: 16
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Freighthub Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/shipments/{shipmentId}/documents/{role}/upload
operation_count: 25
overview: 'Forto exposes 25 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read, 8 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Forto
provider_slug: freighthub-com
slug: freighthub-com-agentic-access
source_filename: freighthub-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: generated\nsource: openapi/freighthub-com-forto-platform-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    connected: 16\n    acting: 9\n  by_consequence:\n    read: 16\n    write: 8\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /shipments/{shipmentId}/transportPlan\n  method: get\n  operationId: getShipmentTransportPlan[0]\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/booking-requests\n  method: get\n  operationId: listv1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/booking-requests\n  method: post\n  operationId: createv1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/booking-requests/{id}\n  method: get\n  operationId: getv1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/booking-requests/{id}/discard\n  method: put\n  operationId: discardv1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/booking-requests/{id}/finalize\n\
  \  method: put\n  operationId: finalizev1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/booking-requests/{id}/update-details\n  method: put\n  operationId: updateDetailsv1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/events-api/inbox/{id}\n  method: get\n  operationId: getInboxv1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/events-api/subscriptions\n  method: get\n  operationId: listSubscriptionsv1\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/events-api/subscriptions\n  method: post\n  operationId: createSubscriptionv1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/events-api/subscriptions/{id}\n  method: delete\n  operationId: deleteSubscriptionv1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/reports/{templateId}/{reportId}\n  method: get\n  operationId: downloadReportv1\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/shipments\n  method: get\n  operationId: getShipmentsv1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/shipments/{shipmentId}\n  method: get\n  operationId: getShipmentv1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/shipments/{shipmentId}/documents\n  method: get\n  operationId: getShipmentDocumentsv1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/shipments/{shipmentId}/documents/{role}/upload\n  method: post\n  operationId: uploadShipmentDocumentv1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/shipments/{shipmentId}/invoices\n  method: get\n  operationId: getShipmentInvoicesv1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/shipments/{shipmentId}/transportPlan\n  method: get\n  operationId: getShipmentTransportPlan[1]v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tokens\n  method: post\n  operationId: createTokenv1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tokens\n  method: get\n  operationId: getTokensv1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tokens/{id}\n  method: delete\n  operationId: deleteTokenv1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/shipments/{shipmentId}/transportPlan\n  method: get\n  operationId: getShipmentTransportPlanv2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/shipments/{shipmentId}/transportPlan/events\n  method: get\n  operationId: getShipmentTransportPlanEventsv2\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/shipments/{shipmentId}/transportPlan/{referenceNumber}\n  method: get\n  operationId: getShipmentTransportPlanForContainerv2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/shipments/{shipmentId}/transportPlan/{referenceNumber}/events\n  method: get\n  operationId: getShipmentTransportPlanEventsForContainerv2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/freighthub-com/agentic-access/freighthub-com-agentic-access.yml
summary_line: 25 operations · 9 acting
tags:
- Ocean Freight
- Air Freight
- Rail Freight
- Logistics
- Sustainability
- Artificial Intelligence
- Platform
---
