---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 4
api_specs:
- filename: Looker.4.0.oas.json
  format: json
  label: Looker API
  slug: looker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/looker-open-source/sdk-codegen/main/spec/Looker.4.0.oas.json
- filename: rest
  format: yaml
  label: Looker (Google Cloud core) API
  slug: looker-google-cloud-core-api
  spec_type: OpenAPI
  url: https://looker.googleapis.com/$discovery/rest?version=v1
consequence_counts:
  read: 4
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Google Looker Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Google Looker exposes 5 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Google Looker
provider_slug: google-looker
slug: google-looker-agentic-access
source_filename: google-looker-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    acting: 1\n    connected: 4\n  by_consequence:\n    write: 1\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /login\n  method: post\n  operationId: login\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user\n  method: get\n  operationId: getCurrentUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /users\n  method: get\n  operationId: getAllUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /looks\n  method: get\n  operationId: getAllLooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /looks/{look_id}/run/{result_format}\n  method: get\n  operationId: runLook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-looker/refs/heads/main/agentic-access/google-looker-agentic-access.yml
summary_line: 5 operations · 1 acting
tags: []
---
