---
acting_count: 0
action_class_counts:
  connected: 7
api_specs:
- filename: bfe-management-api.yaml
  format: yaml
  label: BFE Management API
  slug: bfe-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bfe/refs/heads/main/openapi/bfe-management-api.yaml
consequence_counts:
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bfe Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'BFE exposes 7 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BFE
provider_slug: bfe
slug: bfe-agentic-access
source_filename: bfe-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/bfe-management-api.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 7\n  by_consequence:\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /monitor\n  method: get\n  operationId: listMonitorCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monitor/{name}\n  method: get\n  operationId: getMonitorMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reload\n  method: get\n  operationId: listReloadEntries\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reload/{name}\n  method: get\n  operationId: reloadConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /debug/pprof/\n  method: get\n  operationId: getPprofIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /debug/cmdline\n  method: get\n  operationId: getCommandLine\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /debug/profile\n  method: get\n  operationId: getCpuProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bfe/refs/heads/main/agentic-access/bfe-agentic-access.yml
summary_line: 7 operations
tags:
- Load Balancer
- Networking
- Open Source
- Traffic Management
- CNCF
- Baidu
---
