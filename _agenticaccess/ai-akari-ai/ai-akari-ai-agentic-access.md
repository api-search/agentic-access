---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 8
api_specs:
- filename: ai-akari-ai-a2a-api-openapi.yml
  format: yaml
  label: ai-akari-ai A2A API
  slug: ai-akari-ai-a2a-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ai-akari-ai/openapi/ai-akari-ai-a2a-api-openapi.yml
- filename: ai-akari-ai-mcp-api-openapi.yml
  format: yaml
  label: ai-akari-ai MCP API
  slug: ai-akari-ai-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ai-akari-ai/openapi/ai-akari-ai-mcp-api-openapi.yml
- filename: ai-akari-ai-public-support-api-openapi.yml
  format: yaml
  label: ai-akari-ai Public support API
  slug: ai-akari-ai-public-support-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ai-akari-ai/openapi/ai-akari-ai-public-support-api-openapi.yml
- filename: ai-akari-ai-trust-api-openapi.yml
  format: yaml
  label: ai-akari-ai Trust API
  slug: ai-akari-ai-trust-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ai-akari-ai/openapi/ai-akari-ai-trust-api-openapi.yml
- filename: ai-akari-ai-x402-api-openapi.yml
  format: yaml
  label: ai-akari-ai X402 API
  slug: ai-akari-ai-x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ai-akari-ai/openapi/ai-akari-ai-x402-api-openapi.yml
consequence_counts:
  physical: 1
  read: 8
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ai Akari Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/x402/agent-market-pulse
operation_count: 13
overview: 'ai-akari-ai exposes 13 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 4 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ai-akari-ai
provider_slug: ai-akari-ai
slug: ai-akari-ai-agentic-access
source_filename: ai-akari-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/ai-akari-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 8\n    acting: 5\n  by_consequence:\n    read: 8\n    write: 4\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/one-minute\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp-trust\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp-trust\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /.well-known/agent-trust.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/x402/result-claim-audit\n  method: get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/x402/result-claim-audit\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/x402/happiness-first-decision\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/x402/philosophy\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /a2a/result-receipt-auditor\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/x402/agent-market-pulse\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/x402/agent-market-pulse\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/ai-akari-ai/agentic-access/ai-akari-ai-agentic-access.yml
summary_line: 13 operations · 5 acting
tags:
- Artificial Intelligence
- Music
- DigitalTown
- Community
- Japanese
---
