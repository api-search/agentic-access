---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 7
api_specs:
- filename: subex-revenue-assurance-openapi.yml
  format: yaml
  label: Subex Revenue Assurance & Fraud Management API
  slug: subex-revenue-assurance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/subex/refs/heads/main/openapi/subex-revenue-assurance-openapi.yml
consequence_counts:
  read: 7
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Subex Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Subex exposes 8 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Subex
provider_slug: subex
slug: subex-agentic-access
source_filename: subex-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/subex-revenue-assurance-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 7\n    acting: 1\n  by_consequence:\n    read: 7\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /revenue-assurance/leakages\n  method: get\n  operationId: listLeakageAlerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /revenue-assurance/leakages/{leakageId}\n  method: get\n  operationId: getLeakageAlert\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n \
  \   audit: none\n- path: /revenue-assurance/leakages/{leakageId}\n  method: patch\n  operationId: updateLeakageAlert\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fraud/cases\n  method: get\n  operationId: listFraudCases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fraud/cases/{caseId}\n  method: get\n  operationId: getFraudCase\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fraud/subscribers/{msisdn}/risk-score\n  method: get\n  operationId: getSubscriberRiskScore\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reconciliation/runs\n  method: get\n  operationId: listReconciliationRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/summary\n  method: get\n  operationId: getAnalyticsSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/subex/refs/heads/main/agentic-access/subex-agentic-access.yml
summary_line: 8 operations · 1 acting
tags:
- Telecom
- Revenue Assurance
- Fraud Management
- Analytics
- BSS/OSS
---
