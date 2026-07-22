---
acting_count: 6
action_class_counts:
  acting: 6
api_specs:
- filename: moondream-openapi.yml
  format: yaml
  label: Moondream Cloud API
  slug: moondream-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moondream/refs/heads/main/openapi/moondream-openapi.yml
consequence_counts:
  safety-critical: 5
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 5
kind: agentic-access
layout: agentic-access
method: generated
name: Moondream Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /caption
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /detect
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /point
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /query
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /segment
operation_count: 6
overview: 'Moondream exposes 6 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 write and 5 safety-critical.


  5 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Moondream
provider_slug: moondream
slug: moondream-agentic-access
source_filename: moondream-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/moondream-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    acting: 6\n  by_consequence:\n    safety-critical: 5\n    write: 1\n  human_in_the_loop_required: 5\noperations:\n- path: /query\n  method: post\n  operationId: query\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /caption\n  method: post\n  operationId: caption\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /detect\n  method: post\n  operationId: detect\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /point\n  method: post\n  operationId: point\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /segment\n\
  \  method: post\n  operationId: segment\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /chat/completions\n  method: post\n  operationId: createChatCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moondream/refs/heads/main/agentic-access/moondream-agentic-access.yml
summary_line: 6 operations · 6 acting · 5 human-in-the-loop
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Computer Vision
- Vision Language Model
- Object Detection
- Image Captioning
- OCR
- Developer Tools
---
