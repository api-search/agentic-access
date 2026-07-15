---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 4
api_specs:
- filename: sse
  format: yaml
  label: Neuphonic TTS SSE API
  slug: neuphonic-tts-sse-api
  spec_type: OpenAPI
  url: https://docs.neuphonic.com/api-reference/tts/sse
- filename: websocket
  format: yaml
  label: Neuphonic TTS WebSocket API
  slug: neuphonic-tts-websocket-api
  spec_type: AsyncAPI
  url: https://docs.neuphonic.com/api-reference/tts/websocket
consequence_counts:
  read: 4
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Neuphonic Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Neuphonic exposes 12 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Neuphonic
provider_slug: neuphonic
slug: neuphonic-agentic-access
source_filename: neuphonic-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/neuphonic-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 4\n    acting: 8\n  by_consequence:\n    read: 4\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /ping\n  method: get\n  operationId: ping_ping_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /voices\n  method: get\n  operationId: tts_endpoint_voices_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /voices\n  method: post\n  operationId:\
  \ clone_voice_voices_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /voices/{voice_id}\n  method: patch\n  operationId: update_voice_voices__voice_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /voices/{voice_id}\n  method: delete\n  operationId: delete_cloned_voice_voices__voice_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /sse/auth\n  method: post\n  operationId: swap_api_key_for_jwt_token_sse_auth_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sse/speak/{lang_code}\n  method: post\n  operationId: sse_generator_sse_speak__lang_code__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents\n  method: get\n  operationId: list_all_agents_agents_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n- path: /agents\n  method: post\n  operationId: create_agent_agents_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents/{agent_id}\n  method: get\n  operationId: get_agent_agents__agent_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/{agent_id}\n  method: delete\n  operationId: delete_agent_agents__agent_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /agents/{agent_id}/token\n  method: post\n  operationId: get_livekit_token_agents__agent_id__token_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neuphonic/refs/heads/main/agentic-access/neuphonic-agentic-access.yml
summary_line: 12 operations · 8 acting
tags:
- Text-to-Speech
- Voice AI
- Audio
- Streaming
- WebSocket
- Voice Cloning
- Conversational AI
- Real-Time
- Multilingual
- On-Device AI
---
