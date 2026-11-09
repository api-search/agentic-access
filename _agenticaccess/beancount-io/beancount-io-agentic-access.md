---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 4
api_specs:
- filename: beancount-io-ledger-api-openapi.yml
  format: yaml
  label: Beancount.io Ledger API
  slug: beancount-io-ledger-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beancount-io/openapi/beancount-io-ledger-api-openapi.yml
- filename: beancount-io-mcp-api-openapi.yml
  format: yaml
  label: Beancount.io MCP API
  slug: beancount-io-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beancount-io/openapi/beancount-io-mcp-api-openapi.yml
- filename: beancount-io-graph-ql-api-openapi.yml
  format: yaml
  label: Beancount.io Graph QL API
  slug: beancount-io-graph-ql-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beancount-io/openapi/beancount-io-graph-ql-api-openapi.yml
consequence_counts:
  read: 4
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Beancount Io Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Beancount.io exposes 6 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Beancount.io
provider_slug: beancount-io
slug: beancount-io-agentic-access
source_filename: beancount-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/beancount-io-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    acting: 2\n    connected: 4\n  by_consequence:\n    write: 2\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /graphql\n  method: post\n  operationId: executeGraphQL\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /graphql\n  method: get\n  operationId: graphqlIntrospection\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api-gateway/mcp\n  method: post\n  operationId: mcpCall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - read\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api-gateway/mcp\n  method: get\n  operationId: mcpManifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n- path: /mcp\n  method: get\n  operationId: mcpInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n\
  - path: /docs/{slug}\n  method: get\n  operationId: getDoc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n"
source_yaml_url: https://artifacts.apis.io/beancount-io/agentic-access/beancount-io-agentic-access.yml
summary_line: 6 operations · 2 acting
tags:
- Accounting
- Finance
- Software-as-a-Service
- Open Source
- Collaboration
---
