---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 3
api_specs:
- filename: kitforai-batch-api-openapi.yml
  format: yaml
  label: Kit For AI Batch API
  slug: kitforai-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kitforai/refs/heads/main/openapi/kitforai-batch-api-openapi.yml
- filename: kitforai-convert-api-openapi.yml
  format: yaml
  label: Kit For AI Convert API
  slug: kitforai-convert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kitforai/refs/heads/main/openapi/kitforai-convert-api-openapi.yml
- filename: kitforai-knowledge-bases-api-openapi.yml
  format: yaml
  label: Kit For AI Knowledge Bases API
  slug: kitforai-knowledge-bases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kitforai/refs/heads/main/openapi/kitforai-knowledge-bases-api-openapi.yml
consequence_counts:
  read: 3
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Kitforai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Kit For AI exposes 8 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Kit For AI
provider_slug: kitforai
slug: kitforai-agentic-access
source_filename: kitforai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: generated\nsource: openapi/kitforai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 5\n    connected: 3\n  by_consequence:\n    write: 5\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/convert\n  method: post\n  operationId: convertDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/batch\n  method: post\n  operationId: convertBatch\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/knowledge-bases\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/knowledge-bases\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/knowledge-bases/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/knowledge-bases/{id}\n  method: delete\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/knowledge-bases/{id}/documents\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/knowledge-bases/{id}/search\n  method: post\n  operationId: searchKnowledgeBase\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kitforai/refs/heads/main/agentic-access/kitforai-agentic-access.yml
summary_line: 8 operations · 5 acting
tags:
- AI
- Memory
- DocumentConversion
- RetrievalAugmentedGeneration
- KnowledgeBase
---
