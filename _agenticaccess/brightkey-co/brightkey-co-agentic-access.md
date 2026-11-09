---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 6
api_specs:
- filename: brightkey-co-answers-api-openapi.yml
  format: yaml
  label: BrightKey Answers API
  slug: brightkey-co-answers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brightkey-co/openapi/brightkey-co-answers-api-openapi.yml
- filename: brightkey-co-compare-api-openapi.yml
  format: yaml
  label: BrightKey Compare API
  slug: brightkey-co-compare-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brightkey-co/openapi/brightkey-co-compare-api-openapi.yml
- filename: brightkey-co-roi-api-openapi.yml
  format: yaml
  label: BrightKey Roi API
  slug: brightkey-co-roi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brightkey-co/openapi/brightkey-co-roi-api-openapi.yml
- filename: brightkey-co-schools-api-openapi.yml
  format: yaml
  label: BrightKey Schools API
  slug: brightkey-co-schools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brightkey-co/openapi/brightkey-co-schools-api-openapi.yml
- filename: brightkey-co-universities-api-openapi.yml
  format: yaml
  label: BrightKey Universities API
  slug: brightkey-co-universities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brightkey-co/openapi/brightkey-co-universities-api-openapi.yml
consequence_counts:
  read: 6
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Brightkey Co Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'BrightKey exposes 7 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BrightKey
provider_slug: brightkey-co
slug: brightkey-co-agentic-access
source_filename: brightkey-co-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/brightkey-co-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 6\n    acting: 1\n  by_consequence:\n    read: 6\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /universities\n  method: get\n  operationId: listUniversities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /universities/{slug}\n  method: get\n  operationId: getUniversity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /compare\n  method: get\n\
  \  operationId: compareUniversities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /roi\n  method: post\n  operationId: degreeRoi\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /roi/countries\n  method: get\n  operationId: listRoiCountries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schools\n  method: get\n  operationId: listSchools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /answers\n  method: get\n  operationId: searchAnswers\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/brightkey-co/agentic-access/brightkey-co-agentic-access.yml
summary_line: 7 operations · 1 acting
tags:
- Education
- Consulting
- International
- Family
- Asia Pacific
---
