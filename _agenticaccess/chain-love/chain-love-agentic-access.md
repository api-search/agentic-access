---
acting_count: 0
action_class_counts:
  connected: 5
api_specs:
- filename: chain-love-ai-context-api-openapi.yml
  format: yaml
  label: Chain.Love AI Context API
  slug: chain-love-ai-context-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chain-love/openapi/chain-love-ai-context-api-openapi.yml
- filename: chain-love-discovery-api-openapi.yml
  format: yaml
  label: Chain.Love Discovery API
  slug: chain-love-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chain-love/openapi/chain-love-discovery-api-openapi.yml
consequence_counts:
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Chain Love Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Chain.Love exposes 5 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Chain.Love
provider_slug: chain-love
slug: chain-love-agentic-access
source_filename: chain-love-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/chain-love-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 5\n  by_consequence:\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /api/networks\n  method: get\n  operationId: listNetworks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms.txt\n  method: get\n  operationId: getLlmsText\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms-full.txt\n  method: get\n  operationId: getLlmsFullText\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp-gateway\n  method: get\n  operationId: readMcpGatewayPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /about\n  method: get\n  operationId: readAboutPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/chain-love/agentic-access/chain-love-agentic-access.yml
summary_line: 5 operations
tags:
- Web3 Infrastructure
- RPC
- Indexing
- Oracle
- Bridge
- Developer Tools
- Marketplace
---
