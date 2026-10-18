---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 3
api_specs:
- filename: rephraseai-actor-api-openapi.yml
  format: yaml
  label: Rephrase.ai Actor API
  slug: rephraseai-actor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rephraseai/refs/heads/main/openapi/rephraseai-actor-api-openapi.yml
- filename: rephraseai-authentication-api-openapi.yml
  format: yaml
  label: Rephrase.ai Authentication API
  slug: rephraseai-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rephraseai/refs/heads/main/openapi/rephraseai-authentication-api-openapi.yml
- filename: rephraseai-video-api-openapi.yml
  format: yaml
  label: Rephrase.ai Video API
  slug: rephraseai-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rephraseai/refs/heads/main/openapi/rephraseai-video-api-openapi.yml
- filename: rephraseai-voice-api-openapi.yml
  format: yaml
  label: Rephrase.ai Voice API
  slug: rephraseai-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rephraseai/refs/heads/main/openapi/rephraseai-voice-api-openapi.yml
consequence_counts:
  read: 3
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Rephraseai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Rephrase.ai exposes 6 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Rephrase.ai
provider_slug: rephraseai
slug: rephraseai-agentic-access
source_filename: rephraseai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/rephraseai-rephrase-studio-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    acting: 3\n    connected: 3\n  by_consequence:\n    write: 3\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /auth.rephrase.ai/oauth/token\n  method: post\n  operationId: get-access-token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /personalized-brand.api.rephrase.ai/v2/actors\n  method: get\n  operationId: get-actors\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /personalized-brand.api.rephrase.ai/v2/campaign/create\n  method: post\n  operationId: create-video\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /personalized-brand.api.rephrase.ai/v2/campaign/{campaign_id}\n  method: get\n  operationId: get-video\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /personalized-brand.api.rephrase.ai/v2/campaign/{campaign_id}/export\n  method: post\n  operationId: export-video\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /personalized-brand.api.rephrase.ai/v2/voices\n  method: get\n  operationId: get-voices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rephraseai/refs/heads/main/agentic-access/rephraseai-agentic-access.yml
summary_line: 6 operations · 3 acting
tags:
- Company
- Artificial Intelligence
- Generative AI
- Video
- Video Generation
- Avatars
- Media
- Content Creation
---
