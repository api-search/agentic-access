---
acting_count: 9
action_class_counts:
  acting: 9
api_specs:
- filename: x402supply-com-chess-eval-api-openapi.yml
  format: yaml
  label: x402supply-com Chess Eval API
  slug: x402supply-com-chess-eval-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/x402supply-com/openapi/x402supply-com-chess-eval-api-openapi.yml
- filename: x402supply-com-endpoint-diligence-api-openapi.yml
  format: yaml
  label: x402supply-com Endpoint Diligence API
  slug: x402supply-com-endpoint-diligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/x402supply-com/openapi/x402supply-com-endpoint-diligence-api-openapi.yml
- filename: x402supply-com-entity-resolve-api-openapi.yml
  format: yaml
  label: x402supply-com Entity Resolve API
  slug: x402supply-com-entity-resolve-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/x402supply-com/openapi/x402supply-com-entity-resolve-api-openapi.yml
consequence_counts:
  physical: 1
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: X402Supply Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /tools/check_endpoint
operation_count: 9
overview: 'x402supply-com exposes 9 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 write and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: x402supply-com
provider_slug: x402supply-com
slug: x402supply-com-agentic-access
source_filename: x402supply-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/chess-eval-openapi.json, openapi/diligence-openapi.json, openapi/entity-resolve-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    acting: 9\n  by_consequence:\n    write: 8\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /mcp\n  method: post\n  operationId: chess-eval_call\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/evaluate_position\n  method: post\n  operationId: chess-eval_evaluate_position_http\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/best_line\n  method: post\n  operationId: chess-eval_best_line_http\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp\n  method: post\n  operationId: endpoint-diligence_call\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/check_endpoint\n\
  \  method: post\n  operationId: endpoint-diligence_check_endpoint_http\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/compare_price\n  method: post\n  operationId: endpoint-diligence_compare_price_http\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/reseller_check\n  method: post\n  operationId: endpoint-diligence_reseller_check_http\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n  \
  \  token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp\n  method: post\n  operationId: entity-resolve_call\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/resolve\n  method: post\n  operationId: entity-resolve_resolve_http\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/x402supply-com/agentic-access/x402supply-com-agentic-access.yml
summary_line: 9 operations · 9 acting
tags:
- Company
- Artificial Intelligence
- Pay-per-call
- Blockchain
- Tools
---
