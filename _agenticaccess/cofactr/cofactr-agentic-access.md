---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 3
api_specs:
- filename: cofactr-knowledge-graph-openapi-original.json
  format: json
  label: Cofactr Knowledge Graph (Component Cloud) API
  slug: cofactr-knowledge-graph-component-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cofactr/refs/heads/main/openapi/cofactr-knowledge-graph-openapi-original.json
consequence_counts:
  read: 3
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cofactr Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'Cofactr exposes 4 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cofactr
provider_slug: cofactr
slug: cofactr-agentic-access
source_filename: cofactr-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/cofactr-knowledge-graph-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    connected: 3\n    acting: 1\n  by_consequence:\n    read: 3\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /products/\n  method: get\n  operationId: listProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/{id}\n  method: get\n  operationId: getProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/autocompletions/\n\
  \  method: get\n  operationId: autocompleteProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /batch/products/\n  method: post\n  operationId: batchProducts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cofactr/refs/heads/main/agentic-access/cofactr-agentic-access.yml
summary_line: 4 operations · 1 acting
tags:
- Company
- Physical Ai
- Component Intelligence
- Electronics
- Supply Chain
- Procurement
- Manufacturing
- Hardware
- Bill Of Materials
---
