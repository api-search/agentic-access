---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 8
api_specs:
- filename: markifact-com-connections-api-openapi.yml
  format: yaml
  label: markifact-com Connections API
  slug: markifact-com-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/markifact-com/openapi/markifact-com-connections-api-openapi.yml
- filename: markifact-com-credits-api-openapi.yml
  format: yaml
  label: markifact-com Credits API
  slug: markifact-com-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/markifact-com/openapi/markifact-com-credits-api-openapi.yml
- filename: markifact-com-logs-api-openapi.yml
  format: yaml
  label: markifact-com Logs API
  slug: markifact-com-logs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/markifact-com/openapi/markifact-com-logs-api-openapi.yml
consequence_counts:
  read: 8
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Markifact Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'markifact-com exposes 11 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: markifact-com
provider_slug: markifact-com
slug: markifact-com-agentic-access
source_filename: markifact-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/markifact-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 8\n    acting: 3\n  by_consequence:\n    read: 8\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/connections\n  method: get\n  operationId: listConnections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connections\n  method: post\n  operationId: createConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connections/types\n  method: get\n  operationId: listConnectionTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connections/{connection_id}\n  method: get\n  operationId: getConnection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connections/{connection_id}\n  method: delete\n  operationId: deleteConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connections/auth-link\n  method: post\n  operationId: createAuthLink\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connections/auth-links/{auth_link_id}/status\n  method: get\n  operationId: getAuthLinkStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/credits\n  method: get\n  operationId: getCreditBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/credits/logs\n  method: get\n  operationId: listCreditLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/logs\n  method: get\n  operationId:\
  \ listLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/logs/{log_id}\n  method: get\n  operationId: getLog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/markifact-com/agentic-access/markifact-com-agentic-access.yml
summary_line: 11 operations · 3 acting
tags:
- AI Marketing Automation
- Ad Management
- Reporting
- Workflow Automation
- Marketing Operations
- Data Integration
---
