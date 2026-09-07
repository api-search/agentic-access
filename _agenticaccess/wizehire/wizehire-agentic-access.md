---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 3
api_specs:
- filename: wizehire-scout-service-openapi.yml
  format: yaml
  label: Wizehire Scout Service API
  slug: wizehire-scout-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wizehire/refs/heads/main/openapi/wizehire-scout-service-openapi.yml
consequence_counts:
  read: 3
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Wizehire Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'WizeHire exposes 5 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: WizeHire
provider_slug: wizehire
slug: wizehire-agentic-access
source_filename: wizehire-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: generated\nsource: openapi/wizehire-scout-service-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 3\n    acting: 2\n  by_consequence:\n    read: 3\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /healthz\n  method: get\n  operationId: healthz\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/chat\n  method: post\n  operationId: agentChat\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/candidates/top/{job_key}\n  method: get\n  operationId: get_top_applies_v1_candidates_top__job_key__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/candidates/{apply_id}\n  method: get\n  operationId: get_apply_details_v1_candidates__apply_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/interviews/schedule\n  method: post\n  operationId: schedule_interview_v1_interviews_schedule_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wizehire/refs/heads/main/agentic-access/wizehire-agentic-access.yml
summary_line: 5 operations · 2 acting
tags:
- Hiring
- Recruiting
- Applicant Tracking
- Human Resources
- Talent Assessment
- Small Business
- Artificial Intelligence
- Job Boards
- Onboarding
- HR Tech
---
