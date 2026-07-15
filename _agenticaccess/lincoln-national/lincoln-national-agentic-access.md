---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 1
api_specs:
- filename: lincoln-national-openapi.yml
  format: yaml
  label: Lincoln Financial LincSmart Enrollment API
  slug: lincsmart-enrollment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lincoln-national/refs/heads/main/openapi/lincoln-national-openapi.yml
- filename: lincoln-national-openapi.yml
  format: yaml
  label: Lincoln Financial LincSmart EOI Solution API
  slug: lincsmart-eoi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lincoln-national/refs/heads/main/openapi/lincoln-national-openapi.yml
- filename: lincoln-national-openapi.yml
  format: yaml
  label: Lincoln Financial LincSmart Plan Design API
  slug: lincsmart-plan-design-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lincoln-national/refs/heads/main/openapi/lincoln-national-openapi.yml
consequence_counts:
  read: 1
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Lincoln National Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 3
overview: 'Lincoln National exposes 3 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Lincoln National
provider_slug: lincoln-national
slug: lincoln-national-agentic-access
source_filename: lincoln-national-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/lincoln-national-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 3\n  by_action_class:\n    acting: 2\n    connected: 1\n  by_consequence:\n    write: 2\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /enrollment\n  method: post\n  operationId: syncEnrollment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /eoi\n  method: post\n  operationId: submitEOI\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /plan-design\n  method: get\n  operationId: getPlanDesign\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lincoln-national/refs/heads/main/agentic-access/lincoln-national-agentic-access.yml
summary_line: 3 operations · 2 acting
tags:
- Annuities
- Benefits
- Enrollment
- HR
- Insurance
- Retirement
- Fortune 500
---
