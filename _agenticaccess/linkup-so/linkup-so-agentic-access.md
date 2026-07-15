---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 2
api_specs:
- filename: linkup-so-openapi.yml
  format: yaml
  label: Linkup Search API
  slug: linkup-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkup-so/refs/heads/main/openapi/linkup-so-openapi.yml
- filename: linkup-so-openapi.yml
  format: yaml
  label: Linkup Fetch API
  slug: linkup-fetch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkup-so/refs/heads/main/openapi/linkup-so-openapi.yml
- filename: linkup-so-openapi.yml
  format: yaml
  label: Linkup Research API
  slug: linkup-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkup-so/refs/heads/main/openapi/linkup-so-openapi.yml
- filename: linkup-so-openapi.yml
  format: yaml
  label: Linkup Credits API
  slug: linkup-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkup-so/refs/heads/main/openapi/linkup-so-openapi.yml
consequence_counts:
  read: 2
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Linkup So Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Linkup exposes 5 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Linkup
provider_slug: linkup-so
slug: linkup-so-agentic-access
source_filename: linkup-so-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/linkup-so-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    acting: 3\n    connected: 2\n  by_consequence:\n    write: 3\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /search\n  method: post\n  operationId: search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fetch\n  method: post\n  operationId: fetch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /research\n  method: post\n  operationId: createResearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /research/{id}\n  method: get\n  operationId: getResearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /credits/balance\n  method: get\n  operationId: getCreditsBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linkup-so/refs/heads/main/agentic-access/linkup-so-agentic-access.yml
summary_line: 5 operations · 3 acting
tags:
- AI
- LLM
- Web Search
- Grounding
- RAG
---
