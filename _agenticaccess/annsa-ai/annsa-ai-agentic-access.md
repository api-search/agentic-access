---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 1
api_specs:
- filename: annsa-ai-agents-api-openapi.yml
  format: yaml
  label: Annsa Agents API
  slug: annsa-ai-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/annsa-ai/openapi/annsa-ai-agents-api-openapi.yml
- filename: annsa-ai-ingest-api-openapi.yml
  format: yaml
  label: Annsa Ingest API
  slug: annsa-ai-ingest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/annsa-ai/openapi/annsa-ai-ingest-api-openapi.yml
- filename: annsa-ai-service-api-openapi.yml
  format: yaml
  label: Annsa Service API
  slug: annsa-ai-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/annsa-ai/openapi/annsa-ai-service-api-openapi.yml
consequence_counts:
  read: 1
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Annsa Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Annsa exposes 5 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Annsa
provider_slug: annsa-ai
slug: annsa-ai-agentic-access
source_filename: annsa-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/annsa-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    acting: 4\n    connected: 1\n  by_consequence:\n    write: 4\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /feedback\n  method: post\n  operationId: submitFeedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transcripts/upload\n  method: post\n  operationId: uploadTranscript\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /surface/submit\n  method: post\n  operationId: submitSurveyFeedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp\n  method: post\n  operationId: callMcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - read\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/annsa-ai/agentic-access/annsa-ai-agentic-access.yml
summary_line: 5 operations · 4 acting
tags:
- Project Management
- Customer Management
- Agent Teams
- Artificial Intelligence
- Software-as-a-Service
---
