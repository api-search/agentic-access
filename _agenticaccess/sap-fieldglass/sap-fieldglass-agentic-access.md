---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 11
api_specs:
- filename: sap-fieldglass-approval-openapi.yaml
  format: yaml
  label: SAP Fieldglass Approval API
  slug: sap-fieldglass-approval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-fieldglass/refs/heads/main/openapi/sap-fieldglass-approval-openapi.yaml
- filename: sap-fieldglass-odata-analytic-openapi.json
  format: json
  label: SAP Fieldglass OData-Based Analytic API
  slug: sap-fieldglass-odata-based-analytic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-fieldglass/refs/heads/main/openapi/sap-fieldglass-odata-analytic-openapi.json
- filename: sap-fieldglass-background-check-openapi.json
  format: json
  label: SAP Fieldglass Background Check API
  slug: sap-fieldglass-background-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-fieldglass/refs/heads/main/openapi/sap-fieldglass-background-check-openapi.json
- filename: sap-fieldglass-audit-trail-openapi.json
  format: json
  label: SAP Fieldglass Audit Trail API
  slug: sap-fieldglass-audit-trail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-fieldglass/refs/heads/main/openapi/sap-fieldglass-audit-trail-openapi.json
- filename: sap-fieldglass-business-analytics-openapi.json
  format: json
  label: SAP Fieldglass Business Analytics API
  slug: sap-fieldglass-business-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-fieldglass/refs/heads/main/openapi/sap-fieldglass-business-analytics-openapi.json
consequence_counts:
  physical: 2
  read: 11
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sap Fieldglass Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /order_confirmation
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /result
operation_count: 14
overview: 'SAP Fieldglass exposes 14 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 1 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SAP Fieldglass
provider_slug: sap-fieldglass
slug: sap-fieldglass-agentic-access
source_filename: sap-fieldglass-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/sap-fieldglass-approval-openapi.yaml, openapi/sap-fieldglass-audit-trail-openapi.json,\n  openapi/sap-fieldglass-background-check-openapi.json, openapi/sap-fieldglass-business-analytics-openapi.json,\n  openapi/sap-fieldglass-odata-analytic-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 11\n    acting: 3\n  by_consequence:\n    read: 11\n    write: 1\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /approvals\n  method: get\n  operationId: getItemListForApproval\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  \    scope:\n    - user\n- path: /approvals/module_{moduleId}\n  method: get\n  operationId: getItemListFroApprovalByModule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - user\n- path: /approvals/module_{moduleId}/{workItemId}/action/{action}\n  method: post\n  operationId: approveOrRejectItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - user\n- path: /approvals/module_{moduleId}/{workItemId}\n  method: get\n  operationId: getWorkItemDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - user\n- path: /approvals/reject_reasons/module_{moduleId}\n\
  \  method: get\n  operationId: getRejectionReasons\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - user\n- path: /auditTrail\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - user\n- path: /order_confirmation\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - user\n- path: /result\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - user\n- path: /report\n  method: get\n  operationId: getReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /report/{report_id}\n  method: get\n  operationId: getReportById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Providers\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{ProviderID}/$metadata\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    scope:\n    - user\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{ServiceURL}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{ProviderID}/{entityName}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - user\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-fieldglass/refs/heads/main/agentic-access/sap-fieldglass-agentic-access.yml
summary_line: 14 operations · 3 acting
tags:
- Contingent Workforce
- External Talent
- Human Capital Management
- Services Procurement
- Statements of Work
- Vendor Management
- Workforce Management
---
