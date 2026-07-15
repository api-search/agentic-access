---
acting_count: 0
action_class_counts:
  connected: 6
api_specs:
- filename: wolframalpha-llm-api-openapi.yml
  format: yaml
  label: Wolfram|Alpha LLM API
  slug: llm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wolframalpha/refs/heads/main/openapi/wolframalpha-llm-api-openapi.yml
- filename: wolframalpha-full-results-api-openapi.yml
  format: yaml
  label: Wolfram|Alpha Full Results API
  slug: full-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wolframalpha/refs/heads/main/openapi/wolframalpha-full-results-api-openapi.yml
- filename: wolframalpha-short-answers-api-openapi.yml
  format: yaml
  label: Wolfram|Alpha Short Answers API
  slug: short-answers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wolframalpha/refs/heads/main/openapi/wolframalpha-short-answers-api-openapi.yml
- filename: wolframalpha-simple-api-openapi.yml
  format: yaml
  label: Wolfram|Alpha Simple API
  slug: simple-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wolframalpha/refs/heads/main/openapi/wolframalpha-simple-api-openapi.yml
- filename: wolframalpha-spoken-results-api-openapi.yml
  format: yaml
  label: Wolfram|Alpha Spoken Results API
  slug: spoken-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wolframalpha/refs/heads/main/openapi/wolframalpha-spoken-results-api-openapi.yml
- filename: wolframalpha-fast-query-recognizer-api-openapi.yml
  format: yaml
  label: Wolfram|Alpha Fast Query Recognizer API
  slug: fast-query-recognizer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wolframalpha/refs/heads/main/openapi/wolframalpha-fast-query-recognizer-api-openapi.yml
consequence_counts:
  read: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Wolframalpha Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Wolfram|Alpha exposes 6 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Wolfram|Alpha
provider_slug: wolframalpha
slug: wolframalpha-agentic-access
source_filename: wolframalpha-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/wolframalpha-fast-query-recognizer-api-openapi.yml, openapi/wolframalpha-full-results-api-openapi.yml,\n  openapi/wolframalpha-llm-api-openapi.yml, openapi/wolframalpha-short-answers-api-openapi.yml,\n  openapi/wolframalpha-simple-api-openapi.yml, openapi/wolframalpha-spoken-results-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 6\n  by_consequence:\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /query.jsp\n  method: get\n  operationId: recognizeQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /query\n\
  \  method: get\n  operationId: queryFullResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llm-api\n  method: get\n  operationId: queryLlmApi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /result\n  method: get\n  operationId: queryShortAnswer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /simple\n  method: get\n  operationId: querySimpleApi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spoken\n  method: get\n  operationId: querySpokenResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n  \
  \    max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wolframalpha/refs/heads/main/agentic-access/wolframalpha-agentic-access.yml
summary_line: 6 operations
tags:
- AI
- Artificial Intelligence
- Computational Knowledge
- Machine Learning
- Natural Language Processing
- Public APIs
- Search
---
