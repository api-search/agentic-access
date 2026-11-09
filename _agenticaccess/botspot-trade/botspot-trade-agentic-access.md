---
acting_count: 0
action_class_counts:
  connected: 5
api_specs:
- filename: botspot-trade-llms-txt-api-openapi.yml
  format: yaml
  label: botspot-trade Llms.txt API
  slug: botspot-trade-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botspot-trade/openapi/botspot-trade-llms-txt-api-openapi.yml
- filename: botspot-trade-openapi-json-api-openapi.yml
  format: yaml
  label: botspot-trade Openapi.json API
  slug: botspot-trade-openapi-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botspot-trade/openapi/botspot-trade-openapi-json-api-openapi.yml
- filename: botspot-trade-sitemap-xml-api-openapi.yml
  format: yaml
  label: botspot-trade Sitemap.xml API
  slug: botspot-trade-sitemap-xml-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botspot-trade/openapi/botspot-trade-sitemap-xml-api-openapi.yml
- filename: botspot-trade-well-known-api-openapi.yml
  format: yaml
  label: botspot-trade .well Known API
  slug: botspot-trade-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botspot-trade/openapi/botspot-trade-well-known-api-openapi.yml
consequence_counts:
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Botspot Trade Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'botspot-trade exposes 5 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: botspot-trade
provider_slug: botspot-trade
slug: botspot-trade-agentic-access
source_filename: botspot-trade-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/botspot-trade-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 5\n  by_consequence:\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /.well-known/botspot-manifest.json\n  method: get\n  operationId: getBotspotManifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms.txt\n  method: get\n  operationId: getBotspotAgentIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sitemap.xml\n  method: get\n  operationId:\
  \ getBotspotSitemap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi.json\n  method: get\n  operationId: getBotspotOpenapiDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/mcp\n  method: get\n  operationId: discoverBotspotMcpServer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/botspot-trade/agentic-access/botspot-trade-agentic-access.yml
summary_line: 5 operations
tags:
- AI Trading
- Bot Builder
- Backtesting
- Trading Platform
---
