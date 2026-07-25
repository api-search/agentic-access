---
acting_count: 7
action_class_counts:
  acting: 7
api_specs:
- filename: ibisworld-business-environment-api-openapi.yml
  format: yaml
  label: IBISWorld Business Environment API
  slug: ibisworld-business-environment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibisworld/refs/heads/main/openapi/ibisworld-business-environment-api-openapi.yml
- filename: ibisworld-classification-api-openapi.yml
  format: yaml
  label: IBISWorld Classification API
  slug: ibisworld-classification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibisworld/refs/heads/main/openapi/ibisworld-classification-api-openapi.yml
- filename: ibisworld-company-api-openapi.yml
  format: yaml
  label: IBISWorld Company API
  slug: ibisworld-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibisworld/refs/heads/main/openapi/ibisworld-company-api-openapi.yml
- filename: ibisworld-downloads-api-openapi.yml
  format: yaml
  label: IBISWorld Downloads API
  slug: ibisworld-downloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibisworld/refs/heads/main/openapi/ibisworld-downloads-api-openapi.yml
- filename: ibisworld-industry-api-openapi.yml
  format: yaml
  label: IBISWorld Industry API
  slug: ibisworld-industry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibisworld/refs/heads/main/openapi/ibisworld-industry-api-openapi.yml
consequence_counts:
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ibisworld Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'IBISWorld exposes 7 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: IBISWorld
provider_slug: ibisworld
slug: ibisworld-agentic-access
source_filename: ibisworld-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/ibisworld-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    acting: 7\n  by_consequence:\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /industry/v3/reportlist\n  method: post\n  operationId: listReports\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /industry/v3/sections\n  method: post\n  operationId: listSections\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n  \
  \  subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /industry/v3/report\n  method: post\n  operationId: getReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /company/v3/lookup\n  method: post\n  operationId: lookupCompany\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /environment/v3/profilelist\n  method: post\n  operationId: listEnvironmentProfiles\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /classification/v3/systems\n  method: post\n  operationId: listClassificationSystems\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /downloads/v3/list\n  method: post\n  operationId: listDownloads\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ibisworld/refs/heads/main/agentic-access/ibisworld-agentic-access.yml
summary_line: 7 operations · 7 acting
tags:
- Business Intelligence
- Economics
- Industry Data
- Market Research
---
