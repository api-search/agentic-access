---
acting_count: 0
action_class_counts:
  connected: 7
api_specs:
- filename: dealermax-app-dealerpublicapi-api-openapi.yml
  format: yaml
  label: DealerMAX Dealer Public API
  slug: dealermax-app-dealerpublicapi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealermax-app/openapi/dealermax-app-dealerpublicapi-api-openapi.yml
consequence_counts:
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Dealermax App Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'DealerMAX exposes 7 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: DealerMAX
provider_slug: dealermax-app
slug: dealermax-app-agentic-access
source_filename: dealermax-app-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/dealermax-app-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 7\n  by_consequence:\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /dealer/{service}/listing\n  method: get\n  operationId: listInventory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dealer/{service}/details\n  method: get\n  operationId: getInventoryItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dealer/{service}/quality-programs\n\
  \  method: get\n  operationId: listQualityPrograms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dealer/content/hub\n  method: get\n  operationId: getContentHub\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dealer/content/search\n  method: get\n  operationId: searchContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dealer/content/{content_type}/listing\n  method: get\n  operationId: listContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dealer/content/{content_type}/details\n  method: get\n  operationId: getContentItem\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/dealermax-app/agentic-access/dealermax-app-agentic-access.yml
summary_line: 7 operations
tags:
- Dealer Identity
- AI Visibility
- CRM
---
