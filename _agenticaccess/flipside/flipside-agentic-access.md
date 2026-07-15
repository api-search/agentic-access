---
acting_count: 1
action_class_counts:
  acting: 1
api_specs:
- filename: flipside-openapi.yml
  format: yaml
  label: Query Execution (SQL)
  slug: query-execution-sql
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipside/refs/heads/main/openapi/flipside-openapi.yml
- filename: flipside-openapi.yml
  format: yaml
  label: Query Results
  slug: query-results
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipside/refs/heads/main/openapi/flipside-openapi.yml
- filename: flipside-openapi.yml
  format: yaml
  label: Datasets
  slug: datasets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flipside/refs/heads/main/openapi/flipside-openapi.yml
consequence_counts:
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Flipside Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 1
overview: 'Flipside Crypto exposes 1 API operation that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Flipside Crypto
provider_slug: flipside
slug: flipside-agentic-access
source_filename: flipside-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/flipside-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 1\n  by_action_class:\n    acting: 1\n  by_consequence:\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /json-rpc\n  method: post\n  operationId: jsonRpc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flipside/refs/heads/main/agentic-access/flipside-agentic-access.yml
summary_line: 1 operation · 1 acting
tags:
- Blockchain
- Analytics
- SQL
- Web3
- Data
---
