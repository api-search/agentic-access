---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 5
api_specs:
- filename: indeed-employer-api-openapi.yml
  format: yaml
  label: Indeed Job Sync API
  slug: job-sync
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/indeed/refs/heads/main/openapi/indeed-employer-api-openapi.yml
- filename: indeed-employer-api-openapi.yml
  format: yaml
  label: Indeed Employer API
  slug: employer
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/indeed/refs/heads/main/openapi/indeed-employer-api-openapi.yml
consequence_counts:
  read: 5
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Indeed Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Indeed exposes 12 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Indeed
provider_slug: indeed
slug: indeed-agentic-access
source_filename: indeed-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/indeed-employer-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    acting: 7\n    connected: 5\n  by_consequence:\n    write: 7\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/employers\n  method: post\n  operationId: createEmployer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/employers/{employerId}\n  method: get\n  operationId: getEmployer\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/employers/{employerId}\n  method: patch\n  operationId: updateEmployer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/employers/{employerId}/registration\n  method: put\n  operationId: registerEmployerForCandidateSync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/employers/{employerId}/candidates\n  method: get\n  operationId: listCandidates\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/employers/{employerId}/candidates/{candidateId}\n  method: get\n  operationId: getCandidate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/employers/{employerId}/candidates/{candidateId}/disposition\n  method: put\n  operationId: updateCandidateDisposition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/jobs\n  method: post\n  operationId: createJobPostings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/jobs/{jobPostingId}\n  method: get\n  operationId: getJobPosting\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{jobPostingId}\n  method: put\n  operationId: updateJobPosting\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/jobs/{jobPostingId}\n  method: delete\n  operationId: expireJobPosting\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /v1/employers/{employerId}/jobs\n  method: get\n  operationId: listEmployerJobPostings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/indeed/refs/heads/main/agentic-access/indeed-agentic-access.yml
summary_line: 12 operations · 7 acting
tags:
- Careers
- Employment
- Hiring
- Job Search
- Jobs
- Recruiting
---
