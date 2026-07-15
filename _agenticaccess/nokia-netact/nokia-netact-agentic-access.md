---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 7
api_specs:
- filename: nokia-netact-nbi-openapi.yml
  format: yaml
  label: Nokia NetAct / Ericsson OSS API
  slug: nokia-netact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nokia-netact/refs/heads/main/openapi/nokia-netact-nbi-openapi.yml
consequence_counts:
  read: 7
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Nokia Netact Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Nokia NetAct exposes 9 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Nokia NetAct
provider_slug: nokia-netact
slug: nokia-netact-agentic-access
source_filename: nokia-netact-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/nokia-netact-nbi-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 7\n    acting: 2\n  by_consequence:\n    read: 7\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /topology/network-elements\n  method: get\n  operationId: listNetworkElements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /topology/network-elements/{distinguishedName}\n  method: get\n  operationId: getNetworkElement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /topology/network-elements/{distinguishedName}/children\n  method: get\n  operationId: getNetworkElementChildren\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /faults/alarms\n  method: get\n  operationId: listActiveAlarms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /faults/alarms/{alarmId}\n  method: get\n  operationId: getAlarm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /faults/alarms/{alarmId}/acknowledge\n  method: post\n  operationId: acknowledgeAlarm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /performance/kpis\n  method: get\n  operationId: getPerformanceKPIs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /configuration/network-elements/{distinguishedName}/attributes\n  method: get\n  operationId: getNetworkElementAttributes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /configuration/network-elements/{distinguishedName}/attributes\n  method: patch\n  operationId: updateNetworkElementAttributes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nokia-netact/refs/heads/main/agentic-access/nokia-netact-agentic-access.yml
summary_line: 9 operations · 2 acting
tags:
- Network Management
- OSS
- SNMP
- Telecom
---
