---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 1
api_specs:
- filename: yoti-accounts-api-openapi.yml
  format: yaml
  label: Yoti Accounts API
  slug: yoti-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yoti/openapi/yoti-accounts-api-openapi.yml
- filename: yoti-ai-api-openapi.yml
  format: yaml
  label: Yoti AI API
  slug: yoti-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yoti/openapi/yoti-ai-api-openapi.yml
- filename: yoti-oauth-api-openapi.yml
  format: yaml
  label: Yoti OAuth API
  slug: yoti-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yoti/openapi/yoti-oauth-api-openapi.yml
- filename: yoti-path-api-openapi.yml
  format: yaml
  label: Yoti Path API
  slug: yoti-path-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yoti/openapi/yoti-path-api-openapi.yml
- filename: yoti-poa-api-openapi.yml
  format: yaml
  label: Yoti Poa API
  slug: yoti-poa-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yoti/openapi/yoti-poa-api-openapi.yml
- filename: yoti-sessions-api-openapi.yml
  format: yaml
  label: Yoti Sessions API
  slug: yoti-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yoti/openapi/yoti-sessions-api-openapi.yml
consequence_counts:
  read: 1
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Yoti Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Yoti exposes 7 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Yoti
provider_slug: yoti
slug: yoti-agentic-access
source_filename: yoti-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/yoti-accounts-api-openapi.yml, openapi/yoti-ai-api-openapi.yml, openapi/yoti-oauth-api-openapi.yml,\n  openapi/yoti-path-api-openapi.yml, openapi/yoti-poa-api-openapi.yml, openapi/yoti-sessions-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    acting: 6\n    connected: 1\n  by_consequence:\n    write: 6\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /accounts/{accountid}/moderations\n  method: post\n  operationId: post_accounts_accountid_moderations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - did:match\n    - poa:verify\n- path: /ai/v1/{v1id}\n  method: post\n  operationId: post_ai_v1_v1id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - did:match\n    - poa:verify\n- path: /v1/oauth/token\n  method: post\n  operationId: post_v1_oauth_token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - did:match\n    - poa:verify\n- path: /path/to/resource\n  method: post\n  operationId: post_path_to_resource\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - did:match\n    - poa:verify\n- path: /poa/v1/verify\n  method: post\n  operationId: post_poa_v1_verify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - did:match\n    - poa:verify\n- path: /api/v1/sessions\n  method: post\n  operationId: post_api_v1_sessions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - did:match\n    - poa:verify\n- path: /api/v1/sessions/{sessionid}\n  method: get\n  operationId: get_api_v1_sessions_sessionid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - did:match\n    - poa:verify\n"
source_yaml_url: https://artifacts.apis.io/yoti/agentic-access/yoti-agentic-access.yml
summary_line: 7 operations · 6 acting
tags:
- Company
- Identity
- Verification
- DigitalID
- SDK
---
