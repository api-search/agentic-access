---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 8
api_specs:
- filename: pinpoint-openapi.yml
  format: yaml
  label: Pinpoint Jobs API
  slug: jobs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinpoint/refs/heads/main/openapi/pinpoint-openapi.yml
- filename: pinpoint-openapi.yml
  format: yaml
  label: Pinpoint Applications API
  slug: applications
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinpoint/refs/heads/main/openapi/pinpoint-openapi.yml
- filename: pinpoint-openapi.yml
  format: yaml
  label: Pinpoint Applicants API
  slug: applicants
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinpoint/refs/heads/main/openapi/pinpoint-openapi.yml
- filename: pinpoint-openapi.yml
  format: yaml
  label: Pinpoint Job Stages API
  slug: job-stages
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinpoint/refs/heads/main/openapi/pinpoint-openapi.yml
- filename: pinpoint-openapi.yml
  format: yaml
  label: Pinpoint Comments and Files API
  slug: comments-files
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinpoint/refs/heads/main/openapi/pinpoint-openapi.yml
- filename: pinpoint-openapi.yml
  format: yaml
  label: Pinpoint Webhooks
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinpoint/refs/heads/main/openapi/pinpoint-openapi.yml
consequence_counts:
  read: 8
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Pinpoint Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'Pinpoint exposes 16 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Pinpoint
provider_slug: pinpoint
slug: pinpoint-agentic-access
source_filename: pinpoint-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/pinpoint-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 8\n    acting: 8\n  by_consequence:\n    read: 8\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /jobs\n  method: get\n  operationId: listJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs\n  method: post\n  operationId: createJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /jobs/{id}\n  method: get\n  operationId: getJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{id}\n  method: patch\n  operationId: updateJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs/{id}\n  method: delete\n  operationId: destroyJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications\n  method: get\n  operationId: listApplications\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications\n  method: post\n  operationId: createApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{id}\n  method: get\n  operationId: getApplication\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{id}\n  method: patch\n  operationId: updateApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n  \
  \    triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{id}\n  method: delete\n  operationId: destroyApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /candidates\n  method: get\n  operationId: listCandidates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /candidates/{id}\n  method: get\n  operationId: getCandidate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /candidates/{id}\n  method: patch\n  operationId: updateCandidate\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /comments\n  method: get\n  operationId: listComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /comments\n  method: post\n  operationId: createComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /comments/{id}\n  method: get\n  operationId: getComment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pinpoint/refs/heads/main/agentic-access/pinpoint-agentic-access.yml
summary_line: 16 operations · 8 acting
tags:
- ATS
- Recruitment
- Hiring
- HR Tech
- JSON:API
---
