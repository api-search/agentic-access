---
acting_count: 0
action_class_counts:
  connected: 9
api_specs:
- filename: asia-pulse-com-market-intelligence-api-openapi.yml
  format: yaml
  label: Asia Pulse Market Intelligence API
  slug: asia-pulse-com-market-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asia-pulse-com/openapi/asia-pulse-com-market-intelligence-api-openapi.yml
- filename: asia-pulse-com-meta-api-openapi.yml
  format: yaml
  label: Asia Pulse Meta API
  slug: asia-pulse-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asia-pulse-com/openapi/asia-pulse-com-meta-api-openapi.yml
consequence_counts:
  read: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Asia Pulse Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Asia Pulse exposes 9 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Asia Pulse
provider_slug: asia-pulse-com
slug: asia-pulse-com-agentic-access
source_filename: asia-pulse-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/asia-pulse-com-openapi.json, openapi/asia-pulse-com.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 9\n  by_consequence:\n    read: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /report\n  method: get\n  operationId: report\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /report\n  method: get\n  operationId: report\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /report/premium\n  method: get\n  operationId: report_premium\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chain/semis\n  method: get\n  operationId: chain_semis\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chain/defense\n  method: get\n  operationId: chain_defense\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chain/power\n  method: get\n  operationId: chain_power\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chain\n  method: get\n  operationId: chain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /japan\n\
  \  method: get\n  operationId: japan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/asia-pulse-com/agentic-access/asia-pulse-com-agentic-access.yml
summary_line: 9 operations
tags:
- Company
- Artificial Intelligence
- Market Intelligence
- Cryptocurrency
- Asia
---
