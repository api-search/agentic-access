---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 2
api_specs:
- filename: automation-preflight-api-acceptance-pack-api-openapi.yml
  format: yaml
  label: Automation Preflight API Acceptance Pack API
  slug: automation-preflight-api-acceptance-pack-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automation-preflight-api/refs/heads/main/openapi/automation-preflight-api-acceptance-pack-api-openapi.yml
- filename: automation-preflight-api-analyze-api-openapi.yml
  format: yaml
  label: Automation Preflight API Analyze API
  slug: automation-preflight-api-analyze-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automation-preflight-api/refs/heads/main/openapi/automation-preflight-api-analyze-api-openapi.yml
- filename: automation-preflight-api-direct-api-openapi.yml
  format: yaml
  label: Automation Preflight API Direct API
  slug: automation-preflight-api-direct-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automation-preflight-api/refs/heads/main/openapi/automation-preflight-api-direct-api-openapi.yml
- filename: automation-preflight-api-health-api-openapi.yml
  format: yaml
  label: Automation Preflight API Health API
  slug: automation-preflight-api-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automation-preflight-api/refs/heads/main/openapi/automation-preflight-api-health-api-openapi.yml
consequence_counts:
  read: 2
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Automation Preflight Api Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Automation Preflight API exposes 5 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Automation Preflight API
provider_slug: automation-preflight-api
slug: automation-preflight-api-agentic-access
source_filename: automation-preflight-api-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: generated\nsource: openapi/automation-preflight-api-direct-openapi.json, openapi/automation-preflight-api-preflight-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    acting: 3\n    connected: 2\n  by_consequence:\n    write: 3\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /direct/analyze\n  method: post\n  operationId: analyzeIntegrationReadiness\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /health\n  method: get\n\
  \  operationId: health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analyze\n  method: post\n  operationId: analyzeIntegrationReadiness\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /acceptance-pack\n  method: post\n  operationId: buildAutomationAcceptancePack\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /health\n  method: get\n  operationId: health\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/automation-preflight-api/refs/heads/main/agentic-access/automation-preflight-api-agentic-access.yml
summary_line: 5 operations · 3 acting
tags:
- automation
- integration
- Developer Tools
- readiness
- Testing
- url-analysis
- Web Scraping
- agent-tools
- quality-assurance
- site-audit
---
