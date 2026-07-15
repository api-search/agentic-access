---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 3
api_specs:
- filename: counter-dev-openapi.yml
  format: yaml
  label: Counter Tracking / Collect API
  slug: counter-dev-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/counter-dev/refs/heads/main/openapi/counter-dev-openapi.yml
- filename: counter-dev-openapi.yml
  format: yaml
  label: Counter Stats / Dashboard Data API
  slug: counter-dev-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/counter-dev/refs/heads/main/openapi/counter-dev-openapi.yml
- filename: counter-dev-openapi.yml
  format: yaml
  label: Counter Account API
  slug: counter-dev-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/counter-dev/refs/heads/main/openapi/counter-dev-openapi.yml
consequence_counts:
  read: 3
  safety-critical: 1
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Counter Dev Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /resettoken
operation_count: 8
overview: 'Counter exposes 8 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read, 4 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Counter
provider_slug: counter-dev
slug: counter-dev-agentic-access
source_filename: counter-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/counter-dev-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 3\n    acting: 5\n  by_consequence:\n    read: 3\n    write: 4\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /track\n  method: get\n  operationId: track\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trackpage\n  method: post\n  operationId: trackpage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /query\n  method: get\n  operationId: query\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dump\n  method: get\n  operationId: dump\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resettoken\n  method: post\n  operationId: resetToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /login\n  method: post\n  operationId: login\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /register\n  method: post\n  operationId: register\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /logout\n  method: post\n  operationId: logout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/counter-dev/refs/heads/main/agentic-access/counter-dev-agentic-access.yml
summary_line: 8 operations · 5 acting · 1 human-in-the-loop
tags:
- Web Analytics
- Privacy
- Open Source
- Tracking
- Self-Hosted
---
