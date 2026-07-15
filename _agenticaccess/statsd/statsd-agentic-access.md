---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 6
api_specs:
- filename: statsd-wire-protocol-asyncapi.yml
  format: yaml
  label: StatsD Wire Protocol
  slug: statsd-wire-protocol
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsd/refs/heads/main/asyncapi/statsd-wire-protocol-asyncapi.yml
- filename: statsd-admin-interface-openapi.yml
  format: yaml
  label: StatsD Admin Interface
  slug: statsd-admin-interface
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsd/refs/heads/main/openapi/statsd-admin-interface-openapi.yml
- filename: dogstatsd-wire-protocol-asyncapi.yml
  format: yaml
  label: DogStatsD Wire Protocol
  slug: dogstatsd-wire-protocol
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsd/refs/heads/main/asyncapi/dogstatsd-wire-protocol-asyncapi.yml
consequence_counts:
  read: 6
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Statsd Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'StatsD exposes 10 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: StatsD
provider_slug: statsd
slug: statsd-agentic-access
source_filename: statsd-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/statsd-admin-interface-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 6\n    acting: 4\n  by_consequence:\n    read: 6\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /stats\n  method: get\n  operationId: getStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /counters\n  method: get\n  operationId: listCounters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gauges\n  method: get\n  operationId: listGauges\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /timers\n  method: get\n  operationId: listTimers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /delcounters\n  method: post\n  operationId: deleteCounters\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /delgauges\n  method: post\n  operationId: deleteGauges\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /deltimers\n  method: post\n  operationId: deleteTimers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: post\n  operationId: setHealth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /config\n  method: get\n  operationId: dumpConfig\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/statsd/refs/heads/main/agentic-access/statsd-agentic-access.yml
summary_line: 10 operations · 4 acting
tags:
- Aggregation
- Daemon
- DogStatsD
- Line Protocol
- Metrics
- Observability
- Open Source
- StatsD
- TCP
- UDP
- Wire Protocol
---
