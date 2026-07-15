---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 1
api_specs:
- filename: north-cloud-openapi.yml
  format: yaml
  label: North.Cloud Public API
  slug: north-cloud
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/north-cloud/refs/heads/main/openapi/north-cloud-openapi.yml
consequence_counts:
  read: 1
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: North Cloud Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 2
overview: 'North.Cloud exposes 2 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: North.Cloud
provider_slug: north-cloud
slug: north-cloud-agentic-access
source_filename: north-cloud-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/north-cloud-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 2\n  by_action_class:\n    connected: 1\n    acting: 1\n  by_consequence:\n    read: 1\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /public/cost-units\n  method: get\n  operationId: getCostUnit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/cost-units\n  method: post\n  operationId: updateCostUnit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/north-cloud/refs/heads/main/agentic-access/north-cloud-agentic-access.yml
summary_line: 2 operations · 1 acting
tags:
- FinOps
- Cloud Cost Management
- GCP
- Cost Optimization
- Cost Units
---
