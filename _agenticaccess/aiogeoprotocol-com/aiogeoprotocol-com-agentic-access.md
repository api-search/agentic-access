---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 2
api_specs:
- filename: aiogeoprotocol-com-audit-api-openapi.yml
  format: yaml
  label: AIO.GEO Protocol Audit API
  slug: aiogeoprotocol-com-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiogeoprotocol-com/openapi/aiogeoprotocol-com-audit-api-openapi.yml
- filename: aiogeoprotocol-com-brief-api-openapi.yml
  format: yaml
  label: AIO.GEO Protocol Brief API
  slug: aiogeoprotocol-com-brief-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiogeoprotocol-com/openapi/aiogeoprotocol-com-brief-api-openapi.yml
consequence_counts:
  read: 2
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Aiogeoprotocol Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'AIO.GEO Protocol exposes 5 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AIO.GEO Protocol
provider_slug: aiogeoprotocol-com
slug: aiogeoprotocol-com-agentic-access
source_filename: aiogeoprotocol-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/aiogeoprotocol-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    acting: 3\n    connected: 2\n  by_consequence:\n    write: 3\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/public/audit\n  method: post\n  operationId: publicAudit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/public/brief\n  method: post\n  operationId: publicExecutiveBrief\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/public/brief\n  method: get\n  operationId: publicBriefHelp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/public/wall\n  method: get\n  operationId: firstHtmlWall\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/public/wall\n  method: post\n  operationId: pinFirstHtmlReceipt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/aiogeoprotocol-com/agentic-access/aiogeoprotocol-com-agentic-access.yml
summary_line: 5 operations · 3 acting
tags:
- Company
- Artificial Intelligence
- Search
- Audit
- Measurements
- CLI
---
