---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 1
api_specs:
- filename: formant-admin-api.yaml
  format: yaml
  label: Formant Admin API
  slug: formant-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formant/refs/heads/main/openapi/formant-admin-api.yaml
consequence_counts:
  read: 1
  safety-critical: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Formant Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /admin/auth/login
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /admin/commands
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /queries/stream-current-value
operation_count: 4
overview: 'Formant exposes 4 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Formant
provider_slug: formant
slug: formant-agentic-access
source_filename: formant-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/formant-admin-api.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    acting: 3\n    connected: 1\n  by_consequence:\n    safety-critical: 3\n    read: 1\n  human_in_the_loop_required: 3\noperations:\n- path: /admin/auth/login\n  method: post\n  operationId: AuthController.login\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /admin/command-templates/\n  method: get\n  operationId: CommandTemplateController.list\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/commands\n  method: post\n  operationId: CommandController.post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /queries/stream-current-value\n  method: post\n  operationId: StreamCurrentValueController.query\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/formant/refs/heads/main/agentic-access/formant-agentic-access.yml
summary_line: 4 operations · 3 acting · 3 human-in-the-loop
tags:
- Robotics
- Robot Fleet Management
- Teleoperation
- Observability
- Telemetry
- ROS
- ROS2
- Edge Devices
- Physical Operations
- Incident Management
- Industrial AI
- SCADA
- Predictive Maintenance
- Remote Monitoring
- Embedded Devices
---
