---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 2
api_specs:
- filename: mnemoverse-com-health-api-openapi.yml
  format: yaml
  label: Mnemoverse Health API
  slug: mnemoverse-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mnemoverse-com/openapi/mnemoverse-com-health-api-openapi.yml
- filename: mnemoverse-com-memory-api-openapi.yml
  format: yaml
  label: Mnemoverse Memory API
  slug: mnemoverse-com-memory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mnemoverse-com/openapi/mnemoverse-com-memory-api-openapi.yml
- filename: mnemoverse-com-memory-v1-api-openapi.yml
  format: yaml
  label: Mnemoverse Memory V1 API
  slug: mnemoverse-com-memory-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mnemoverse-com/openapi/mnemoverse-com-memory-v1-api-openapi.yml
- filename: mnemoverse-com-vault-api-openapi.yml
  format: yaml
  label: Mnemoverse Vault API
  slug: mnemoverse-com-vault-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mnemoverse-com/openapi/mnemoverse-com-vault-api-openapi.yml
consequence_counts:
  read: 2
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Mnemoverse Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'Mnemoverse exposes 4 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Mnemoverse
provider_slug: mnemoverse-com
slug: mnemoverse-com-agentic-access
source_filename: mnemoverse-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/mnemoverse-com-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    acting: 2\n    connected: 2\n  by_consequence:\n    write: 2\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /memory/write\n  method: post\n  operationId: writeMemory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /memory/read\n  method: post\n  operationId: readMemory\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /memory/feedback\n  method: post\n  operationId: giveFeedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /memory/stats\n  method: get\n  operationId: getMemoryStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/mnemoverse-com/agentic-access/mnemoverse-com-agentic-access.yml
summary_line: 4 operations · 2 acting
tags:
- Company
- Artificial Intelligence
- Memory
- Persistent
---
