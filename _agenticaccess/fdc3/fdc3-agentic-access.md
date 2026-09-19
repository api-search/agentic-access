---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 4
api_specs:
- filename: app-directory.html
  format: yaml
  label: FDC3 App Directory API
  slug: app-directory-api
  spec_type: OpenAPI
  url: https://fdc3.finos.org/schemas/2.2/app-directory.html
- filename: fdc3-application-api-openapi.yml
  format: yaml
  label: FDC3 Application API
  slug: fdc3-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fdc3/refs/heads/main/openapi/fdc3-application-api-openapi.yml
consequence_counts:
  read: 4
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Fdc3 Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'FDC3 exposes 5 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: FDC3
provider_slug: fdc3
slug: fdc3-agentic-access
source_filename: fdc3-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: generated\nsource: openapi/fdc3-application-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 4\n    acting: 1\n  by_consequence:\n    read: 4\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/apps/{appId}\n  method: get\n  operationId: getV2AppsByAppId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/apps\n  method: get\n  operationId: getV2Apps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps/{appId}\n  method: get\n\
  \  operationId: getV1AppsByAppId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apps\n  method: post\n  operationId: postV1Apps\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apps/search\n  method: get\n  operationId: getV1AppsSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fdc3/refs/heads/main/agentic-access/fdc3-agentic-access.yml
summary_line: 5 operations · 1 acting
tags:
- Financial-Services
- Fintech
- Desktop Interoperability
- Open Standard
- FINOS
- Context Sharing
- Intents
---
