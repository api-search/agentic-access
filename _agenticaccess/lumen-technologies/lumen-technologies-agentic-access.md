---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 2
api_specs:
- filename: lumen-internet-on-demand-api-openapi.yml
  format: yaml
  label: Lumen Internet On-Demand API
  slug: internet-on-demand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumen-technologies/refs/heads/main/openapi/lumen-internet-on-demand-api-openapi.yml
consequence_counts:
  read: 2
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Lumen Technologies Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'Lumen Technologies exposes 4 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Lumen Technologies
provider_slug: lumen-technologies
slug: lumen-technologies-agentic-access
source_filename: lumen-technologies-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/lumen-internet-on-demand-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    connected: 2\n    acting: 2\n  by_consequence:\n    read: 2\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /internet-on-demand/connections\n  method: get\n  operationId: listConnections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /internet-on-demand/connections\n  method: post\n  operationId: createConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n   \
  \   max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /internet-on-demand/connections/{connectionId}\n  method: get\n  operationId: getConnection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /internet-on-demand/connections/{connectionId}/bandwidth\n  method: put\n  operationId: updateBandwidth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lumen-technologies/refs/heads/main/agentic-access/lumen-technologies-agentic-access.yml
summary_line: 4 operations · 2 acting
tags:
- Bandwidth
- Edge Cloud
- Fiber
- Infrastructure
- Internet
- Network
- Networking
- Security
- Telecom
---
