---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 7
api_specs:
- filename: libertai-aleph-credits-api-openapi.yml
  format: yaml
  label: LibertAI Aleph Credits API
  slug: libertai-aleph-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/libertai/refs/heads/main/openapi/libertai-aleph-credits-api-openapi.yml
- filename: libertai-auth-api-openapi.yml
  format: yaml
  label: LibertAI Auth API
  slug: libertai-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/libertai/refs/heads/main/openapi/libertai-auth-api-openapi.yml
- filename: libertai-health-api-openapi.yml
  format: yaml
  label: LibertAI Health API
  slug: libertai-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/libertai/refs/heads/main/openapi/libertai-health-api-openapi.yml
- filename: libertai-models-api-openapi.yml
  format: yaml
  label: LibertAI Models API
  slug: libertai-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/libertai/refs/heads/main/openapi/libertai-models-api-openapi.yml
- filename: libertai-proxy-api-openapi.yml
  format: yaml
  label: LibertAI Proxy API
  slug: libertai-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/libertai/refs/heads/main/openapi/libertai-proxy-api-openapi.yml
- filename: libertai-search-api-openapi.yml
  format: yaml
  label: LibertAI Search API
  slug: libertai-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/libertai/refs/heads/main/openapi/libertai-search-api-openapi.yml
consequence_counts:
  physical: 1
  read: 7
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Libertai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /libertai/aleph-credits
operation_count: 9
overview: 'LibertAI exposes 9 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read, 1 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: LibertAI
provider_slug: libertai
slug: libertai-agentic-access
source_filename: libertai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: generated\nsource: openapi/libertai-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 7\n    acting: 2\n  by_consequence:\n    read: 7\n    physical: 1\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /health\n  method: get\n  operationId: health_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /libertai/auth/check\n  method: get\n  operationId: check_auth_libertai_auth_check_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /libertai/models\n  method: get\n  operationId: models_list_libertai_models_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/models\n  method: get\n  operationId: openai_models_list_v1_models_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openrouter/models\n  method: get\n  operationId: openrouter_models_list_openrouter_models_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /libertai/aleph-credits\n  method: post\n  operationId: purchase_aleph_credits_libertai_aleph_credits_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n   \
  \   purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /search\n  method: post\n  operationId: search_search_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/fetch\n  method: post\n  operationId: fetch_search_fetch_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{full_path}\n  method: post\n  operationId: proxy_request__full_path__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/libertai/refs/heads/main/agentic-access/libertai-agentic-access.yml
summary_line: 9 operations · 2 acting
tags:
- Company
- Artificial Intelligence
- Inference
- Model Routing
- OpenAI-Compatible
- Decentralized
- Confidential Computing
- x402
---
