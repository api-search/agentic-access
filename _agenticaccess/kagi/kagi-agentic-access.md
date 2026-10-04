---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 2
api_specs:
- filename: kagi-extract-api-openapi.yml
  format: yaml
  label: Kagi Extract API
  slug: kagi-extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kagi/refs/heads/main/openapi/kagi-extract-api-openapi.yml
- filename: kagi-search-api-openapi.yml
  format: yaml
  label: Kagi Search API
  slug: kagi-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kagi/refs/heads/main/openapi/kagi-search-api-openapi.yml
consequence_counts:
  read: 2
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Kagi Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 3
overview: 'Kagi exposes 3 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Kagi
provider_slug: kagi
slug: kagi-agentic-access
source_filename: kagi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/kagi-extract-api-openapi.yml, openapi/kagi-search-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 3\n  by_action_class:\n    acting: 1\n    connected: 2\n  by_consequence:\n    write: 1\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /extract\n  method: post\n  operationId: extract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /search\n  method: post\n  operationId: search\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search\n  method: get\n  operationId: searchGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kagi/refs/heads/main/agentic-access/kagi-agentic-access.yml
summary_line: 3 operations · 1 acting
tags:
- Search
- Premium Search
- AI Search
- Summarization
- FastGPT
- Enrichment
- OpenAPI
- Pay-Per-Use
- Privacy
- LLM
- Web Index
---
