---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 7
api_specs:
- filename: plyrium-com-vouchspec-openapi.yml
  format: yaml
  label: VouchSpec Agent Skill Evidence API
  slug: vouchspec-agent-skill-evidence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plyrium-com/refs/heads/main/openapi/plyrium-com-vouchspec-openapi.yml
consequence_counts:
  read: 7
  safety-critical: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Plyrium Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/vouchspec/v1/validate
operation_count: 8
overview: 'Plyrium exposes 8 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Plyrium
provider_slug: plyrium-com
slug: plyrium-com-agentic-access
source_filename: plyrium-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: generated\nsource: openapi/plyrium-com-vouchspec-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 7\n    acting: 1\n  by_consequence:\n    read: 7\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /api/vouchspec/v1/health\n  method: get\n  operationId: getVouchSpecHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/vouchspec/v1/discovery\n  method: get\n  operationId: getVouchSpecDiscovery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n \
  \   audit: none\n- path: /.well-known/x402\n  method: get\n  operationId: getVouchSpecX402Manifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/vouchspec/v1/validate\n  method: get\n  operationId: getVouchSpecValidationService\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/vouchspec/v1/validate\n  method: post\n  operationId: purchaseExactCommitValidation\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/vouchspec/v1/keys/issuer\n  method: get\n  operationId: getVouchSpecIssuerKey\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/vouchspec/v1/receipts/{sha256_hex}\n  method: get\n  operationId: getVouchSpecReceipt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/vouchspec/v1/receipts/{sha256_hex}/status\n  method: get\n  operationId: getVouchSpecReceiptStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plyrium-com/refs/heads/main/agentic-access/plyrium-com-agentic-access.yml
summary_line: 8 operations · 1 acting · 1 human-in-the-loop
tags:
- Company
- Agent Skills
- Supply Chain Security
- Software Provenance
- x402
- Agentic Commerce
- A2A
- MCP
- Field Service
- Home Services
---
