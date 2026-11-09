---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 2
api_specs:
- filename: boncourant-fr-audit-api-openapi.yml
  format: yaml
  label: Boncourant Audit API
  slug: boncourant-fr-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/boncourant-fr/openapi/boncourant-fr-audit-api-openapi.yml
- filename: boncourant-fr-commissions-api-openapi.yml
  format: yaml
  label: Boncourant Commissions API
  slug: boncourant-fr-commissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/boncourant-fr/openapi/boncourant-fr-commissions-api-openapi.yml
- filename: boncourant-fr-mcp-api-openapi.yml
  format: yaml
  label: Boncourant MCP API
  slug: boncourant-fr-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/boncourant-fr/openapi/boncourant-fr-mcp-api-openapi.yml
- filename: boncourant-fr-simulate-api-openapi.yml
  format: yaml
  label: Boncourant Simulate API
  slug: boncourant-fr-simulate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/boncourant-fr/openapi/boncourant-fr-simulate-api-openapi.yml
- filename: boncourant-fr-trv-gap-api-openapi.yml
  format: yaml
  label: Boncourant Trv Gap API
  slug: boncourant-fr-trv-gap-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/boncourant-fr/openapi/boncourant-fr-trv-gap-api-openapi.yml
consequence_counts:
  read: 2
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Boncourant Fr Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Boncourant exposes 6 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Boncourant
provider_slug: boncourant-fr
slug: boncourant-fr-agentic-access
source_filename: boncourant-fr-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/boncourant-fr-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    acting: 4\n    connected: 2\n  by_consequence:\n    write: 4\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/simulate\n  method: post\n  operationId: simulateResidential\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/audit\n  method: post\n  operationId: analyzeStructuredBill\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/simulate/pro\n  method: post\n  operationId: estimateC5Base\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/trv-gap\n  method: get\n  operationId: getTrvGap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/commissions\n  method: get\n  operationId: getCommissionEvidence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /mcp\n  method: post\n  operationId: callPublicTool\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/boncourant-fr/agentic-access/boncourant-fr-agentic-access.yml
summary_line: 6 operations · 4 acting
tags:
- Electricity
- Audit
- Optimization
- France
- Independent
---
