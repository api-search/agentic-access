---
acting_count: 2
action_class_counts:
  acting: 2
api_specs:
- filename: atlassian-compass-openapi.yml
  format: yaml
  label: Atlassian Compass REST API
  slug: atlassian-compass-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlassian-compass/refs/heads/main/openapi/atlassian-compass-openapi.yml
consequence_counts:
  physical: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Atlassian Compass Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /compass/v1/events
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /compass/v1/metrics
operation_count: 2
overview: 'Atlassian Compass exposes 2 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Atlassian Compass
provider_slug: atlassian-compass
slug: atlassian-compass-agentic-access
source_filename: atlassian-compass-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/atlassian-compass-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 2\n  by_action_class:\n    acting: 2\n  by_consequence:\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /compass/v1/metrics\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - write:metric:compass\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /compass/v1/events\n  method: post\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    scope:\n    - write:event:compass\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atlassian-compass/refs/heads/main/agentic-access/atlassian-compass-agentic-access.yml
summary_line: 2 operations · 2 acting
tags:
- Atlassian
- Component Management
- Developer Experience
- Software Catalog
- GraphQL
---
