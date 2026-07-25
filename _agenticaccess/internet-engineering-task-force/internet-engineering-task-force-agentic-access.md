---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 5
api_specs:
- filename: internet-engineering-task-force-documents-api-openapi.yml
  format: yaml
  label: Internet Engineering Task Force Documents API
  slug: internet-engineering-task-force-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/internet-engineering-task-force/refs/heads/main/openapi/internet-engineering-task-force-documents-api-openapi.yml
- filename: internet-engineering-task-force-framework-api-api-openapi.yml
  format: yaml
  label: Internet Engineering Task Force Framework API API
  slug: internet-engineering-task-force-framework-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/internet-engineering-task-force/refs/heads/main/openapi/internet-engineering-task-force-framework-api-api-openapi.yml
- filename: internet-engineering-task-force-identity-api-openapi.yml
  format: yaml
  label: Internet Engineering Task Force Identity API
  slug: internet-engineering-task-force-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/internet-engineering-task-force/refs/heads/main/openapi/internet-engineering-task-force-identity-api-openapi.yml
- filename: internet-engineering-task-force-iesg-api-openapi.yml
  format: yaml
  label: Internet Engineering Task Force IESG API
  slug: internet-engineering-task-force-iesg-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/internet-engineering-task-force/refs/heads/main/openapi/internet-engineering-task-force-iesg-api-openapi.yml
- filename: internet-engineering-task-force-meetings-api-openapi.yml
  format: yaml
  label: Internet Engineering Task Force Meetings API
  slug: internet-engineering-task-force-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/internet-engineering-task-force/refs/heads/main/openapi/internet-engineering-task-force-meetings-api-openapi.yml
consequence_counts:
  read: 5
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Internet Engineering Task Force Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Internet Engineering Task Force exposes 7 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Internet Engineering Task Force
provider_slug: internet-engineering-task-force
slug: internet-engineering-task-force-agentic-access
source_filename: internet-engineering-task-force-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/internet-engineering-task-force-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 5\n    acting: 2\n  by_consequence:\n    read: 5\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/version\n  method: get\n  operationId: getVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/{model}/{resource}/\n  method: get\n  operationId: listResource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/{model}/{resource}/{id}/\n\
  \  method: get\n  operationId: getResource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /doc/{document}/doc.json\n  method: get\n  operationId: getDocumentJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/iesg/position\n  method: post\n  operationId: setIesgPosition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/meeting/session/video/url\n  method: post\n  operationId: setSessionVideoUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/openid/\n  method: get\n  operationId: getOpenIdConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/internet-engineering-task-force/refs/heads/main/agentic-access/internet-engineering-task-force-agentic-access.yml
summary_line: 7 operations · 2 acting
tags:
- Internet
- Protocols
- RFC
- Standards
- Working Groups
---
