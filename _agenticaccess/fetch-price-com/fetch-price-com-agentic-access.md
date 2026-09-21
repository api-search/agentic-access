---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 3
api_specs:
- filename: fetch-price-com-openapi.yml
  format: yaml
  label: fetch-price API
  slug: fetch-price-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fetch-price-com/refs/heads/main/openapi/fetch-price-com-openapi.yml
consequence_counts:
  read: 3
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: searched
name: Fetch Price Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'POLICYANDPLAY LTD exposes 4 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: POLICYANDPLAY LTD
provider_slug: fetch-price-com
slug: fetch-price-com-agentic-access
source_filename: fetch-price-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/fetch-price-com-openapi.yml, curated against https://fetch-price.com/docs/, the provider SKILL.md\n  and mcp/fetch_price_mcp.py\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance\n  starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    acting: 1\n    connected: 3\n  by_consequence:\n    write: 1\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /api/query\n  method: post\n  operationId: queryProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    audience: null\n    token:\n      max-ttl: 3600\n    escalation:\n      human-in-the-loop: none\n      triggers: []\n    audit: recommended\n    note: Spends one lookup of the plan quota per call; the only\
  \ side effect. Results may contain affiliate-tracked\n      URLs the provider asks the agent to disclose to the human.\n- path: /api/agents/register\n  method: post\n  operationId: registerAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/stats\n  method: get\n  operationId: getStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\ncuration_note: 'Heuristic output reclassified queryProducts: it is a POST but semantically a read - a marketplace\n \
  \ search that persists nothing for the caller, places no order and moves no money (the buy URL is handed to a human).\n  The provider describes both agent-facing skills as search and a \"read-only health check\". registerAgent stays\n  acting/write (creates an account and a key). audience left null to bind per deployment.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fetch-price-com/refs/heads/main/agentic-access/fetch-price-com-agentic-access.yml
summary_line: 4 operations · 1 acting
tags:
- Company
- Price Comparison
- Product Search
- E-Commerce
- Affiliates
- Marketplace
- Shopping
- eBay
- United Kingdom
- AI Agents
- A2A
- MCP
---
