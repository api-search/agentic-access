---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 5
api_specs:
- filename: nerdio-distributor-api-openapi.json
  format: json
  label: Nerdio Manager Distributor API
  slug: nerdio-manager-distributor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nerdio/refs/heads/main/openapi/nerdio-distributor-api-openapi.json
consequence_counts:
  physical: 2
  read: 5
  safety-critical: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Nerdio Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api-v{version}/reactivate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api-v{version}/suspend
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api-v{version}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api-v{version}/register
operation_count: 9
overview: 'Nerdio exposes 9 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read, 2 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Nerdio
provider_slug: nerdio
slug: nerdio-agentic-access
source_filename: nerdio-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: generated\nsource: openapi/nerdio-distributor-api-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 5\n    acting: 4\n  by_consequence:\n    read: 5\n    physical: 2\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /api-v{version}/checkhealth\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api-v{version}/installs\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api-v{version}/register\n  method:\
  \ post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api-v{version}/suspend\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api-v{version}/reactivate\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /api-v{version}/cancel\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api-v{version}/invoices\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api-v{version}/invoices/grouped\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api-v{version}/usage\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nerdio/refs/heads/main/agentic-access/nerdio-agentic-access.yml
summary_line: 9 operations · 4 acting · 2 human-in-the-loop
tags:
- Company
- Azure Virtual Desktop
- Windows 365
- Virtual Desktop Infrastructure
- Cloud Desktop Management
- Microsoft Intune
- Managed Service Providers
- Cloud Cost Optimization
- Endpoint Management
- IT Automation
---
