---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 5
api_specs:
- filename: openapi.yml
  format: yaml
  label: Google Cloud Load Balancing API
  slug: google-cloud-load-balancing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-load-balancing/refs/heads/main/openapi/openapi.yml
consequence_counts:
  read: 5
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Google Cloud Load Balancing Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Google Cloud Load Balancing exposes 7 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Google Cloud Load Balancing
provider_slug: google-cloud-load-balancing
slug: google-cloud-load-balancing-agentic-access
source_filename: google-cloud-load-balancing-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 5\n    acting: 2\n  by_consequence:\n    read: 5\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /projects/{project}/global/backendServices\n  method: get\n  operationId: listBackendServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/compute\n- path: /projects/{project}/global/backendServices\n  method: post\n  operationId: createBackendService\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/compute\n- path: /projects/{project}/global/backendServices/{backendService}\n  method: get\n  operationId: getBackendService\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/compute\n- path: /projects/{project}/global/backendServices/{backendService}\n  method: delete\n  operationId: deleteBackendService\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n\
  \    - https://www.googleapis.com/auth/compute\n- path: /projects/{project}/global/healthChecks\n  method: get\n  operationId: listHealthChecks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/compute\n- path: /projects/{project}/global/forwardingRules\n  method: get\n  operationId: listForwardingRules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/compute\n- path: /projects/{project}/global/urlMaps\n  method: get\n  operationId: listUrlMaps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/compute\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-load-balancing/refs/heads/main/agentic-access/google-cloud-load-balancing-agentic-access.yml
summary_line: 7 operations · 2 acting
tags:
- Google Cloud
- Infrastructure
- Load Balancing
- Networking
- Traffic Management
---
