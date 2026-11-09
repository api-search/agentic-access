---
acting_count: 0
action_class_counts:
  connected: 8
api_specs:
- filename: pinnodds-com-drops-api-openapi.yml
  format: yaml
  label: pinnodds-com Drops API
  slug: pinnodds-com-drops-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pinnodds-com/openapi/pinnodds-com-drops-api-openapi.yml
- filename: pinnodds-com-health-api-openapi.yml
  format: yaml
  label: pinnodds-com Health API
  slug: pinnodds-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pinnodds-com/openapi/pinnodds-com-health-api-openapi.yml
- filename: pinnodds-com-kit-api-openapi.yml
  format: yaml
  label: pinnodds-com Kit API
  slug: pinnodds-com-kit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pinnodds-com/openapi/pinnodds-com-kit-api-openapi.yml
- filename: pinnodds-com-ping-api-openapi.yml
  format: yaml
  label: pinnodds-com Ping API
  slug: pinnodds-com-ping-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pinnodds-com/openapi/pinnodds-com-ping-api-openapi.yml
consequence_counts:
  read: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Pinnodds Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'pinnodds-com exposes 8 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: pinnodds-com
provider_slug: pinnodds-com
slug: pinnodds-com-agentic-access
source_filename: pinnodds-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/pinnodds-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 8\n  by_consequence:\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /kit/v1/markets\n  method: get\n  operationId: getMarkets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /kit/v1/details\n  method: get\n  operationId: getDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /kit/v1/prematch/fixtures\n  method: get\n  operationId: getPrematchFixtures\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /kit/v1/prematch/markets\n  method: get\n  operationId: getPrematchMarkets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /kit/v1/prematch/lines\n  method: get\n  operationId: getPrematchLines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/drops\n  method: get\n  operationId: getDrops\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /ping\n  method: get\n  operationId: getPing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/pinnodds-com/agentic-access/pinnodds-com-agentic-access.yml
summary_line: 8 operations
tags:
- Company
- Sports
- Odds
- Real-Time
- Pinnacle
---
