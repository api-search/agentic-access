---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 8
api_specs:
- filename: cogny-openapi.yml
  format: yaml
  label: Cogny API
  slug: cogny-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cogny/refs/heads/main/openapi/cogny-openapi.yml
consequence_counts:
  read: 8
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cogny Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'Cogny exposes 15 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cogny
provider_slug: cogny
slug: cogny-agentic-access
source_filename: cogny-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/cogny-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 8\n    acting: 7\n  by_consequence:\n    read: 8\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /reports\n  method: get\n  operationId: listReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - reports:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports\n  method: post\n  operationId: createReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - reports:write\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reports/{report_id}\n  method: get\n  operationId: getReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - reports:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/{report_id}\n  method: delete\n  operationId: cancelReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - reports:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reports/{report_id}/stream\n  method: get\n  operationId: streamReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - reports:read\n    token:\n    \
  \  max-ttl: 3600\n    audit: none\n- path: /reports/{report_id}/content\n  method: get\n  operationId: getReportContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - reports:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tickets\n  method: get\n  operationId: listTickets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - tickets:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tickets/{ticket_id}\n  method: get\n  operationId: getTicket\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - tickets:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tickets/{ticket_id}\n  method: patch\n  operationId: updateTicket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - tickets:write\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tickets/bulk-update\n  method: post\n  operationId: bulkUpdateTickets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - tickets:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tickets/{ticket_id}/dismiss\n  method: post\n  operationId: dismissTicket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - tickets:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tickets/stats\n  method: get\n  operationId:\
  \ getTicketStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - tickets:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tickets/export\n  method: post\n  operationId: exportTickets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - tickets:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /warehouses\n  method: get\n  operationId: listWarehouses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - warehouses:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    -\
  \ write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cogny/refs/heads/main/agentic-access/cogny-agentic-access.yml
summary_line: 15 operations · 7 acting
tags:
- Company
- Ai Enterprise Software
- Marketing
- Marketing Analytics
- Marketing Automation
- MCP
- Agents
- Data Warehouse
- Advertising
---
