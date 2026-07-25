---
acting_count: 0
action_class_counts:
  connected: 8
api_specs:
- filename: ripe-insurance-umbraco-content-delivery-openapi.json
  format: json
  label: Ripe Insurance Umbraco Content Delivery API
  slug: ripe-insurance-umbraco-content-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ripe-insurance/refs/heads/main/openapi/ripe-insurance-umbraco-content-delivery-openapi.json
- filename: ripe-insurance-cycleplan-content-delivery-openapi.json
  format: json
  label: Cycleplan Umbraco Content Delivery API
  slug: ripe-insurance-cycleplan-content-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ripe-insurance/refs/heads/main/openapi/ripe-insurance-cycleplan-content-delivery-openapi.json
consequence_counts:
  read: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ripe Insurance Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Ripe Insurance exposes 8 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Ripe Insurance
provider_slug: ripe-insurance
slug: ripe-insurance-agentic-access
source_filename: ripe-insurance-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: generated\nsource: openapi/ripe-insurance-umbraco-content-delivery-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 8\n  by_consequence:\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /umbraco/delivery/api/v2/content\n  method: get\n  operationId: GetContent2.0\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /umbraco/delivery/api/v2/content/item/{path}\n  method: get\n  operationId: GetContentItemByPath2.0\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /umbraco/delivery/api/v2/content/item/{id}\n  method: get\n  operationId: GetContentItemById2.0\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /umbraco/delivery/api/v2/content/items\n  method: get\n  operationId: GetContentItems2.0\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /umbraco/delivery/api/v2/media\n  method: get\n  operationId: GetMedia2.0\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /umbraco/delivery/api/v2/media/item/{path}\n  method: get\n  operationId: GetMediaItemByPath2.0\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /umbraco/delivery/api/v2/media/item/{id}\n  method: get\n  operationId: GetMediaItemById2.0\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /umbraco/delivery/api/v2/media/items\n  method: get\n  operationId: GetMediaItems2.0\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ripe-insurance/refs/heads/main/agentic-access/ripe-insurance-agentic-access.yml
summary_line: 8 operations
tags:
- Insurance
- United Kingdom
- Insurtech
- Managing General Agent
- Specialist Insurance
- Personal Lines
- Small Business Insurance
- Underwriting
- Direct to Consumer
- Broker
---
