---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 3
api_specs:
- filename: momentum-openapi-generated.yml
  format: yaml
  label: Momentum API
  slug: momentum-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/momentum/openapi/_ae-authored/momentum-openapi-generated.yml
- filename: momentum-meeting-api-openapi.yml
  format: yaml
  label: Momentum Meeting API
  slug: momentum-meeting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/momentum/openapi/momentum-meeting-api-openapi.yml
- filename: momentum-momentum-api-api-openapi.yml
  format: yaml
  label: Momentum Momentum API
  slug: momentum-momentum-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/momentum/openapi/momentum-momentum-api-api-openapi.yml
- filename: momentum-signals-api-openapi.yml
  format: yaml
  label: Momentum Signals API
  slug: momentum-signals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/momentum/openapi/momentum-signals-api-openapi.yml
- filename: momentum-user-provided-meeting-api-openapi.yml
  format: yaml
  label: Momentum User Provided Meeting API
  slug: momentum-user-provided-meeting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/momentum/openapi/momentum-user-provided-meeting-api-openapi.yml
consequence_counts:
  read: 3
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Momentum Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Momentum exposes 5 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Momentum
provider_slug: momentum
slug: momentum-agentic-access
source_filename: momentum-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/momentum-meeting-api-openapi.yml, openapi/momentum-momentum-api-api-openapi.yml,\n  openapi/momentum-signals-api-openapi.yml, openapi/momentum-user-provided-meeting-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    acting: 2\n    connected: 3\n  by_consequence:\n    write: 2\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/meeting/remap\n  method: post\n  operationId: post_v1_meeting_remap\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/{v1id}\n  method: get\n  operationId: get_v1_v1id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/signals/prompts\n  method: get\n  operationId: get_v1_signals_prompts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/signals\n  method: get\n  operationId: get_v2_signals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/user-provided-meeting\n  method: post\n  operationId: post_v1_user_provided_meeting\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/momentum/agentic-access/momentum-agentic-access.yml
summary_line: 5 operations · 2 acting
tags:
- Company
- Artificial Intelligence
- Revenue
- Automation
- Salesforce
---
