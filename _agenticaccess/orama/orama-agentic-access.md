---
acting_count: 8
action_class_counts:
  acting: 8
api_specs:
- filename: orama-openapi.yml
  format: yaml
  label: Orama Cloud Indexes and Collections
  slug: indexes-collections
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orama/refs/heads/main/openapi/orama-openapi.yml
- filename: orama-openapi.yml
  format: yaml
  label: Orama Cloud Documents
  slug: documents
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orama/refs/heads/main/openapi/orama-openapi.yml
- filename: orama-openapi.yml
  format: yaml
  label: Orama Cloud Search
  slug: search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orama/refs/heads/main/openapi/orama-openapi.yml
- filename: orama-openapi.yml
  format: yaml
  label: Orama Cloud Answer Sessions (RAG)
  slug: answer-sessions-rag
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orama/refs/heads/main/openapi/orama-openapi.yml
consequence_counts:
  physical: 1
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Orama Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/webhooks/{indexId}/deploy
operation_count: 8
overview: 'Orama exposes 8 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 write and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Orama
provider_slug: orama
slug: orama-agentic-access
source_filename: orama-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/orama-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 8\n  by_consequence:\n    write: 7\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/webhooks/{indexId}/update-schema\n  method: post\n  operationId: updateSchema\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/webhooks/{indexId}/has-data\n  method: post\n  operationId: hasData\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/webhooks/{indexId}/empty\n  method: post\n  operationId: emptyIndex\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/webhooks/{indexId}/deploy\n  method: post\n  operationId: deployIndex\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/v1/webhooks/{indexId}/notify\n  method: post\n  operationId: notify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/webhooks/{indexId}/snapshot\n  method: post\n  operationId: snapshot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/indexes/{indexId}/search\n  method: post\n  operationId: search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/answer\n  method: post\n  operationId: answer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orama/refs/heads/main/agentic-access/orama-agentic-access.yml
summary_line: 8 operations · 8 acting
tags:
- Search
- Vector Search
- RAG
- Open Source
- Search as a Service
---
