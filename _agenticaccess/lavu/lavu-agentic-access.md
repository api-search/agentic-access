---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 1
api_specs:
- filename: lavu-menu-api-openapi.yml
  format: yaml
  label: Lavu Menu API
  slug: lavu-menu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lavu/refs/heads/main/openapi/lavu-menu-api-openapi.yml
- filename: lavu-orders-api-openapi.yml
  format: yaml
  label: Lavu Orders API
  slug: lavu-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lavu/refs/heads/main/openapi/lavu-orders-api-openapi.yml
consequence_counts:
  physical: 1
  read: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Lavu Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /insert
operation_count: 2
overview: 'Lavu exposes 2 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Lavu
provider_slug: lavu
slug: lavu-agentic-access
source_filename: lavu-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/lavu-menu-api-openapi.yml, openapi/lavu-orders-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 2\n  by_action_class:\n    connected: 1\n    acting: 1\n  by_consequence:\n    read: 1\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: post\n  operationId: queryTable\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insert\n  method: post\n  operationId: insertRecords\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n\
  \      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lavu/refs/heads/main/agentic-access/lavu-agentic-access.yml
summary_line: 2 operations · 1 acting
tags:
- Restaurant
- Point-of-Sale
- Payments
- Inventory
- Menu Management
---
