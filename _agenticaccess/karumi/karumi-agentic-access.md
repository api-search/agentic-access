---
acting_count: 0
action_class_counts:
  connected: 9
api_specs:
- filename: karumi-analytics-api-openapi.yml
  format: yaml
  label: Karumi Analytics API
  slug: karumi-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karumi/refs/heads/main/openapi/karumi-analytics-api-openapi.yml
- filename: karumi-sessions-api-openapi.yml
  format: yaml
  label: Karumi Sessions API
  slug: karumi-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karumi/refs/heads/main/openapi/karumi-sessions-api-openapi.yml
- filename: karumi-targets-api-openapi.yml
  format: yaml
  label: Karumi Targets API
  slug: karumi-targets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karumi/refs/heads/main/openapi/karumi-targets-api-openapi.yml
consequence_counts:
  read: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Karumi Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Karumi exposes 9 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Karumi
provider_slug: karumi
slug: karumi-agentic-access
source_filename: karumi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: generated\nsource: openapi/karumi-public-api-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 9\n  by_consequence:\n    read: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /sessions\n  method: get\n  operationId: list_sessions_sessions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions/meeting-events\n  method: get\n  operationId: list_meeting_events_sessions_meeting_events_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions/{session_id}\n\
  \  method: get\n  operationId: get_session_sessions__session_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions/{session_id}/insights\n  method: get\n  operationId: get_session_insights_sessions__session_id__insights_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions/{session_id}/recording\n  method: get\n  operationId: download_session_recording_sessions__session_id__recording_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics\n  method: get\n  operationId: get_analytics_analytics_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /analytics/timeline\n  method: get\n  operationId: get_analytics_timeline_analytics_timeline_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /targets\n  method: get\n  operationId: list_targets_targets_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /targets/{target_id}\n  method: get\n  operationId: get_target_targets__target_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/karumi/refs/heads/main/agentic-access/karumi-agentic-access.yml
summary_line: 9 operations
tags:
- Company
- AI Agents
- Product Demos
- Sales Enablement
- Go-To-Market
- Software-as-a-Service
- Conversational AI
- Video
- Y Combinator
- MCP
- agent-native
- Analytics
- Conversation Intelligence
---
