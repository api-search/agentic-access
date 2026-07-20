---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 1
api_specs:
- filename: eder-labs-persona-openapi.yml
  format: yaml
  label: Persona API
  slug: persona-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eder-labs/refs/heads/main/openapi/eder-labs-persona-openapi.yml
consequence_counts:
  read: 1
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Eder Labs Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Eder Labs exposes 7 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Eder Labs
provider_slug: eder-labs
slug: eder-labs-agentic-access
source_filename: eder-labs-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/eder-labs-persona-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 1\n    acting: 6\n  by_consequence:\n    read: 1\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /version\n  method: get\n  operationId: get_version\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{user_id}\n  method: post\n  operationId: create_user\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{user_id}\n  method: delete\n  operationId: delete_user\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{user_id}/ingest\n  method: post\n  operationId: ingest_data\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{user_id}/ingest/batch\n  method: post\n  operationId: ingest_batch_data\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n  \
  \  token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{user_id}/rag/query\n  method: post\n  operationId: rag_query\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{user_id}/ask\n  method: post\n  operationId: ask_insights\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eder-labs/refs/heads/main/agentic-access/eder-labs-agentic-access.yml
summary_line: 7 operations · 6 acting
tags:
- Company
- Cloud Saas
- AI Agents
- Memory
- Knowledge Graph
- Personalization
- Data Privacy
- Open Source
- Developer Tools
- RAG
---
