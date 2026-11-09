---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 3
api_specs:
- filename: agentrapay-ai-agents-api-openapi.yml
  format: yaml
  label: Agentra Agents API
  slug: agentrapay-ai-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentrapay-ai/openapi/agentrapay-ai-agents-api-openapi.yml
- filename: agentrapay-ai-authorizations-api-openapi.yml
  format: yaml
  label: Agentra Authorizations API
  slug: agentrapay-ai-authorizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentrapay-ai/openapi/agentrapay-ai-authorizations-api-openapi.yml
- filename: agentrapay-ai-health-api-openapi.yml
  format: yaml
  label: Agentra Health API
  slug: agentrapay-ai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentrapay-ai/openapi/agentrapay-ai-health-api-openapi.yml
- filename: agentrapay-ai-trust-api-openapi.yml
  format: yaml
  label: Agentra Trust API
  slug: agentrapay-ai-trust-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentrapay-ai/openapi/agentrapay-ai-trust-api-openapi.yml
- filename: agentrapay-ai-wallets-api-openapi.yml
  format: yaml
  label: Agentra Wallets API
  slug: agentrapay-ai-wallets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentrapay-ai/openapi/agentrapay-ai-wallets-api-openapi.yml
consequence_counts:
  physical: 2
  read: 3
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Agentrapay Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/authorizations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/wallets/provision
operation_count: 7
overview: 'Agentra exposes 7 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read, 2 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Agentra
provider_slug: agentrapay-ai
slug: agentrapay-ai-agentic-access
source_filename: agentrapay-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/agentrapay-ai-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 3\n    acting: 4\n  by_consequence:\n    read: 3\n    write: 2\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agents/register\n  method: post\n  operationId: registerAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agents/{agent_id}\n  method: get\n  operationId: getAgent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/wallets/provision\n  method: post\n  operationId: provisionWallet\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/trust/{agent_id}\n  method: get\n  operationId: getTrustScore\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/authorizations\n  method: post\n  operationId: createAuthorization\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/authorizations/{authorization_id}/settle\n  method: post\n  operationId: settleAuthorization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/agentrapay-ai/agentic-access/agentrapay-ai-agentic-access.yml
summary_line: 7 operations · 4 acting
tags:
- Identity Verification
- Reputation Scoring
- Transaction Authorization
- Non‑Custodial Wallet
- Agent Infrastructure
---
