---
acting_count: 0
action_class_counts:
  connected: 6
api_specs:
- filename: adgentek-ai-advertiser-api-openapi.yml
  format: yaml
  label: Adgentek Advertiser API
  slug: adgentek-ai-advertiser-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adgentek-ai/openapi/adgentek-ai-advertiser-api-openapi.yml
- filename: adgentek-ai-meta-api-openapi.yml
  format: yaml
  label: Adgentek Meta API
  slug: adgentek-ai-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adgentek-ai/openapi/adgentek-ai-meta-api-openapi.yml
- filename: adgentek-ai-publisher-api-openapi.yml
  format: yaml
  label: Adgentek Publisher API
  slug: adgentek-ai-publisher-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adgentek-ai/openapi/adgentek-ai-publisher-api-openapi.yml
consequence_counts:
  read: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Adgentek Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Adgentek exposes 6 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Adgentek
provider_slug: adgentek-ai
slug: adgentek-ai-agentic-access
source_filename: adgentek-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/adgentek-ai-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 6\n  by_consequence:\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /health\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /version\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /openapi.yaml\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/advertiser/reporting/campaigns\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/publisher/reporting/overview\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/adgentek-ai/agentic-access/adgentek-ai-agentic-access.yml
summary_line: 6 operations
tags:
- Advertising
- Artificial Intelligence
- AdTech
- AI Agents
- Monetization
- Servers
---
