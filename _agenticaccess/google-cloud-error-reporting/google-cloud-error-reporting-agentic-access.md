---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 3
api_specs:
- filename: openapi.yml
  format: yaml
  label: Google Cloud Error Reporting API
  slug: google-cloud-error-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-error-reporting/refs/heads/main/openapi/openapi.yml
consequence_counts:
  read: 3
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Google Cloud Error Reporting Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Google Cloud Error Reporting exposes 6 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Google Cloud Error Reporting
provider_slug: google-cloud-error-reporting
slug: google-cloud-error-reporting-agentic-access
source_filename: google-cloud-error-reporting-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 3\n    acting: 3\n  by_consequence:\n    read: 3\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /v1beta1/projects/{projectId}/events\n  method: get\n  operationId: listEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1beta1/projects/{projectId}/events:report\n  method: post\n  operationId: reportEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1beta1/projects/{projectId}/groupStats\n  method: get\n  operationId: listGroupStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1beta1/projects/{projectId}/groups/{groupId}\n  method: get\n  operationId: getGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1beta1/projects/{projectId}/groups/{groupId}\n  method: put\n  operationId: updateGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1beta1/projects/{projectId}/events:deleteAll\n\
  \  method: delete\n  operationId: deleteEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-error-reporting/refs/heads/main/agentic-access/google-cloud-error-reporting-agentic-access.yml
summary_line: 6 operations · 3 acting
tags:
- Debugging
- Error Reporting
- Errors
- Exceptions
- Google Cloud
- Observability
- Reliability
---
