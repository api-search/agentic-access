---
acting_count: 0
action_class_counts:
  connected: 5
api_specs:
- filename: saas-alerts-events-api-openapi.yml
  format: yaml
  label: SaaS Alerts Events API
  slug: saas-alerts-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saas-alerts/refs/heads/main/openapi/saas-alerts-events-api-openapi.yml
- filename: saas-alerts-reports-api-openapi.yml
  format: yaml
  label: SaaS Alerts Reports API
  slug: saas-alerts-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saas-alerts/refs/heads/main/openapi/saas-alerts-reports-api-openapi.yml
consequence_counts:
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Saas Alerts Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'SaaS Alerts exposes 5 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SaaS Alerts
provider_slug: saas-alerts
slug: saas-alerts-agentic-access
source_filename: saas-alerts-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/saas-alerts-events-api-openapi.yml, openapi/saas-alerts-reports-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 5\n  by_consequence:\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /reports/events\n  method: get\n  operationId: listSecurityEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/event/query\n  method: post\n  operationId: querySecurityEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /reports/alerts\n  method: get\n  operationId: listAlerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/customers\n  method: get\n  operationId: listCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/saas-alerts/refs/heads/main/agentic-access/saas-alerts-agentic-access.yml
summary_line: 5 operations
tags:
- MSP
- SaaS Security
- Security Monitoring
- Threat Detection
- Microsoft 365
- Google Workspace
- MSSP
---
