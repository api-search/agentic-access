---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 7
api_specs:
- filename: gamesight-measurement-openapi.json
  format: json
  label: Gamesight Measurement API
  slug: gamesight-measurement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gamesight/refs/heads/main/openapi/gamesight-measurement-openapi.json
- filename: gamesight-reporting-openapi.json
  format: json
  label: Gamesight Reporting API
  slug: gamesight-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gamesight/refs/heads/main/openapi/gamesight-reporting-openapi.json
consequence_counts:
  read: 7
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Gamesight Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'Gamesight exposes 14 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Gamesight
provider_slug: gamesight
slug: gamesight-agentic-access
source_filename: gamesight-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/gamesight-measurement-openapi.json, openapi/gamesight-reporting-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    acting: 7\n    connected: 7\n  by_consequence:\n    write: 7\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /events\n  method: post\n  operationId: measurement-api-events\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/batch\n  method: post\n  operationId: eventsbatch\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /games/{game_id}/do_not_track\n  method: put\n  operationId: do_not_track\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /games/{game_id}/do_not_track\n  method: get\n  operationId: get_do_not_track\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats\n  method: post\n  operationId: stats-v3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reporting/goals\n  method: post\n  operationId: reportinggoals\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /games\n  method: get\n  operationId: games\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trackers\n  method: get\n  operationId: trackers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trackers\n  method: post\n  operationId:\
  \ trackers-1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /goal_types\n  method: get\n  operationId: goal_types\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /audit_logs\n  method: get\n  operationId: audit_logs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reporting/users/events\n  method: get\n  operationId: reportingusersevents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reporting/users/touchpoints\n  method: get\n  operationId:\
  \ reportinguserstouchpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reporting/users/remove\n  method: delete\n  operationId: reportingusersremove\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gamesight/refs/heads/main/agentic-access/gamesight-agentic-access.yml
summary_line: 14 operations · 7 acting
tags:
- Company
- Gaming
- Marketing
- Analytics
- Attribution
- Measurement
- Advertising
- Creators
- Game Development
---
