---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 3
api_specs:
- filename: sieve-openapi.yml
  format: yaml
  label: Sieve Jobs Push API
  slug: sieve-jobs-push-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sieve/refs/heads/main/openapi/sieve-openapi.yml
- filename: sieve-openapi.yml
  format: yaml
  label: Sieve Jobs Status API
  slug: sieve-jobs-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sieve/refs/heads/main/openapi/sieve-openapi.yml
- filename: sieve-openapi.yml
  format: yaml
  label: Sieve Functions API
  slug: sieve-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sieve/refs/heads/main/openapi/sieve-openapi.yml
- filename: sieve-openapi.yml
  format: yaml
  label: Sieve Webhooks API
  slug: sieve-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sieve/refs/heads/main/openapi/sieve-openapi.yml
consequence_counts:
  read: 3
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sieve Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Sieve exposes 5 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Sieve
provider_slug: sieve
slug: sieve-agentic-access
source_filename: sieve-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/sieve-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    acting: 2\n    connected: 3\n  by_consequence:\n    write: 2\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /push\n  method: post\n  operationId: pushJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs\n  method: get\n  operationId: listJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{job_id}\n  method: get\n  operationId: getJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{job_id}\n  method: delete\n  operationId: cancelJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /functions/{owner_name}/{function_name}\n  method: get\n  operationId: getFunction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sieve/refs/heads/main/agentic-access/sieve-agentic-access.yml
summary_line: 5 operations · 2 acting
tags:
- AI
- Video
- Audio
- Media Processing
- Async Jobs
---
