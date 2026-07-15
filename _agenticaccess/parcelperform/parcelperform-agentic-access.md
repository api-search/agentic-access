---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 6
api_specs:
- filename: parcelperform-openapi.yml
  format: yaml
  label: Parcel Perform Shipments API
  slug: parcelperform-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parcelperform/refs/heads/main/openapi/parcelperform-openapi.yml
- filename: parcelperform-openapi.yml
  format: yaml
  label: Parcel Perform Tracking Events API
  slug: parcelperform-tracking-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parcelperform/refs/heads/main/openapi/parcelperform-openapi.yml
- filename: parcelperform-openapi.yml
  format: yaml
  label: Parcel Perform Returns API
  slug: parcelperform-returns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parcelperform/refs/heads/main/openapi/parcelperform-openapi.yml
- filename: parcelperform-openapi.yml
  format: yaml
  label: Parcel Perform Webhooks API
  slug: parcelperform-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parcelperform/refs/heads/main/openapi/parcelperform-openapi.yml
- filename: parcelperform-openapi.yml
  format: yaml
  label: Parcel Perform Couriers API
  slug: parcelperform-couriers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parcelperform/refs/heads/main/openapi/parcelperform-openapi.yml
- filename: parcelperform-openapi.yml
  format: yaml
  label: Parcel Perform Analytics API
  slug: parcelperform-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parcelperform/refs/heads/main/openapi/parcelperform-openapi.yml
consequence_counts:
  physical: 4
  read: 6
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Parcelperform Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /return/shipment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /shipment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /shipment/details/{tracking_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /shipment/{tracking_id}/event
operation_count: 13
overview: 'Parcel Perform exposes 13 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 3 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Parcel Perform
provider_slug: parcelperform
slug: parcelperform-agentic-access
source_filename: parcelperform-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/parcelperform-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    acting: 7\n    connected: 6\n  by_consequence:\n    write: 3\n    physical: 4\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /auth/oauth/token/\n  method: post\n  operationId: createAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shipment\n  method: post\n  operationId: createShipment\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shipment/list\n  method: get\n  operationId: listShipments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shipment/details/{tracking_id}\n  method: get\n  operationId: getShipmentDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shipment/details/{tracking_id}\n  method: put\n  operationId: updateShipment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n\
  \      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shipment/{tracking_id}/event\n  method: post\n  operationId: createShipmentEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /return\n  method: post\n  operationId: createReturn\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /return/shipment\n  method: post\n  operationId: createReturnWithShipment\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook\n  method: get\n  operationId: listWebhookSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook\n  method: post\n  operationId: createWebhookSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /courier\n  method: get\n  operationId: listCouriers\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /courier/{courier_code}\n  method: get\n  operationId: getCourier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/performance\n  method: get\n  operationId: getPerformanceAnalytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parcelperform/refs/heads/main/agentic-access/parcelperform-agentic-access.yml
summary_line: 13 operations · 7 acting
tags:
- Logistics
- Shipment Tracking
- Post-Purchase
- Delivery Experience
- Returns
- E-Commerce
---
