---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 4
api_specs:
- filename: paidsync-ai-billing-api-openapi.yml
  format: yaml
  label: paidsync-ai Billing API
  slug: paidsync-ai-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paidsync-ai/openapi/paidsync-ai-billing-api-openapi.yml
- filename: paidsync-ai-mcp-api-openapi.yml
  format: yaml
  label: paidsync-ai MCP API
  slug: paidsync-ai-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paidsync-ai/openapi/paidsync-ai-mcp-api-openapi.yml
- filename: paidsync-ai-paidsync-api-api-openapi.yml
  format: yaml
  label: paidsync-ai PaidSync API
  slug: paidsync-ai-paidsync-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paidsync-ai/openapi/paidsync-ai-paidsync-api-api-openapi.yml
- filename: paidsync-ai-payment-api-openapi.yml
  format: yaml
  label: paidsync-ai Payment API
  slug: paidsync-ai-payment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paidsync-ai/openapi/paidsync-ai-payment-api-openapi.yml
- filename: paidsync-ai-subscribe-api-openapi.yml
  format: yaml
  label: paidsync-ai Subscribe API
  slug: paidsync-ai-subscribe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paidsync-ai/openapi/paidsync-ai-subscribe-api-openapi.yml
consequence_counts:
  read: 4
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Paidsync Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'paidsync-ai exposes 5 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: paidsync-ai
provider_slug: paidsync-ai
slug: paidsync-ai-agentic-access
source_filename: paidsync-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/paidsync-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 4\n    acting: 1\n  by_consequence:\n    read: 4\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /mcp\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - ads\n- path: /api/subscribe\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n    scope:\n    - ads\n- path: /api/v1\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - ads\n- path: /payment\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - ads\n- path: /billing\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - ads\n"
source_yaml_url: https://artifacts.apis.io/paidsync-ai/agentic-access/paidsync-ai-agentic-access.yml
summary_line: 5 operations · 1 acting
tags:
- Company
- Artificial Intelligence
- Advertising
- Automation
- Marketing
---
