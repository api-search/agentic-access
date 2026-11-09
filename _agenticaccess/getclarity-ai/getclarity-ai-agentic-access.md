---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 2
api_specs:
- filename: getclarity-ai-media-statement-api-openapi.yml
  format: yaml
  label: Clarity Media Statement API
  slug: getclarity-ai-media-statement-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getclarity-ai/openapi/getclarity-ai-media-statement-api-openapi.yml
- filename: getclarity-ai-users-api-openapi.yml
  format: yaml
  label: Clarity Users API
  slug: getclarity-ai-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getclarity-ai/openapi/getclarity-ai-users-api-openapi.yml
consequence_counts:
  read: 2
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Getclarity Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'Clarity exposes 4 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Clarity
provider_slug: getclarity-ai
slug: getclarity-ai-agentic-access
source_filename: getclarity-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: generated\nsource: openapi/getclarity-ai-clarity-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    acting: 2\n    connected: 2\n  by_consequence:\n    write: 2\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /media-statement\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /media-statement\n  method: get\n  operationId: search_multicasts_v1_rest_get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /media-statement/{mcid}\n  method: get\n  operationId: get_multicast_result_v1_rest__mcid__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/token\n  method: post\n  operationId: user_login_v1_token_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/getclarity-ai/agentic-access/getclarity-ai-agentic-access.yml
summary_line: 4 operations · 2 acting
tags:
- Hiring fraud
- Identity Verification
- Deepfake Detection
- Talent acquisition security
- AI hiring security
---
