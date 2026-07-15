---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 8
api_specs:
- filename: wtw-hr-portal-openapi.yml
  format: yaml
  label: WTW HR Portal
  slug: wtw-hr-portal
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/towers-watson/refs/heads/main/openapi/wtw-hr-portal-openapi.yml
- filename: wtw-benefits-administration-openapi.yml
  format: yaml
  label: WTW Benefits Administration
  slug: wtw-benefits-administration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/towers-watson/refs/heads/main/openapi/wtw-benefits-administration-openapi.yml
consequence_counts:
  read: 8
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Towers Watson Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Towers Watson exposes 12 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Towers Watson
provider_slug: towers-watson
slug: towers-watson-agentic-access
source_filename: towers-watson-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/wtw-hr-portal-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 8\n    acting: 4\n  by_consequence:\n    read: 8\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /employees\n  method: get\n  operationId: listEmployees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employees/{employeeId}\n  method: get\n  operationId: getEmployee\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employees/{employeeId}/total-rewards\n\
  \  method: get\n  operationId: getEmployeeTotalRewards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /content\n  method: get\n  operationId: listContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /content\n  method: post\n  operationId: createContent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /content/{contentId}\n  method: get\n  operationId: getContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /content/{contentId}\n \
  \ method: put\n  operationId: updateContent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cases\n  method: get\n  operationId: listCases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cases\n  method: post\n  operationId: createCase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cases/{caseId}\n  method: get\n  operationId: getCase\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n \
  \   subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cases/{caseId}\n  method: put\n  operationId: updateCase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /employees/{employeeId}/benefits\n  method: get\n  operationId: getEmployeeBenefits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/towers-watson/refs/heads/main/agentic-access/towers-watson-agentic-access.yml
summary_line: 12 operations · 4 acting
tags:
- Human Resources
- Risk Management
- Benefits
- Consulting
- Actuarial
- Insurance Brokerage
- Human Capital
---
