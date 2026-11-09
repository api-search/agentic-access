---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 8
api_specs:
- filename: keenethics-labs-com-activity-api-openapi.yml
  format: yaml
  label: keenethics-labs-com Activity API
  slug: keenethics-labs-com-activity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keenethics-labs-com/openapi/keenethics-labs-com-activity-api-openapi.yml
- filename: keenethics-labs-com-districts-api-openapi.yml
  format: yaml
  label: keenethics-labs-com Districts API
  slug: keenethics-labs-com-districts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keenethics-labs-com/openapi/keenethics-labs-com-districts-api-openapi.yml
- filename: keenethics-labs-com-events-api-openapi.yml
  format: yaml
  label: keenethics-labs-com Events API
  slug: keenethics-labs-com-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keenethics-labs-com/openapi/keenethics-labs-com-events-api-openapi.yml
- filename: keenethics-labs-com-feedbacks-api-openapi.yml
  format: yaml
  label: keenethics-labs-com Feedbacks API
  slug: keenethics-labs-com-feedbacks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keenethics-labs-com/openapi/keenethics-labs-com-feedbacks-api-openapi.yml
- filename: keenethics-labs-com-navigation-api-openapi.yml
  format: yaml
  label: keenethics-labs-com Navigation API
  slug: keenethics-labs-com-navigation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keenethics-labs-com/openapi/keenethics-labs-com-navigation-api-openapi.yml
- filename: keenethics-labs-com-search-api-openapi.yml
  format: yaml
  label: keenethics-labs-com Search API
  slug: keenethics-labs-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keenethics-labs-com/openapi/keenethics-labs-com-search-api-openapi.yml
- filename: keenethics-labs-com-specialization-api-openapi.yml
  format: yaml
  label: keenethics-labs-com Specialization API
  slug: keenethics-labs-com-specialization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keenethics-labs-com/openapi/keenethics-labs-com-specialization-api-openapi.yml
consequence_counts:
  physical: 1
  read: 8
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Keenethics Labs Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /feedback
operation_count: 10
overview: 'keenethics-labs-com exposes 10 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 1 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: keenethics-labs-com
provider_slug: keenethics-labs-com
slug: keenethics-labs-com-agentic-access
source_filename: keenethics-labs-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/keenethics-entertainment-hub-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 8\n    acting: 2\n  by_consequence:\n    read: 8\n    physical: 1\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /district\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /event\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feedback\n  method: post\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /navigation\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/count\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/sync\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /specialization\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /activity\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /activity/{id}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/keenethics-labs-com/agentic-access/keenethics-labs-com-agentic-access.yml
summary_line: 10 operations · 2 acting
tags:
- Company
- R&D
- Innovation
- Artificial Intelligence
- Web Development
- Experimental Projects
---
