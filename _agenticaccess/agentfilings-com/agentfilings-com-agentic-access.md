---
acting_count: 0
action_class_counts:
  connected: 5
api_specs:
- filename: agentfilings-com-earnings-api-openapi.yml
  format: yaml
  label: AgentFilings Earnings API
  slug: agentfilings-com-earnings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentfilings-com/openapi/agentfilings-com-earnings-api-openapi.yml
- filename: agentfilings-com-filings-api-openapi.yml
  format: yaml
  label: AgentFilings Filings API
  slug: agentfilings-com-filings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentfilings-com/openapi/agentfilings-com-filings-api-openapi.yml
- filename: agentfilings-com-health-api-openapi.yml
  format: yaml
  label: AgentFilings Health API
  slug: agentfilings-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentfilings-com/openapi/agentfilings-com-health-api-openapi.yml
- filename: agentfilings-com-insiders-api-openapi.yml
  format: yaml
  label: AgentFilings Insiders API
  slug: agentfilings-com-insiders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentfilings-com/openapi/agentfilings-com-insiders-api-openapi.yml
- filename: agentfilings-com-probe-api-openapi.yml
  format: yaml
  label: AgentFilings Probe API
  slug: agentfilings-com-probe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentfilings-com/openapi/agentfilings-com-probe-api-openapi.yml
consequence_counts:
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Agentfilings Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'AgentFilings exposes 5 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AgentFilings
provider_slug: agentfilings-com
slug: agentfilings-com-agentic-access
source_filename: agentfilings-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/agentfilings-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 5\n  by_consequence:\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /health\n  method: get\n  operationId: health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /probe\n  method: get\n  operationId: probe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /filings/latest\n  method: get\n  operationId: filings_latest\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /earnings/summary\n  method: get\n  operationId: earnings_summary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insiders\n  method: get\n  operationId: insiders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/agentfilings-com/agentic-access/agentfilings-com-agentic-access.yml
summary_line: 5 operations
tags:
- SEC
- EDGAR
- Finance
- Artificial Intelligence
- Data
- Filings
---
