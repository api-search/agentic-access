---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 13
api_specs:
- filename: agentik-cc-discover-api-openapi.yml
  format: yaml
  label: Agentik Discover API
  slug: agentik-cc-discover-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentik-cc/openapi/agentik-cc-discover-api-openapi.yml
- filename: agentik-cc-oauth-api-openapi.yml
  format: yaml
  label: Agentik OAuth API
  slug: agentik-cc-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentik-cc/openapi/agentik-cc-oauth-api-openapi.yml
- filename: agentik-cc-run-api-openapi.yml
  format: yaml
  label: Agentik Run API
  slug: agentik-cc-run-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentik-cc/openapi/agentik-cc-run-api-openapi.yml
- filename: agentik-cc-wallet-api-openapi.yml
  format: yaml
  label: Agentik Wallet API
  slug: agentik-cc-wallet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentik-cc/openapi/agentik-cc-wallet-api-openapi.yml
consequence_counts:
  read: 13
  safety-critical: 1
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Agentik Cc Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /oauth/revoke
operation_count: 20
overview: 'Agentik exposes 20 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read, 6 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Agentik
provider_slug: agentik-cc
slug: agentik-cc-agentic-access
source_filename: agentik-cc-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/agentik-cc-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    connected: 13\n    acting: 7\n  by_consequence:\n    read: 13\n    write: 6\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /v1/agent-info\n  method: get\n  operationId: getAgentInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connect.md\n  method: get\n  operationId: get_connect_md\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/discover\n\
  \  method: post\n  operationId: discoverTools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tools\n  method: get\n  operationId: listTools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tools/reliability\n  method: get\n  operationId: get_v1_tools_reliability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tools/{provider}/{tool}\n  method: get\n  operationId: inspectTool\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/run\n  method: post\n  operationId: runTool\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/runs/{id}\n  method: get\n  operationId: getRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/keys/me\n  method: get\n  operationId: get_v1_keys_me\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/wallet/balance\n  method: get\n  operationId: get_v1_wallet_balance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/topups\n  method: post\n  operationId: post_v1_topups\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/topups/{id}\n  method: get\n  operationId: get_v1_topups_by_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp\n  method: post\n  operationId: post_mcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - run\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/public\n  method: post\n  operationId: post_mcp_public\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /.well-known/oauth-protected-resource/mcp\n  method: get\n  operationId: get_well_known_oauth_protected_resource_mcp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-protected-resource\n  method: get\n  operationId: get_well_known_oauth_protected_resource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-authorization-server\n  method: get\n  operationId: get_well_known_oauth_authorization_server\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/register\n  method: post\n  operationId: post_oauth_register\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/token\n  method: post\n  operationId: post_oauth_token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/revoke\n  method: post\n  operationId: post_oauth_revoke\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/agentik-cc/agentic-access/agentik-cc-agentic-access.yml
summary_line: 20 operations · 7 acting · 1 human-in-the-loop
tags:
- Artificial Intelligence
- Automation
- Tools
- MCP
- Software-as-a-Service
---
