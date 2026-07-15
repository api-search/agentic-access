---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 17
api_specs:
- filename: freshteam-openapi.yml
  format: yaml
  label: Freshteam Employees API
  slug: freshteam-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshteam/refs/heads/main/openapi/freshteam-openapi.yml
- filename: freshteam-openapi.yml
  format: yaml
  label: Freshteam Time-off API
  slug: freshteam-time-off-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshteam/refs/heads/main/openapi/freshteam-openapi.yml
- filename: freshteam-openapi.yml
  format: yaml
  label: Freshteam Job Postings API
  slug: freshteam-job-postings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshteam/refs/heads/main/openapi/freshteam-openapi.yml
- filename: freshteam-openapi.yml
  format: yaml
  label: Freshteam Applicants API
  slug: freshteam-applicants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshteam/refs/heads/main/openapi/freshteam-openapi.yml
- filename: freshteam-openapi.yml
  format: yaml
  label: Freshteam Onboarding API
  slug: freshteam-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshteam/refs/heads/main/openapi/freshteam-openapi.yml
consequence_counts:
  read: 17
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Freshteam Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 25
overview: 'Freshteam exposes 25 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Freshteam
provider_slug: freshteam
slug: freshteam-agentic-access
source_filename: freshteam-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/freshteam-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    connected: 17\n    acting: 8\n  by_consequence:\n    read: 17\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /employees\n  method: get\n  operationId: listEmployees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employees\n  method: post\n  operationId: createEmployee\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /employees/{id}\n  method: get\n  operationId: getEmployee\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employees/{id}\n  method: put\n  operationId: updateEmployee\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /employee_fields\n  method: get\n  operationId: listEmployeeFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /branches\n  method: get\n  operationId: listBranches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /departments\n  method: get\n  operationId: listDepartments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sub_departments\n  method: get\n  operationId: listSubDepartments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /business_units\n  method: get\n  operationId: listBusinessUnits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /teams\n  method: get\n  operationId: listTeams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /roles\n  method: get\n  operationId: listRoles\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /time_offs\n  method: get\n  operationId: listTimeOffs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /time_offs\n  method: post\n  operationId: createTimeOff\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /time_offs/{id}\n  method: get\n  operationId: getTimeOff\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /time_offs/{id}/approve\n  method: put\n  operationId: approveTimeOff\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /time_offs/{id}/cancel\n  method: put\n  operationId: cancelTimeOff\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /time_off_types\n  method: get\n  operationId: listTimeOffTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /job_postings\n  method: get\n  operationId: listJobPostings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /job_postings/{id}\n  method: get\n  operationId: getJobPosting\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /job_posting_fields\n  method: get\n  operationId: listJobPostingFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /job_postings/{id}/applicants\n  method: post\n  operationId: createApplicant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /candidate_sources\n  method: get\n  operationId: listCandidateSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /candidate_sources\n  method: post\n  operationId: createCandidateSource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /new_hires\n  method: post\n  operationId: createNewHire\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /new_hires/{id}\n  method: get\n  operationId: getNewHire\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freshteam/refs/heads/main/agentic-access/freshteam-agentic-access.yml
summary_line: 25 operations · 8 acting
tags:
- Human Resources
- HRIS
- Applicant Tracking
- ATS
- Recruiting
- Employee Management
- Onboarding
- Time Off
- HR Software
- End of Life
---
