---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 5
api_specs:
- filename: cri-o-status-openapi.yml
  format: yaml
  label: CRI-O Status API
  slug: cri-o-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cri-o/refs/heads/main/openapi/cri-o-status-openapi.yml
- filename: cri-o-metrics-openapi.yml
  format: yaml
  label: CRI-O Metrics API
  slug: cri-o-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cri-o/refs/heads/main/openapi/cri-o-metrics-openapi.yml
consequence_counts:
  read: 5
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cri O Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'CRI-O exposes 7 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CRI-O
provider_slug: cri-o
slug: cri-o-agentic-access
source_filename: cri-o-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/cri-o-metrics-openapi.yml, openapi/cri-o-status-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 5\n    acting: 2\n  by_consequence:\n    read: 5\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /metrics\n  method: get\n  operationId: getMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /info\n  method: get\n  operationId: getInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /config\n  method: get\n\
  \  operationId: getConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /containers/{id}\n  method: get\n  operationId: getContainer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pause/{id}\n  method: post\n  operationId: pauseContainer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /unpause/{id}\n  method: post\n  operationId: unpauseContainer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /debug/goroutines\n  method: get\n  operationId: getGoroutines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cri-o/refs/heads/main/agentic-access/cri-o-agentic-access.yml
summary_line: 7 operations · 2 acting
tags:
- Apache 2.0
- CNCF
- Cloud Native
- conmon
- Container Runtime
- Containers
- CRI
- Go
- Graduated
- Kubernetes
- OCI
- Open Source
- Prometheus
- runc
---
