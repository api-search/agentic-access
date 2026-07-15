---
acting_count: 0
action_class_counts:
  connected: 6
api_specs:
- filename: architectural-design-patterns-api.yaml
  format: yaml
  label: Architectural Design Patterns API
  slug: architectural-design-patterns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/architectural-design-patterns/refs/heads/main/openapi/architectural-design-patterns-api.yaml
consequence_counts:
  read: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Architectural Design Patterns Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Architectural Design Patterns exposes 6 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Architectural Design Patterns
provider_slug: architectural-design-patterns
slug: architectural-design-patterns-agentic-access
source_filename: architectural-design-patterns-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/architectural-design-patterns-api.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 6\n  by_consequence:\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /patterns\n  method: get\n  operationId: listPatterns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /patterns/{patternId}\n  method: get\n  operationId: getPattern\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /patterns/{patternId}/examples\n  method: get\n \
  \ operationId: getPatternExamples\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /patterns/{patternId}/relationships\n  method: get\n  operationId: getPatternRelationships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /categories\n  method: get\n  operationId: listCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /anti-patterns\n  method: get\n  operationId: listAntiPatterns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/architectural-design-patterns/refs/heads/main/agentic-access/architectural-design-patterns-agentic-access.yml
summary_line: 6 operations
tags:
- Design Patterns
- Software Architecture
- Best Practices
- Software Engineering
- System Design
- Microservices
---
