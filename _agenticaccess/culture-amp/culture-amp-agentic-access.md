---
acting_count: 0
action_class_counts:
  connected: 19
api_specs:
- filename: spec
  format: yaml
  label: Culture Amp Public API
  slug: culture-amp-public-api
  spec_type: OpenAPI
  url: https://api.cultureamp.com/spec
consequence_counts:
  read: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Culture Amp Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 19
overview: 'Culture Amp exposes 19 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Culture Amp
provider_slug: culture-amp
slug: culture-amp-agentic-access
source_filename: culture-amp-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/culture-amp-public-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 19\n  by_consequence:\n    read: 19\n  human_in_the_loop_required: 0\noperations:\n- path: /employees\n  method: get\n  operationId: list-employees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - employees-read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employees/{id}\n  method: get\n  operationId: get-employee\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - employees-read\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /employees/{id}/demographics\n  method: get\n  operationId: list-demographics-by-employee\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - employee-demographics-read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employees/{id}/manager-reviews\n  method: get\n  operationId: list-manager-reviews-by-employee\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - performance-evaluations-read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /performance-cycles\n  method: get\n  operationId: list-performance-cycles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - performance-evaluations-read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /performance-cycles/{id}\n  method: get\n  operationId: get-performance-cycle\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    scope:\n    - performance-evaluations-read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /performance-cycles/{id}/manager-reviews\n  method: get\n  operationId: list-manager-reviews-by-performance-cycle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - performance-evaluations-read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /manager-reviews\n  method: get\n  operationId: list-manager-reviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - performance-evaluations-read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /manager-reviews/{id}\n  method: get\n  operationId: get-manager-review\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - performance-evaluations-read\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /surveys\n  method: get\n  operationId: list-surveys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - surveys-read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /surveys/{id}\n  method: get\n  operationId: get-survey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - surveys-read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /surveys/{id}/questions\n  method: get\n  operationId: list-survey-questions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - surveys-read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /surveys/{survey_id}/question/{question_id}\n  method: get\n  operationId: get-survey-question\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - surveys-read\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /surveys/{id}/responses\n  method: get\n  operationId: list-survey-responses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - surveys-read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /surveys/{survey_id}/responses/{response_id}\n  method: get\n  operationId: get-survey-response\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - surveys-read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /surveys/{id}/factors\n  method: get\n  operationId: list-survey-factors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - surveys-read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /surveys/{survey_id}/factors/{factor_id}\n  method: get\n  operationId: get-survey-factor\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    scope:\n    - surveys-read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /surveys/{id}/sections\n  method: get\n  operationId: list-survey-sections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - surveys-read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /surveys/{survey_id}/sections/{section_id}\n  method: get\n  operationId: get-survey-section\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - surveys-read\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/culture-amp/refs/heads/main/agentic-access/culture-amp-agentic-access.yml
summary_line: 19 operations
tags:
- HR
- Employee Engagement
- Performance Management
- People Analytics
- Surveys
- Human Resources
---
