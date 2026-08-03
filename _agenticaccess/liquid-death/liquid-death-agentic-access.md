---
acting_count: 0
action_class_counts:
  connected: 7
api_specs:
- filename: liquid-death-storefront-openapi.yml
  format: yaml
  label: Liquid Death Storefront Read-Only JSON API
  slug: liquid-death-storefront-read-only-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liquid-death/refs/heads/main/openapi/liquid-death-storefront-openapi.yml
consequence_counts:
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Liquid Death Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Liquid Death exposes 7 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Liquid Death
provider_slug: liquid-death
slug: liquid-death-agentic-access
source_filename: liquid-death-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: generated\nsource: openapi/liquid-death-storefront-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 7\n  by_consequence:\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /products/{handle}.json\n  method: get\n  operationId: getProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{handle}/products.json\n  method: get\n  operationId: listCollectionProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search\n  method:\
  \ get\n  operationId: searchStorefront\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sitemap.xml\n  method: get\n  operationId: getSitemap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents.md\n  method: get\n  operationId: getAgentInstructions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms.txt\n  method: get\n  operationId: getLlmsTxt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/ucp\n  method: get\n  operationId: getUcpProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liquid-death/refs/heads/main/agentic-access/liquid-death-agentic-access.yml
summary_line: 7 operations
tags:
- Company
- Beverages
- Consumer Packaged Goods
- Direct to Consumer
- Ecommerce
- Retail
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- Shopify
---
