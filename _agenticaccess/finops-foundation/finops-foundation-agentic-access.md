---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 4
api_specs:
- filename: finops-foundation-focus-cost-and-usage-openapi.yml
  format: yaml
  label: FOCUS Cost and Usage API
  slug: focus-cost-and-usage
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finops-foundation/refs/heads/main/openapi/finops-foundation-focus-cost-and-usage-openapi.yml
consequence_counts:
  read: 4
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Finops Foundation Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'FinOps Foundation exposes 5 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: FinOps Foundation
provider_slug: finops-foundation
slug: finops-foundation-agentic-access
source_filename: finops-foundation-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/finops-foundation-focus-cost-and-usage-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 4\n    acting: 1\n  by_consequence:\n    read: 4\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /cost-and-usage\n  method: get\n  operationId: listCostAndUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cost-and-usage/export\n  method: post\n  operationId: exportCostAndUsage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cost-and-usage/export/{jobId}\n  method: get\n  operationId: getCostAndUsageExportStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contract-commitments\n  method: get\n  operationId: listContractCommitments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schema\n  method: get\n  operationId: getSchemaMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finops-foundation/refs/heads/main/agentic-access/finops-foundation-agentic-access.yml
summary_line: 5 operations · 1 acting
tags:
- Budgets
- Costs
- FinOps
---
