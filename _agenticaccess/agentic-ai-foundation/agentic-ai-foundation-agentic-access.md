---
acting_count: 20
action_class_counts:
  acting: 20
  connected: 12
api_specs:
- filename: agentic-ai-foundation-auth-api-openapi.yml
  format: yaml
  label: Agentic AI Foundation Auth API
  slug: agentic-ai-foundation-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-ai-foundation/openapi/agentic-ai-foundation-auth-api-openapi.yml
- filename: agentic-ai-foundation-health-api-openapi.yml
  format: yaml
  label: Agentic AI Foundation Health API
  slug: agentic-ai-foundation-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-ai-foundation/openapi/agentic-ai-foundation-health-api-openapi.yml
- filename: agentic-ai-foundation-ping-api-openapi.yml
  format: yaml
  label: Agentic AI Foundation Ping API
  slug: agentic-ai-foundation-ping-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-ai-foundation/openapi/agentic-ai-foundation-ping-api-openapi.yml
- filename: agentic-ai-foundation-publish-api-openapi.yml
  format: yaml
  label: Agentic AI Foundation Publish API
  slug: agentic-ai-foundation-publish-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-ai-foundation/openapi/agentic-ai-foundation-publish-api-openapi.yml
- filename: agentic-ai-foundation-servers-api-openapi.yml
  format: yaml
  label: Agentic AI Foundation Servers API
  slug: agentic-ai-foundation-servers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-ai-foundation/openapi/agentic-ai-foundation-servers-api-openapi.yml
- filename: agentic-ai-foundation-validate-api-openapi.yml
  format: yaml
  label: Agentic AI Foundation Validate API
  slug: agentic-ai-foundation-validate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-ai-foundation/openapi/agentic-ai-foundation-validate-api-openapi.yml
- filename: agentic-ai-foundation-version-api-openapi.yml
  format: yaml
  label: Agentic AI Foundation Version API
  slug: agentic-ai-foundation-version-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-ai-foundation/openapi/agentic-ai-foundation-version-api-openapi.yml
consequence_counts:
  read: 12
  write: 20
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Agentic Ai Foundation Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 32
overview: 'Agentic AI Foundation exposes 32 API operations that an AI agent could call, of which 20 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read and 20 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Agentic AI Foundation
provider_slug: agentic-ai-foundation
slug: agentic-ai-foundation-agentic-access
source_filename: agentic-ai-foundation-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/agentic-ai-foundation-auth-api-openapi.yml, openapi/agentic-ai-foundation-health-api-openapi.yml,\n  openapi/agentic-ai-foundation-ping-api-openapi.yml, openapi/agentic-ai-foundation-publish-api-openapi.yml,\n  openapi/agentic-ai-foundation-servers-api-openapi.yml, openapi/agentic-ai-foundation-validate-api-openapi.yml,\n  openapi/agentic-ai-foundation-version-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 32\n  by_action_class:\n    acting: 20\n    connected: 12\n  by_consequence:\n    write: 20\n    read: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /v0.1/auth/dns\n  method: post\n  operationId: exchange-dns-token-v0.1\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.1/auth/github-at\n  method: post\n  operationId: exchange-github-token-v0.1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.1/auth/github-oidc\n  method: post\n  operationId: exchange-github-oidc-token-v0.1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.1/auth/http\n\
  \  method: post\n  operationId: exchange-http-token-v0.1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.1/auth/oidc\n  method: post\n  operationId: exchange-oidc-token-v0.1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/auth/dns\n  method: post\n  operationId: exchange-dns-token-v0\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v0/auth/github-at\n  method: post\n  operationId: exchange-github-token-v0\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/auth/github-oidc\n  method: post\n  operationId: exchange-github-oidc-token-v0\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/auth/http\n  method: post\n  operationId: exchange-http-token-v0\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n  \
  \  escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/auth/oidc\n  method: post\n  operationId: exchange-oidc-token-v0\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.1/health\n  method: get\n  operationId: get-health-v0.1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/health\n  method: get\n  operationId: get-health-v0\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/ping\n  method: get\n  operationId: ping-v0.1\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/ping\n  method: get\n  operationId: ping-v0\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/publish\n  method: post\n  operationId: publish-server-v0.1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/publish\n  method: post\n  operationId: publish-server-v0\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v0.1/servers\n  method: get\n  operationId: list-servers-v0.1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/servers/{serverName}/status\n  method: patch\n  operationId: update-server-all-versions-status-v0.1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.1/servers/{serverName}/versions\n  method: get\n  operationId: get-server-versions-v0.1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/servers/{serverName}/versions/{version}\n  method: get\n  operationId: get-server-version-v0.1\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0.1/servers/{serverName}/versions/{version}\n  method: put\n  operationId: edit-server-v0.1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.1/servers/{serverName}/versions/{version}/status\n  method: patch\n  operationId: update-server-status-v0.1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/servers\n  method: get\n  operationId: list-servers-v0\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/servers/{serverName}/status\n  method: patch\n  operationId: update-server-all-versions-status-v0\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/servers/{serverName}/versions\n  method: get\n  operationId: get-server-versions-v0\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/servers/{serverName}/versions/{version}\n  method: get\n  operationId: get-server-version-v0\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v0/servers/{serverName}/versions/{version}\n  method: put\n  operationId: edit-server-v0\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/servers/{serverName}/versions/{version}/status\n  method: patch\n  operationId: update-server-status-v0\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.1/validate\n  method: post\n  operationId: validate-server-v0.1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0/validate\n  method: post\n  operationId: validate-server-v0\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v0.1/version\n  method: get\n  operationId: get-version-v0.1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/version\n  method: get\n  operationId: get-version-v0\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/agentic-ai-foundation/agentic-access/agentic-ai-foundation-agentic-access.yml
summary_line: 32 operations · 20 acting
tags:
- AI Agents
- Linux Foundation
- Open Source
- Standards
- MCP
- Interoperability
- Agent Protocols
- A2A
- AGENTS.md
- Open Governance
---
