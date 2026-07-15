---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 11
api_specs:
- filename: trelica-rest-api-openapi.yml
  format: yaml
  label: Trelica REST API
  slug: trelica
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trelica/refs/heads/main/openapi/trelica-rest-api-openapi.yml
consequence_counts:
  read: 11
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Trelica Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'Trelica exposes 13 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Trelica
provider_slug: trelica
slug: trelica-agentic-access
source_filename: trelica-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/trelica-rest-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 11\n    acting: 2\n  by_consequence:\n    read: 11\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /apps/v1\n  method: get\n  operationId: listApplications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Apps.Read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps/v1/{appId}\n  method: get\n  operationId: getApplication\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Apps.Read\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /apps/v1/{appId}/users\n  method: get\n  operationId: listApplicationUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Apps.Users.Read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people/v1\n  method: get\n  operationId: listPeople\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - People.Read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people/v1\n  method: post\n  operationId: createPerson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - People.Write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /people/v1/{personId}\n  method: get\n  operationId: getPerson\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - People.Read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people/v1/{personId}\n  method: patch\n  operationId: updatePerson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - People.Write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/v1\n  method: get\n  operationId: listContracts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Contracts.Read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts/v1/{contractId}\n  method: get\n  operationId: getContract\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Contracts.Read\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /workflows/v1\n  method: get\n  operationId: listWorkflows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Workflows.Read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/v1\n  method: get\n  operationId: listAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Assets.Read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /audit/v1\n  method: get\n  operationId: listAuditLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - AuditLog.Read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scim/v2/Users\n  method: get\n  operationId: listScimUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - Users.Read\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trelica/refs/heads/main/agentic-access/trelica-agentic-access.yml
summary_line: 13 operations · 2 acting
tags:
- Contract Management
- IT Management
- License Management
- SaaS Management
- Software Asset Management
---
