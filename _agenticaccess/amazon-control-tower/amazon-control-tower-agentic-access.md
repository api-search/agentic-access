---
acting_count: 27
action_class_counts:
  acting: 27
  connected: 1
api_specs:
- filename: amazon-control-tower-openapi.yml
  format: yaml
  label: AWS Control Tower API
  slug: aws-control-tower-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/openapi/amazon-control-tower-openapi.yml
consequence_counts:
  read: 1
  safety-critical: 27
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 27
kind: agentic-access
layout: agentic-access
method: generated
name: Amazon Control Tower Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /create-landingzone
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /delete-landingzone
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /disable-baseline
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /disable-control
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /enable-baseline
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /enable-control
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /get-baseline
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /get-baseline-operation
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /get-control-operation
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /get-enabled-baseline
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /get-enabled-control
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /get-landingzone
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /get-landingzone-operation
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /list-baselines
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /list-control-operations
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /list-enabled-baselines
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /list-enabled-controls
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /list-landingzone-operations
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /list-landingzones
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /reset-enabled-baseline
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /reset-enabled-control
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /reset-landingzone
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /tags/{resourceArn}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /tags/{resourceArn}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /update-enabled-baseline
operation_count: 28
overview: 'Amazon Control Tower exposes 28 API operations that an AI agent could call, of which 27 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 27 safety-critical.


  27 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amazon Control Tower
provider_slug: amazon-control-tower
slug: amazon-control-tower-agentic-access
source_filename: amazon-control-tower-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/amazon-control-tower-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 28\n  by_action_class:\n    acting: 27\n    connected: 1\n  by_consequence:\n    safety-critical: 27\n    read: 1\n  human_in_the_loop_required: 27\noperations:\n- path: /create-landingzone\n  method: post\n  operationId: createLandingZone\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /delete-landingzone\n  method: post\n  operationId:\
  \ deleteLandingZone\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /get-landingzone\n  method: post\n  operationId: getLandingZone\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /list-landingzones\n  method: post\n  operationId: listLandingZones\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /update-landingzone\n  method: post\n  operationId: updateLandingZone\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /reset-landingzone\n  method: post\n  operationId: resetLandingZone\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /get-landingzone-operation\n  method: post\n  operationId: getLandingZoneOperation\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /list-landingzone-operations\n  method: post\n  operationId: listLandingZoneOperations\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /enable-control\n  method: post\n  operationId: enableControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /disable-control\n  method: post\n  operationId: disableControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /get-enabled-control\n  method: post\n  operationId: getEnabledControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /list-enabled-controls\n  method: post\n  operationId: listEnabledControls\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /update-enabled-control\n  method: post\n  operationId: updateEnabledControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /reset-enabled-control\n  method: post\n  operationId: resetEnabledControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n     \
  \ human-in-the-loop: required\n    audit: required\n- path: /get-control-operation\n  method: post\n  operationId: getControlOperation\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /list-control-operations\n  method: post\n  operationId: listControlOperations\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /enable-baseline\n  method: post\n  operationId: enableBaseline\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /disable-baseline\n  method: post\n  operationId: disableBaseline\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /get-baseline\n  method: post\n  operationId: getBaseline\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n\
  - path: /list-baselines\n  method: post\n  operationId: listBaselines\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /get-enabled-baseline\n  method: post\n  operationId: getEnabledBaseline\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /list-enabled-baselines\n  method: post\n  operationId: listEnabledBaselines\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /update-enabled-baseline\n  method: post\n  operationId: updateEnabledBaseline\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /reset-enabled-baseline\n  method: post\n  operationId: resetEnabledBaseline\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /get-baseline-operation\n\
  \  method: post\n  operationId: getBaselineOperation\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /tags/{resourceArn}\n  method: get\n  operationId: listTagsForResource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tags/{resourceArn}\n  method: post\n  operationId: tagResource\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /tags/{resourceArn}\n\
  \  method: delete\n  operationId: untagResource\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/agentic-access/amazon-control-tower-agentic-access.yml
summary_line: 28 operations · 27 acting · 27 human-in-the-loop
tags:
- Compliance
- Governance
- Landing Zone
- Multi-Account
- Security
- Controls
---
