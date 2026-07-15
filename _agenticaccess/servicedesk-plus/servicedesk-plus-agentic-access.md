---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 2
api_specs:
- filename: servicedesk-plus-openapi.yml
  format: yaml
  label: ServiceDesk Plus REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicedesk-plus/refs/heads/main/openapi/servicedesk-plus-openapi.yml
consequence_counts:
  read: 2
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Servicedesk Plus Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'ManageEngine ServiceDesk Plus exposes 6 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ManageEngine ServiceDesk Plus
provider_slug: servicedesk-plus
slug: servicedesk-plus-agentic-access
source_filename: servicedesk-plus-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/servicedesk-plus-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 2\n    acting: 4\n  by_consequence:\n    read: 2\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /app/{portal}/api/v3/requests\n  method: get\n  operationId: listRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app/{portal}/api/v3/requests\n  method: post\n  operationId: createRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /app/{portal}/api/v3/requests/{request_id}\n  method: get\n  operationId: getRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app/{portal}/api/v3/requests/{request_id}\n  method: put\n  operationId: updateRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /app/{portal}/api/v3/requests/{request_id}\n  method: delete\n  operationId: deleteRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /app/{portal}/api/v3/requests/{request_id}/attachments\n  method: post\n  operationId: addRequestAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/servicedesk-plus/refs/heads/main/agentic-access/servicedesk-plus-agentic-access.yml
summary_line: 6 operations · 4 acting
tags:
- ITSM
- Help Desk
- Incident Management
- Asset Management
- CMDB
---
