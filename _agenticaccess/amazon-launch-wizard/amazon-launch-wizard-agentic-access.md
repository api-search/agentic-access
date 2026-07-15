---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 3
api_specs:
- filename: openapi.yaml
  format: yaml
  label: AWS Launch Wizard API
  slug: aws-launch-wizard-api
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/launchwizard/2018-05-10/openapi.yaml
consequence_counts:
  physical: 2
  read: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Amazon Launch Wizard Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /deployments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /deployments/{deploymentId}
operation_count: 5
overview: 'Amazon Launch Wizard exposes 5 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amazon Launch Wizard
provider_slug: amazon-launch-wizard
slug: amazon-launch-wizard-agentic-access
source_filename: amazon-launch-wizard-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/amazon-launch-wizard-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    acting: 2\n    connected: 3\n  by_consequence:\n    physical: 2\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /deployments\n  method: post\n  operationId: CreateDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deployments\n  method: get\n  operationId: ListDeployments\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deployments/{deploymentId}\n  method: get\n  operationId: GetDeployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deployments/{deploymentId}\n  method: delete\n  operationId: DeleteDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workloads\n  method: get\n  operationId: ListWorkloads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-launch-wizard/refs/heads/main/agentic-access/amazon-launch-wizard-agentic-access.yml
summary_line: 5 operations · 2 acting
tags:
- Deployment
- Enterprise Applications
- SAP
- SQL Server
---
