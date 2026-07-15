---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 2
api_specs:
- filename: chowly-openapi.yml
  format: yaml
  label: Chowly Orders API
  slug: orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chowly/refs/heads/main/openapi/chowly-openapi.yml
- filename: chowly-openapi.yml
  format: yaml
  label: Chowly Menu Sync API
  slug: menu-sync
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chowly/refs/heads/main/openapi/chowly-openapi.yml
- filename: chowly-openapi.yml
  format: yaml
  label: Chowly Stores API
  slug: stores
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chowly/refs/heads/main/openapi/chowly-openapi.yml
consequence_counts:
  physical: 1
  read: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Chowly Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders
operation_count: 3
overview: 'Chowly exposes 3 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Chowly
provider_slug: chowly
slug: chowly-agentic-access
source_filename: chowly-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/chowly-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 3\n  by_action_class:\n    acting: 1\n    connected: 2\n  by_consequence:\n    physical: 1\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /orders\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{orderId}\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /menu\n  method: get\n  operationId: getMenu\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chowly/refs/heads/main/agentic-access/chowly-agentic-access.yml
summary_line: 3 operations · 1 acting
tags:
- Restaurants
- Online Ordering
- Delivery
- POS Integration
- Menu Sync
---
