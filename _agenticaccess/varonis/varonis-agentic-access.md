---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 1
api_specs:
- filename: varonis-datalert-openapi.yml
  format: yaml
  label: Varonis DatAlert API
  slug: varonis-datalert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/varonis/refs/heads/main/openapi/varonis-datalert-openapi.yml
consequence_counts:
  read: 1
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Varonis Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Varonis exposes 6 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Varonis
provider_slug: varonis
slug: varonis-agentic-access
source_filename: varonis-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/varonis-datalert-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    acting: 5\n    connected: 1\n  by_consequence:\n    write: 5\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /threatdetection/api/alert/alert/GetAlerts\n  method: post\n  operationId: getAlerts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /threatdetection/api/alert/alert/GetAlertedEvents\n  method: post\n  operationId: getAlertedEvents\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /threatdetection/api/alert/alert/SetAlertStatus\n  method: post\n  operationId: updateAlertStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /threatdetection/api/alert/alert/CloseAlert\n  method: post\n  operationId: closeAlert\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n     \
  \ - high-value\n    audit: required\n- path: /threatdetection/api/alert/alert/AddNote\n  method: post\n  operationId: addAlertNote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /threatdetection/api/alert/alert/GetThreatModels\n  method: get\n  operationId: getThreatModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/varonis/refs/heads/main/agentic-access/varonis-agentic-access.yml
summary_line: 6 operations · 5 acting
tags:
- Cloud Security
- Compliance
- Data Analytics
- Data Governance
- Data Security
- Threat Detection
---
