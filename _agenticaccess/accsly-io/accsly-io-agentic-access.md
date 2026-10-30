---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 13
api_specs:
- filename: accsly-io-accounts-api-openapi.yml
  format: yaml
  label: Accsly Accounts API
  slug: accsly-io-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/accsly-io/openapi/accsly-io-accounts-api-openapi.yml
- filename: accsly-io-markdown-pages-api-openapi.yml
  format: yaml
  label: Accsly Markdown pages API
  slug: accsly-io-markdown-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/accsly-io/openapi/accsly-io-markdown-pages-api-openapi.yml
- filename: accsly-io-mcp-api-openapi.yml
  format: yaml
  label: Accsly MCP API
  slug: accsly-io-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/accsly-io/openapi/accsly-io-mcp-api-openapi.yml
- filename: accsly-io-vps-api-openapi.yml
  format: yaml
  label: Accsly VPS API
  slug: accsly-io-vps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/accsly-io/openapi/accsly-io-vps-api-openapi.yml
consequence_counts:
  read: 13
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Accsly Io Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'Accsly exposes 14 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Accsly
provider_slug: accsly-io
slug: accsly-io-agentic-access
source_filename: accsly-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/accsly-io-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 13\n    acting: 1\n  by_consequence:\n    read: 13\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /{locale}/vps\n  method: get\n  operationId: searchVps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{locale}/vps/{landing}\n  method: get\n  operationId: searchVpsLanding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{locale}/vps/hosting/{slug}\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{locale}/vps/hosting/{slug}/alternatives\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{locale}/vps/rating\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{locale}/vps/rating/{slug}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{locale}/vps/compare/{pair}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{locale}/vps/prices\n  method:\
  \ get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{locale}/vps/guide/{slug}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{locale}/hosting/rating\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ru/vps/promo\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ru/vps/hosting/{slug}/promo\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search\n  method: get\n  operationId: searchAccounts\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp\n  method: post\n  operationId: mcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/accsly-io/agentic-access/accsly-io-agentic-access.yml
summary_line: 14 operations · 1 acting
tags:
- Marketplace
- Accounts
- Gaming
- AI Tools
- E-commerce
---
