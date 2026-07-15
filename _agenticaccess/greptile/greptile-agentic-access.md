---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 1
api_specs:
- filename: greptile-openapi.yml
  format: yaml
  label: Greptile Query API
  slug: greptile-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greptile/refs/heads/main/openapi/greptile-openapi.yml
- filename: greptile-openapi.yml
  format: yaml
  label: Greptile Repositories (Indexing) API
  slug: greptile-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greptile/refs/heads/main/openapi/greptile-openapi.yml
- filename: greptile-openapi.yml
  format: yaml
  label: Greptile Search API
  slug: greptile-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greptile/refs/heads/main/openapi/greptile-openapi.yml
consequence_counts:
  read: 1
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Greptile Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'Greptile exposes 4 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Greptile
provider_slug: greptile
slug: greptile-agentic-access
source_filename: greptile-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/greptile-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    acting: 3\n    connected: 1\n  by_consequence:\n    write: 3\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /repositories\n  method: post\n  operationId: indexRepository\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /repositories/{repositoryId}\n  method: get\n  operationId: getRepository\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /query\n  method: post\n  operationId: queryRepositories\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /search\n  method: post\n  operationId: searchRepositories\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/greptile/refs/heads/main/agentic-access/greptile-agentic-access.yml
summary_line: 4 operations · 3 acting
tags:
- AI
- Codebase Understanding
- Code Review
- Code Search
- Developer Tools
---
