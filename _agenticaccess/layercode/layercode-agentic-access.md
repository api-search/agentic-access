---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 4
api_specs:
- filename: layercode-openapi.yml
  format: yaml
  label: Layercode Agents API
  slug: layercode-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/layercode/refs/heads/main/openapi/layercode-openapi.yml
- filename: layercode-openapi.yml
  format: yaml
  label: Layercode Sessions API
  slug: layercode-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/layercode/refs/heads/main/openapi/layercode-openapi.yml
- filename: layercode-asyncapi.yml
  format: yaml
  label: Layercode Realtime Voice API
  slug: layercode-realtime-voice-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/layercode/refs/heads/main/asyncapi/layercode-asyncapi.yml
- filename: layercode-asyncapi.yml
  format: yaml
  label: Layercode Webhooks API
  slug: layercode-webhooks-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/layercode/refs/heads/main/asyncapi/layercode-asyncapi.yml
consequence_counts:
  read: 4
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Layercode Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Layercode exposes 8 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Layercode
provider_slug: layercode
slug: layercode-agentic-access
source_filename: layercode-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/layercode-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 4\n    acting: 4\n  by_consequence:\n    read: 4\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /agents\n  method: get\n  operationId: listAgents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents\n  method: post\n  operationId: createAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n     \
  \ triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents/{agent_id}\n  method: get\n  operationId: getAgent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/{agent_id}\n  method: post\n  operationId: updateAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents/web/authorize_session\n  method: post\n  operationId: authorizeSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /agents/{agent_id}/sessions/{session_id}\n  method: get\n  operationId: getSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/{agent_id}/sessions/{session_id}/recording\n  method: get\n  operationId: getSessionRecording\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/{agent_id}/calls/initiate_outbound\n  method: post\n  operationId: initiateOutboundCall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/layercode/refs/heads/main/agentic-access/layercode-agentic-access.yml
summary_line: 8 operations · 4 acting
tags:
- AI
- Voice
- Voice Agents
- Realtime
- Low Latency
---
