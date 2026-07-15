---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 1
api_specs:
- filename: presto-foundation-openapi.yml
  format: yaml
  label: Presto Client REST API
  slug: presto-client-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/presto-foundation/refs/heads/main/openapi/presto-foundation-openapi.yml
consequence_counts:
  read: 1
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Presto Foundation Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 3
overview: 'Presto Foundation exposes 3 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Presto Foundation
provider_slug: presto-foundation
slug: presto-foundation-agentic-access
source_filename: presto-foundation-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/presto-foundation-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 3\n  by_action_class:\n    acting: 2\n    connected: 1\n  by_consequence:\n    write: 2\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/statement\n  method: post\n  operationId: submitStatement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/statement/{queryId}/{token}\n  method: get\n  operationId: getStatementResults\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/statement/{queryId}/{token}\n  method: delete\n  operationId: cancelStatement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/presto-foundation/refs/heads/main/agentic-access/presto-foundation-agentic-access.yml
summary_line: 3 operations · 2 acting
tags:
- Analytics
- Big Data
- Distributed SQL
- Linux Foundation
- Open Source
- Query Engine
- SQL
---
