---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 3
api_specs:
- filename: wondercraft-openapi.yml
  format: yaml
  label: Wondercraft Audio Generation API
  slug: audio-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wondercraft/refs/heads/main/openapi/wondercraft-openapi.yml
- filename: wondercraft-openapi.yml
  format: yaml
  label: Wondercraft Scripted Audio API
  slug: scripted-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wondercraft/refs/heads/main/openapi/wondercraft-openapi.yml
- filename: wondercraft-openapi.yml
  format: yaml
  label: Wondercraft Convo Mode API
  slug: convo-mode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wondercraft/refs/heads/main/openapi/wondercraft-openapi.yml
- filename: wondercraft-openapi.yml
  format: yaml
  label: Wondercraft Job Status API
  slug: job-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wondercraft/refs/heads/main/openapi/wondercraft-openapi.yml
consequence_counts:
  read: 3
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Wondercraft Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Wondercraft exposes 7 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Wondercraft
provider_slug: wondercraft
slug: wondercraft-agentic-access
source_filename: wondercraft-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/wondercraft-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    acting: 4\n    connected: 3\n  by_consequence:\n    write: 4\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /podcast\n  method: post\n  operationId: generate_ai_scripted_episode_podcast_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /podcast/scripted\n  method: post\n  operationId: generate_user_scripted_episode_podcast_scripted_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /podcast/convo-mode/ai-scripted\n  method: post\n  operationId: generate_ai_scripted_convo_mode_episode_podcast_convo_mode_ai_scripted_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /podcast/convo-mode/user-scripted\n  method: post\n  operationId: generate_user_scripted_convo_mode_episode_podcast_convo_mode_user_scripted_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /podcast/{job_id}\n  method: get\n  operationId: get_episode_status_podcast__job_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /podcasts\n  method: get\n  operationId: get_podcasts_for_user_podcasts_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /verify\n  method: get\n  operationId: verify_key_verify_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wondercraft/refs/heads/main/agentic-access/wondercraft-agentic-access.yml
summary_line: 7 operations · 4 acting
tags:
- AI
- Audio
- Podcast
- Text to Speech
- Generative Audio
---
