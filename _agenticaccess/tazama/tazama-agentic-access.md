---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 2
api_specs:
- filename: tazama-transaction-monitoring-service-openapi.yml
  format: yaml
  label: Tazama Transaction Monitoring Service API
  slug: transaction-monitoring-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tazama/refs/heads/main/openapi/tazama-transaction-monitoring-service-openapi.yml
consequence_counts:
  read: 2
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tazama Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Tazama exposes 6 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Tazama
provider_slug: tazama
slug: tazama-agentic-access
source_filename: tazama-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/tazama-transaction-monitoring-service-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 2\n    acting: 4\n  by_consequence:\n    read: 2\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: getServiceStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: getHealthStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/evaluate/iso20022/pain.001.001.11\n\
  \  method: post\n  operationId: evaluatePain001Transaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/evaluate/iso20022/pain.013.001.09\n  method: post\n  operationId: evaluatePain013Transaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/evaluate/iso20022/pacs.008.001.10\n  method: post\n  operationId: evaluatePacs008Transaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/evaluate/iso20022/pacs.002.001.12\n  method: post\n  operationId: evaluatePacs002Transaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tazama/refs/heads/main/agentic-access/tazama-agentic-access.yml
summary_line: 6 operations · 4 acting
tags:
- Financial Technology
- Fraud Detection
- Anti-Money Laundering
- Linux Foundation
- Open Source
- Transaction Monitoring
- ISO 20022
- Real Time
---
