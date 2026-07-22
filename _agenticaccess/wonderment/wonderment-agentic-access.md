---
acting_count: 0
action_class_counts:
  connected: 4
api_specs:
- filename: wonderment-openapi.json
  format: json
  label: Wonderment API
  slug: wonderment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wonderment/refs/heads/main/openapi/wonderment-openapi.json
consequence_counts:
  read: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Wonderment Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'Wonderment exposes 4 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Wonderment
provider_slug: wonderment
slug: wonderment-agentic-access
source_filename: wonderment-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/wonderment-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    connected: 4\n  by_consequence:\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /2022-10/shipments/search/{searchTerm}\n  method: get\n  operationId: searchShipments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2022-10/reports\n  method: get\n  operationId: listReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/shipment/report/download/{path}\n\
  \  method: get\n  operationId: downloadReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /predictions\n  method: get\n  operationId: getDeliveryPredictions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wonderment/refs/heads/main/agentic-access/wonderment-agentic-access.yml
summary_line: 4 operations
tags:
- Company
- Ecommerce
- Order Tracking
- Post-Purchase
- Shipping
- Logistics
- Shopify
- Webhooks
---
