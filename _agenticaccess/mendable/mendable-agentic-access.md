---
acting_count: 6
action_class_counts:
  acting: 6
api_specs:
- filename: mendable-openapi.yml
  format: yaml
  label: Mendable Chat & Answers API
  slug: mendable-chat-answers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mendable/refs/heads/main/openapi/mendable-openapi.yml
- filename: mendable-openapi.yml
  format: yaml
  label: Mendable Conversations API
  slug: mendable-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mendable/refs/heads/main/openapi/mendable-openapi.yml
- filename: mendable-openapi.yml
  format: yaml
  label: Mendable Data Ingestion & Sources API
  slug: mendable-data-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mendable/refs/heads/main/openapi/mendable-openapi.yml
- filename: mendable-openapi.yml
  format: yaml
  label: Mendable Ratings API
  slug: mendable-ratings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mendable/refs/heads/main/openapi/mendable-openapi.yml
consequence_counts:
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Mendable Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Mendable exposes 6 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Mendable
provider_slug: mendable
slug: mendable-agentic-access
source_filename: mendable-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/mendable-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    acting: 6\n  by_consequence:\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /newConversation\n  method: post\n  operationId: newConversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mendableChat\n  method: post\n  operationId: mendableChat\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ingestData\n  method: post\n  operationId: ingestData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ingestDocuments\n  method: post\n  operationId: ingestDocuments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ingestionStatus\n  method: post\n  operationId: ingestionStatus\n  x-agentic-access:\n    action-class: acting\n  \
  \  consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rateMessage\n  method: post\n  operationId: rateMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mendable/refs/heads/main/agentic-access/mendable-agentic-access.yml
summary_line: 6 operations · 6 acting
tags:
- AI
- Answers
- Enterprise Search
- RAG
- Support
---
