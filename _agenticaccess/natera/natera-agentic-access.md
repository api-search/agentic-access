---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 1
api_specs:
- filename: natera-openapi.yml
  format: yaml
  label: Natera EMR Ordering and Results Integration
  slug: natera-emr-ordering-integration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natera/refs/heads/main/openapi/natera-openapi.yml
consequence_counts:
  physical: 1
  read: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Natera Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /emr/orders
operation_count: 2
overview: 'Natera exposes 2 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Natera
provider_slug: natera
slug: natera-agentic-access
source_filename: natera-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/natera-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 2\n  by_action_class:\n    acting: 1\n    connected: 1\n  by_consequence:\n    physical: 1\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /emr/orders\n  method: post\n  operationId: submitOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /emr/results/{orderId}\n  method: get\n  operationId: getResults\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/natera/refs/heads/main/agentic-access/natera-agentic-access.yml
summary_line: 2 operations · 1 acting
tags:
- Genetic Testing
- Healthcare
- Diagnostics
- EHR Integration
- HL7
---
