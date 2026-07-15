---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 1
api_specs:
- filename: unisys-stealth-ecoapi-openapi.yaml
  format: yaml
  label: Unisys Stealth EcoAPI
  slug: unisys-stealth-ecoapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unisys/refs/heads/main/openapi/unisys-stealth-ecoapi-openapi.yaml
consequence_counts:
  read: 1
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Unisys Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Unisys exposes 7 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Unisys
provider_slug: unisys
slug: unisys-agentic-access
source_filename: unisys-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/unisys-stealth-ecoapi-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 1\n    acting: 6\n  by_consequence:\n    read: 1\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /api/roles\n  method: get\n  operationId: getStealthRoles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/endpoint/isolate\n  method: post\n  operationId: isolateEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n    \
  \  human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/endpoint/unisolate\n  method: post\n  operationId: unisolateEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/user/isolate\n  method: post\n  operationId: isolateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/user/unisolate\n  method: post\n  operationId: unisolateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/isolate\n  method: post\n  operationId: isolateMachineAndUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/unisolate\n  method: post\n  operationId: unisolateMachineAndUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unisys/refs/heads/main/agentic-access/unisys-agentic-access.yml
summary_line: 7 operations · 6 acting
tags:
- Fortune 1000
- Security
- Zero Trust
- Network Security
- IT Services
- Cybersecurity
- Enterprise Technology
---
