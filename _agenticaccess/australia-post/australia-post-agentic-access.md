---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 8
api_specs:
- filename: locations-openapi.json
  format: json
  label: Australia Post Locations API
  slug: locations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australia-post/refs/heads/main/openapi/locations-openapi.json
- filename: delivery-partner-openapi.json
  format: json
  label: Australia Post Delivery Partner API
  slug: delivery-partner
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australia-post/refs/heads/main/openapi/delivery-partner-openapi.json
consequence_counts:
  physical: 1
  read: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Australia Post Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/event
operation_count: 9
overview: 'Australia Post exposes 9 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Australia Post
provider_slug: australia-post
slug: australia-post-agentic-access
source_filename: australia-post-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/delivery-partner-openapi.json, openapi/locations-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    acting: 1\n    connected: 8\n  by_consequence:\n    physical: 1\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/event\n  method: post\n  operationId: event\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /points/postcode/{postcode}\n\
  \  method: get\n  operationId: getGeoLocationsByPostCodeUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /points/workcentres/{work_centre_id}\n  method: get\n  operationId: getGeoLocationsByWcidUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /points/deliverypoints/{delivery_point_id}\n  method: get\n  operationId: getGeoLocationsByDeliveryPointIdUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /points/{location_code}\n  method: get\n  operationId: getPointsByLocationCodeUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /points/type/{points_type}\n\
  \  method: get\n  operationId: getPointsByTypeUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /points/geo/{longitude}/{latitude}\n  method: get\n  operationId: getGeoLocationsUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services\n  method: get\n  operationId: getServicesUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/{service_codes}\n  method: get\n  operationId: getServicesByServiceCodesUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/australia-post/refs/heads/main/agentic-access/australia-post-agentic-access.yml
summary_line: 9 operations · 1 acting
tags:
- Address Validation
- Click and Collect
- Delivery
- E-Commerce
- Labels
- Locations
- Logistics
- Parcel Locker
- Postal
- Postage
- Shipping
- Tracking
---
