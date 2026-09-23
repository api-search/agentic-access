---
acting_count: 0
action_class_counts:
  connected: 5
api_specs:
- filename: newminecraftservers-openapi.yml
  format: yaml
  label: NewMinecraftServers API
  slug: newminecraftservers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newminecraftservers/refs/heads/main/openapi/newminecraftservers-openapi.yml
consequence_counts:
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Newminecraftservers Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'NewMinecraftServers exposes 5 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: NewMinecraftServers
provider_slug: newminecraftservers
slug: newminecraftservers-agentic-access
source_filename: newminecraftservers-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-21'\nmethod: generated\nsource: openapi/newminecraftservers-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 5\n  by_consequence:\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /servers\n  method: get\n  operationId: listServers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /servers/lookup\n  method: get\n  operationId: lookupServerByAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /servers/{slug}\n  method: get\n  operationId: getServerBySlug\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /servers/{slug}/history\n  method: get\n  operationId: getPublicServerHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /minecraft-status\n  method: get\n  operationId: getMinecraftServiceStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/newminecraftservers/refs/heads/main/agentic-access/newminecraftservers-agentic-access.yml
summary_line: 5 operations
tags:
- Minecraft
- Gaming
- server-directory
- Game Servers
- status-monitoring
- Public APIs
- Read Only
- JSON
---
