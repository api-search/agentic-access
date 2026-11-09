---
acting_count: 0
action_class_counts:
  connected: 5
api_specs:
- filename: deskfeed-dev-bsc-alerts-api-openapi.yml
  format: yaml
  label: deskfeed Bsc Alerts API
  slug: deskfeed-dev-bsc-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskfeed-dev/openapi/deskfeed-dev-bsc-alerts-api-openapi.yml
- filename: deskfeed-dev-bsc-pool-autopsy-api-openapi.yml
  format: yaml
  label: deskfeed Bsc Pool Autopsy API
  slug: deskfeed-dev-bsc-pool-autopsy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskfeed-dev/openapi/deskfeed-dev-bsc-pool-autopsy-api-openapi.yml
- filename: deskfeed-dev-bsc-verdict-api-openapi.yml
  format: yaml
  label: deskfeed Bsc Verdict API
  slug: deskfeed-dev-bsc-verdict-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskfeed-dev/openapi/deskfeed-dev-bsc-verdict-api-openapi.yml
- filename: deskfeed-dev-events-api-openapi.yml
  format: yaml
  label: deskfeed Events API
  slug: deskfeed-dev-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskfeed-dev/openapi/deskfeed-dev-events-api-openapi.yml
- filename: deskfeed-dev-market-state-api-openapi.yml
  format: yaml
  label: deskfeed Market State API
  slug: deskfeed-dev-market-state-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deskfeed-dev/openapi/deskfeed-dev-market-state-api-openapi.yml
consequence_counts:
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Deskfeed Dev Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'deskfeed exposes 5 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: deskfeed
provider_slug: deskfeed-dev
slug: deskfeed-dev-agentic-access
source_filename: deskfeed-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/deskfeed-dev-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 5\n  by_consequence:\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/market-state\n  method: get\n  operationId: market-state\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/events\n  method: get\n  operationId: event-facts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bsc-alerts\n  method: get\n  operationId: bsc-alerts\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bsc-verdict\n  method: get\n  operationId: bsc-verdict\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bsc-pool-autopsy\n  method: get\n  operationId: bsc-pool-autopsy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/deskfeed-dev/agentic-access/deskfeed-dev-agentic-access.yml
summary_line: 5 operations
tags:
- Artificial Intelligence
- Autonomous Agents
- Data Services
- Blockchain
- Open Source
---
