---
acting_count: 0
action_class_counts:
  connected: 8
api_specs:
- filename: bicycle-guide-guide-registry-api-openapi.yml
  format: yaml
  label: Bicycle Guide Guide Registry API
  slug: bicycle-guide-guide-registry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bicycle-guide/openapi/bicycle-guide-guide-registry-api-openapi.yml
consequence_counts:
  read: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bicycle Guide Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Bicycle Guide exposes 8 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bicycle Guide
provider_slug: bicycle-guide
slug: bicycle-guide-agentic-access
source_filename: bicycle-guide-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/bicycle-guide-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 8\n  by_consequence:\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/guides\n  method: get\n  operationId: listGuides\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/guides/{slug}\n  method: get\n  operationId: getGuide\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/guides/search\n  method: get\n  operationId: searchGuides\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/guides/{slug}/disagreements\n  method: get\n  operationId: listDisagreements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/taxonomy\n  method: get\n  operationId: getTaxonomy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/capabilities\n  method: get\n  operationId: listCapabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/conditions\n  method: get\n  operationId: listConditions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/membership-interest\n  method: get\n  operationId: listMembershipInterest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/bicycle-guide/agentic-access/bicycle-guide-agentic-access.yml
summary_line: 8 operations
tags:
- Company
- Guides
- Artificial Intelligence
- Education
- Library
---
