---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 4
api_specs:
- filename: google-data-studio-api-openapi.yml
  format: yaml
  label: Google Data Studio API
  slug: google-data-studio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-data-studio/refs/heads/main/openapi/google-data-studio-api-openapi.yml
- filename: google-data-studio-linking-api-openapi.yml
  format: yaml
  label: Looker Studio Linking API
  slug: looker-studio-linking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-data-studio/refs/heads/main/openapi/google-data-studio-linking-api-openapi.yml
consequence_counts:
  read: 4
  safety-critical: 1
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Google Data Studio Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /assets/{assetName}/permissions:revokeAllPermissions
operation_count: 7
overview: 'Google Data Studio exposes 7 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read, 2 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Google Data Studio
provider_slug: google-data-studio
slug: google-data-studio-agentic-access
source_filename: google-data-studio-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/google-data-studio-api-openapi.yml, openapi/google-data-studio-linking-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 4\n    acting: 3\n  by_consequence:\n    read: 4\n    write: 2\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /assets:search\n  method: get\n  operationId: searchAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/{assetName}/permissions\n  method: get\n  operationId: getPermissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/{assetName}/permissions\n  method: patch\n  operationId: patchPermissions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/{assetName}/permissions:addMembers\n  method: post\n  operationId: addMembers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/{assetName}/permissions:revokeAllPermissions\n  method: post\n  operationId: revokeAllPermissions\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n \
  \   subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /reporting/create\n  method: get\n  operationId: createReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /embed/reporting/create\n  method: get\n  operationId: createEmbeddedReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-data-studio/refs/heads/main/agentic-access/google-data-studio-agentic-access.yml
summary_line: 7 operations · 3 acting · 1 human-in-the-loop
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data
- Reporting
- Visualization
---
