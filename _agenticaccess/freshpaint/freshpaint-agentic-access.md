---
acting_count: 1
action_class_counts:
  acting: 1
api_specs:
- filename: freshpaint-openapi.yml
  format: yaml
  label: Freshpaint Tracking Events API
  slug: freshpaint-tracking-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshpaint/refs/heads/main/openapi/freshpaint-openapi.yml
- filename: freshpaint-openapi.yml
  format: yaml
  label: Freshpaint Identify API
  slug: freshpaint-identify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshpaint/refs/heads/main/openapi/freshpaint-openapi.yml
- filename: freshpaint-openapi.yml
  format: yaml
  label: Freshpaint Page and Screen API
  slug: freshpaint-page-screen-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshpaint/refs/heads/main/openapi/freshpaint-openapi.yml
consequence_counts:
  physical: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Freshpaint Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /track
operation_count: 1
overview: 'Freshpaint exposes 1 API operation that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Freshpaint
provider_slug: freshpaint
slug: freshpaint-agentic-access
source_filename: freshpaint-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/freshpaint-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 1\n  by_action_class:\n    acting: 1\n  by_consequence:\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /track\n  method: post\n  operationId: track\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freshpaint/refs/heads/main/agentic-access/freshpaint-agentic-access.yml
summary_line: 1 operation · 1 acting
tags:
- Customer Data Platform
- Event Tracking
- Healthcare
- HIPAA
- Privacy
- Analytics
---
