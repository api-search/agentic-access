---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 3
api_specs:
- filename: drivings-com-discovery-api-openapi.yml
  format: yaml
  label: Drivings Discovery API
  slug: drivings-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drivings-com/openapi/drivings-com-discovery-api-openapi.yml
- filename: drivings-com-planning-api-openapi.yml
  format: yaml
  label: Drivings Planning API
  slug: drivings-com-planning-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drivings-com/openapi/drivings-com-planning-api-openapi.yml
consequence_counts:
  read: 3
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Drivings Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'Drivings exposes 4 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Drivings
provider_slug: drivings-com
slug: drivings-com-agentic-access
source_filename: drivings-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: generated\nsource: openapi/drivings-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    connected: 3\n    acting: 1\n  by_consequence:\n    read: 3\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/agent/v1/capabilities\n  method: get\n  operationId: getAgentCapabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent/v1/courses\n  method: get\n  operationId: listStudyOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent/v1/test-centres\n\
  \  method: get\n  operationId: findTestCentres\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent/v1/study-plan\n  method: post\n  operationId: buildStudyPlanPreview\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/drivings-com/agentic-access/drivings-com-agentic-access.yml
summary_line: 4 operations · 1 acting
tags:
- Company
- Driving
- Education
- United Kingdom
- US
---
