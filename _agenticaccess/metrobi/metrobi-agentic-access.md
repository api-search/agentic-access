---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 2
api_specs:
- filename: metrobi-delivery-api-openapi.json
  format: json
  label: Metrobi Delivery API
  slug: metrobi-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metrobi/refs/heads/main/openapi/metrobi-delivery-api-openapi.json
consequence_counts:
  read: 2
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Metrobi Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Metrobi exposes 5 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Metrobi
provider_slug: metrobi
slug: metrobi-agentic-access
source_filename: metrobi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/metrobi-delivery-api-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    acting: 3\n    connected: 2\n  by_consequence:\n    write: 3\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/delivery\n  method: post\n  operationId: create-a-delivery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/delivery\n  method: get\n  operationId: list-deliveries\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/delivery/{delivery_id}\n  method: get\n  operationId: get-a-delivery-status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/delivery/{delivery_id}\n  method: delete\n  operationId: cancel-a-delivery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/delivery_estimate\n  method: post\n  operationId: delivery-estimation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n \
  \     - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metrobi/refs/heads/main/agentic-access/metrobi-agentic-access.yml
summary_line: 5 operations · 3 acting
tags:
- Company
- Delivery
- Logistics
- Courier
- Last Mile Delivery
- Route Optimization
- Fulfillment
- Local Delivery
- Webhooks
---
