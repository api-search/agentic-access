---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 1
api_specs:
- filename: nma_swagger.json
  format: json
  label: Vertica Node Management Agent API
  slug: node-management-agent-api
  spec_type: OpenAPI
  url: https://<node-host>:5554/api-docs/nma_swagger.json
consequence_counts:
  read: 1
  safety-critical: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Vertica Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/nma/shutdown
operation_count: 2
overview: 'Vertica exposes 2 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Vertica
provider_slug: vertica
slug: vertica-agentic-access
source_filename: vertica-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/vertica-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 2\n  by_action_class:\n    connected: 1\n    acting: 1\n  by_consequence:\n    read: 1\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /v1/health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/nma/shutdown\n  method: put\n  operationId: shutdownNma\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vertica/refs/heads/main/agentic-access/vertica-agentic-access.yml
summary_line: 2 operations · 1 acting · 1 human-in-the-loop
tags:
- Database
- Analytics Database
- Data Warehouse
- Data Lakehouse
- Columnar Database
- MPP
- In-Database Machine Learning
- SQL
---
