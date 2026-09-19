---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 1
api_specs:
- filename: netdata-alerts-api-openapi.yml
  format: yaml
  label: Netdata alerts API
  slug: netdata-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netdata/refs/heads/main/openapi/netdata-alerts-api-openapi.yml
- filename: netdata-charts-api-openapi.yml
  format: yaml
  label: Netdata charts API
  slug: netdata-charts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netdata/refs/heads/main/openapi/netdata-charts-api-openapi.yml
consequence_counts:
  read: 1
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Netdata Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Netdata exposes 7 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Netdata
provider_slug: netdata
slug: netdata-agentic-access
source_filename: netdata-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: generated\nsource: openapi/netdata-alerts-api-openapi.yml, openapi/netdata-charts-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    acting: 6\n    connected: 1\n  by_consequence:\n    write: 6\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v2/spaces/{spaceID}/notifications/silencing/rrule/evaluate\n  method: post\n  operationId: evaluate-rrule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/spaces/{spaceID}/notifications/silencing/rule\n\
  \  method: post\n  operationId: create-silencing-rule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/spaces/{spaceID}/notifications/silencing/rule/ruleID\n  method: put\n  operationId: update-silencing-rule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/spaces/{spaceID}/notifications/silencing/rules\n  method: get\n  operationId: get-silencing-rules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/v2/spaces/{spaceID}/notifications/silencing/rules/delete\n  method: post\n  operationId: delete-silencing-rules\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/spaces/{spaceID}/rooms/{roomID}/alerts:misconfigured\n  method: post\n  operationId: get-room-alerts-misconfigured\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v3/spaces/{spaceID}/rooms/{roomID}/data\n  method: post\n  operationId: post-scope-data\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/netdata/refs/heads/main/agentic-access/netdata-agentic-access.yml
summary_line: 7 operations · 6 acting
tags:
- Monitoring
- Observability
- Infrastructure
- Metrics
- Alerts
- Real-Time
- APM
- DevOps
---
