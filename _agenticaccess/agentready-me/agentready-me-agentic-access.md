---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 2
api_specs:
- filename: agentready-me-commerce-api-openapi.yml
  format: yaml
  label: AgentReady.me Commerce API
  slug: agentready-me-commerce-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentready-me/openapi/agentready-me-commerce-api-openapi.yml
- filename: agentready-me-diagnostics-api-openapi.yml
  format: yaml
  label: AgentReady.me Diagnostics API
  slug: agentready-me-diagnostics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentready-me/openapi/agentready-me-diagnostics-api-openapi.yml
- filename: agentready-me-scans-api-openapi.yml
  format: yaml
  label: AgentReady.me Scans API
  slug: agentready-me-scans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentready-me/openapi/agentready-me-scans-api-openapi.yml
consequence_counts:
  read: 2
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Agentready Me Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'AgentReady.me exposes 9 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AgentReady.me
provider_slug: agentready-me
slug: agentready-me-agentic-access
source_filename: agentready-me-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/agentready-me-openapi.json, openapi/agentready-me.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    acting: 7\n    connected: 2\n  by_consequence:\n    write: 7\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/scan\n  method: post\n  operationId: scanPublicUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/scan\n  method: post\n  operationId: scanPublicUrlCompatibilityAlias\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/scan\n  method: post\n  operationId: scanPublicUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/scan\n  method: post\n  operationId: scanPublicUrlCompatibilityAlias\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/tools/crawler-access\n  method:\
  \ post\n  operationId: checkDeclaredCrawlerAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/tools/openapi-readiness\n  method: post\n  operationId: auditOpenApiAgentReadiness\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/tools/a2a-agent-card\n  method: post\n  operationId: validateA2aAgentCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/checkout\n  method: get\n  operationId: getCheckoutAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/report\n  method: get\n  operationId: getPublicReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/agentready-me/agentic-access/agentready-me-agentic-access.yml
summary_line: 9 operations · 7 acting
tags:
- Artificial Intelligence
- Agent Readiness
- WebAudit
- SEO
- Platform
---
