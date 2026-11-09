---
acting_count: 0
action_class_counts:
  connected: 5
api_specs:
- filename: 7275-com-activity-api-openapi.yml
  format: yaml
  label: DEXUN Inc Activity API
  slug: 7275-com-activity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/7275-com/openapi/7275-com-activity-api-openapi.yml
- filename: 7275-com-identity-api-openapi.yml
  format: yaml
  label: DEXUN Inc Identity API
  slug: 7275-com-identity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/7275-com/openapi/7275-com-identity-api-openapi.yml
- filename: 7275-com-keys-api-openapi.yml
  format: yaml
  label: DEXUN Inc Keys API
  slug: 7275-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/7275-com/openapi/7275-com-keys-api-openapi.yml
- filename: 7275-com-public-api-openapi.yml
  format: yaml
  label: DEXUN Inc Public API
  slug: 7275-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/7275-com/openapi/7275-com-public-api-openapi.yml
- filename: 7275-com-quota-api-openapi.yml
  format: yaml
  label: DEXUN Inc Quota API
  slug: 7275-com-quota-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/7275-com/openapi/7275-com-quota-api-openapi.yml
consequence_counts:
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: 7275 Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'DEXUN Inc exposes 5 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: DEXUN Inc
provider_slug: 7275-com
slug: 7275-com-agentic-access
source_filename: 7275-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/7275-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 5\n  by_consequence:\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /me\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /usage\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /audit-events\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n    \
  \  max-ttl: 3600\n    audit: none\n- path: /api-keys\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /changelog\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/7275-com/agentic-access/7275-com-agentic-access.yml
summary_line: 5 operations
tags:
- Advertising
- Artificial Intelligence
- Marketing
- Multi-Account
- Automation
---
