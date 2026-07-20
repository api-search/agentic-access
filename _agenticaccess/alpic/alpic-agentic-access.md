---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 13
api_specs:
- filename: alpic-openapi-original.json
  format: json
  label: Alpic API
  slug: alpic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpic/refs/heads/main/openapi/alpic-openapi-original.json
consequence_counts:
  physical: 1
  read: 13
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Alpic Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/environments/{environmentId}/deploy
operation_count: 24
overview: 'Alpic exposes 24 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read, 10 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Alpic
provider_slug: alpic
slug: alpic-agentic-access
source_filename: alpic-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: generated\nsource: openapi/alpic-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 24\n  by_action_class:\n    connected: 13\n    acting: 11\n  by_consequence:\n    read: 13\n    write: 10\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/teams\n  method: get\n  operationId: teams.list.v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/analytics/{projectId}\n  method: get\n  operationId: analytics.get.v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/deployments/{deploymentId}\n  method: get\n  operationId: deployments.get.v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/environments\n  method: post\n  operationId: environments.create.v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/environments/{environmentId}\n  method: get\n  operationId: environments.get.v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/environments/{environmentId}/deploy\n  method: post\n  operationId: environments.deploy.v1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/environments/{environmentId}/logs\n  method: get\n  operationId: environments.getLogs.v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/environments/{environmentId}/latest-logs\n  method: get\n  operationId: environments.getLatestLogs.v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/environments/{environmentId}/environment-variables\n  method: get\n  operationId: environmentVariables.list.v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/environments/{environmentId}/environment-variables\n  method: post\n  operationId: environmentVariables.create.v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/environment-variables/{environmentVariableId}\n  method: patch\n  operationId: environmentVariables.update.v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/environment-variables/{environmentVariableId}\n  method: delete\n  operationId: environmentVariables.delete.v1\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects/{projectId}\n  method: patch\n  operationId: projects.update.v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects/{projectId}\n  method: get\n  operationId: projects.get.v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{projectId}\n  method: delete\n  operationId: projects.delete.v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects\n  method: get\n  operationId: projects.list.v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects\n  method: post\n  operationId: projects.create.v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/environments/{environmentId}/playground\n  method: get\n  operationId: playground.get.v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/environments/{environmentId}/playground\n  method: put\n  operationId: playground.upsert.v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tunnels/ticket\n  method: get\n  operationId: tunnels.getTicket.v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/distribution/publish\n  method: post\n  operationId: distribution.publish.v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/distribution/get\n\
  \  method: get\n  operationId: distribution.get.v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/beacon/audits\n  method: post\n  operationId: beacon.create.v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/beacon/audits/{auditId}\n  method: get\n  operationId: beacon.get.v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alpic/refs/heads/main/agentic-access/alpic-agentic-access.yml
summary_line: 24 operations · 11 acting
tags:
- Company
- Ai/Ml
- MCP
- Model Context Protocol
- Cloud Platform
- Developer Tools
- Deployment
- ChatGPT Apps
- Agentic
---
