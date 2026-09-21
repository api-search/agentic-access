---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 11
api_specs:
- filename: broke2builtai-com-skills-openapi.json
  format: json
  label: broke2built Agent Skills API
  slug: broke2builtai-com-agent-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/broke2builtai-com/refs/heads/main/openapi/broke2builtai-com-skills-openapi.json
- filename: broke2builtai-com-zero-openapi.json
  format: json
  label: ZERO autonomous agent analysis API
  slug: broke2builtai-com-zero-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/broke2builtai-com/refs/heads/main/openapi/broke2builtai-com-zero-openapi.json
consequence_counts:
  read: 11
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Broke2Builtai Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'broke2built exposes 13 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: broke2built
provider_slug: broke2builtai-com
slug: broke2builtai-com-agentic-access
source_filename: broke2builtai-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: generated\nsource: openapi/broke2builtai-com-skills-openapi.json, openapi/broke2builtai-com-zero-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    acting: 2\n    connected: 11\n  by_consequence:\n    write: 2\n    read: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /video\n  method: post\n  operationId: renderVideo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /video/{id}\n  method: get\n  operationId: getVideo\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /watch\n  method: post\n  operationId: createWatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /watch/{id}\n  method: get\n  operationId: getWatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /source-verify\n  method: get\n  operationId: sourceVerify\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vies-check\n  method: get\n  operationId: viesCheck\n  x-agentic-access:\n    action-class: connected\n   \
  \ consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resolver-allowlist\n  method: get\n  operationId: getResolverAllowlist\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/contract-audit\n  method: get\n  operationId: contract_audit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/wallet-brief\n  method: get\n  operationId: wallet_brief\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/payout-oracle\n  method: get\n  operationId: payout_oracle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/interface-xray\n\
  \  method: get\n  operationId: interface_xray\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/payer-census\n  method: get\n  operationId: payer_census\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/buy-zero\n  method: get\n  operationId: buy_zero\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/broke2builtai-com/refs/heads/main/agentic-access/broke2builtai-com-agentic-access.yml
summary_line: 13 operations · 2 acting
tags:
- Company
- AI Agents
- Agent Tools
- Data Intelligence
- Domain Intelligence
- Email Verification
- DNS
- SEO
- Web Audits
- Content Extraction
- Blockchain
- EVM
- Base
- Solana
- x402
- Agent Payments
- A2A
- MCP
- Autonomous Agents
- Agent Networks
- Video Generation
- Monitoring
---
