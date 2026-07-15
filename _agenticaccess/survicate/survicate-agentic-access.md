---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 8
api_specs:
- filename: survicate-data-export-openapi.yml
  format: yaml
  label: Survicate Data Export API
  slug: survicate-data-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/survicate/refs/heads/main/openapi/survicate-data-export-openapi.yml
consequence_counts:
  read: 8
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Survicate Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Survicate exposes 9 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Survicate
provider_slug: survicate
slug: survicate-agentic-access
source_filename: survicate-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/survicate-data-export-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 8\n    acting: 1\n  by_consequence:\n    read: 8\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/surveys\n  method: get\n  operationId: listSurveys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/surveys/{surveyId}\n  method: get\n  operationId: getSurvey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/surveys/{surveyId}/questions\n\
  \  method: get\n  operationId: listSurveyQuestions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/surveys/{surveyId}/responses\n  method: get\n  operationId: listResponses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/surveys/{surveyId}/responses/{responseId}\n  method: get\n  operationId: getResponse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/respondents/{respondentId}/attributes\n  method: get\n  operationId: listRespondentAttributes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/respondents/{respondentId}/responses\n  method: get\n  operationId:\
  \ listRespondentResponses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/personal-data\n  method: get\n  operationId: getPersonalDataCounters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/personal-data\n  method: delete\n  operationId: deletePersonalDataByEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/survicate/refs/heads/main/agentic-access/survicate-agentic-access.yml
summary_line: 9 operations · 1 acting
tags:
- Surveys
- Customer Feedback
- NPS
- User Research
- Feedback Analytics
- CRM Integration
- Customer Experience
---
