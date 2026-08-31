---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 24
api_specs:
- filename: monid-api-keys-api-openapi.yml
  format: yaml
  label: Monid API Keys API
  slug: monid-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monid/refs/heads/main/openapi/monid-api-keys-api-openapi.yml
- filename: monid-auth-api-openapi.yml
  format: yaml
  label: Monid Auth API
  slug: monid-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monid/refs/heads/main/openapi/monid-auth-api-openapi.yml
- filename: monid-controls-api-openapi.yml
  format: yaml
  label: Monid Controls API
  slug: monid-controls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monid/refs/heads/main/openapi/monid-controls-api-openapi.yml
- filename: monid-discover-api-openapi.yml
  format: yaml
  label: Monid Discover API
  slug: monid-discover-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monid/refs/heads/main/openapi/monid-discover-api-openapi.yml
- filename: monid-endpoints-api-openapi.yml
  format: yaml
  label: Monid Endpoints API
  slug: monid-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monid/refs/heads/main/openapi/monid-endpoints-api-openapi.yml
- filename: monid-inspect-api-openapi.yml
  format: yaml
  label: Monid Inspect API
  slug: monid-inspect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monid/refs/heads/main/openapi/monid-inspect-api-openapi.yml
- filename: monid-public-registry-api-openapi.yml
  format: yaml
  label: Monid Public Registry API
  slug: monid-public-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monid/refs/heads/main/openapi/monid-public-registry-api-openapi.yml
- filename: monid-resources-api-openapi.yml
  format: yaml
  label: Monid Resources API
  slug: monid-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monid/refs/heads/main/openapi/monid-resources-api-openapi.yml
- filename: monid-runs-api-openapi.yml
  format: yaml
  label: Monid Runs API
  slug: monid-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monid/refs/heads/main/openapi/monid-runs-api-openapi.yml
- filename: monid-wallet-api-openapi.yml
  format: yaml
  label: Monid Wallet API
  slug: monid-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monid/refs/heads/main/openapi/monid-wallet-api-openapi.yml
consequence_counts:
  read: 24
  safety-critical: 3
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Monid Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/controls/workspace/budgets/{budgetControlId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/controls/workspace/run-caps/{runCapControlId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/runs/{runId}/stop
operation_count: 33
overview: 'Monid exposes 33 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 24 read, 6 write, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Monid
provider_slug: monid
slug: monid-agentic-access
source_filename: monid-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: generated\nsource: openapi/monid-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 33\n  by_action_class:\n    connected: 24\n    acting: 9\n  by_consequence:\n    read: 24\n    write: 6\n    safety-critical: 3\n  human_in_the_loop_required: 3\noperations:\n- path: /v1/auth/whoami\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/auth/workspaces\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/discover\n  method: post\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/endpoints\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/inspect\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/run\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/runs\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/runs/{runId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/runs/{runId}/controls\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/runs/{runId}/stop\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/resources\n  method: get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/resources/{resourceId}/external/{kind}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/resources/{resourceId}/events\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/resources/{resourceId}/release\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/resources/{resourceId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/wallet/balance\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/wallet/topup\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/controls/workspace/budgets\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/controls/workspace/budgets/{budgetControlId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/controls/workspace/budgets/{budgetControlId}\n  method: patch\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/controls/workspace/budgets/{budgetControlId}/runs\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/controls/workspace/run-caps\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/controls/workspace/run-caps/{runCapControlId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/controls/workspace/run-caps/{runCapControlId}\n  method: patch\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/controls/workspace/run-caps/{runCapControlId}/runs\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api-keys\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api-keys/{label}\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/api-keys/{label}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v1/stats\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v1/providers\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v1/providers/{provider}/endpoints\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v1/search\n  method: get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v1/providers/{provider}/endpoints/{endpoint}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monid/refs/heads/main/agentic-access/monid-agentic-access.yml
summary_line: 33 operations · 9 acting · 3 human-in-the-loop
tags:
- Company
- Agents
- MCP
- Tools
- Data
- API Marketplace
---
