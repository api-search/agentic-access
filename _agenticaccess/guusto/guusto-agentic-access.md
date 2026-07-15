---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 7
api_specs:
- filename: guusto-openapi.yml
  format: yaml
  label: Guusto Gifts API
  slug: guusto-gifts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guusto/refs/heads/main/openapi/guusto-openapi.yml
- filename: guusto-openapi.yml
  format: yaml
  label: Guusto Account Budget API
  slug: guusto-account-budget-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guusto/refs/heads/main/openapi/guusto-openapi.yml
- filename: guusto-openapi.yml
  format: yaml
  label: Guusto Reports API
  slug: guusto-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guusto/refs/heads/main/openapi/guusto-openapi.yml
consequence_counts:
  physical: 1
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Guusto Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders
operation_count: 8
overview: 'Guusto exposes 8 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Guusto
provider_slug: guusto
slug: guusto-agentic-access
source_filename: guusto-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/guusto-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 1\n    connected: 7\n  by_consequence:\n    physical: 1\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /orders\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/status/{requestId}\n  method: get\n  operationId: getOrderStatus\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{requestId}\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /balances/workspaces/currencies/{currency}\n  method: get\n  operationId: getWorkspaceBudget\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /balances/members/{employeeNumber}/currencies/{currency}\n  method: get\n  operationId: getMemberBudget\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /balances/members/currencies/{currency}\n  method: get\n  operationId: listMemberBudgets\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/teams/activity\n  method: get\n  operationId: getTeamActivity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/members/last-recognized\n  method: get\n  operationId: getLastRecognized\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/guusto/refs/heads/main/agentic-access/guusto-agentic-access.yml
summary_line: 8 operations · 1 acting
tags:
- Employee Recognition
- Rewards
- Gifting
- Gift Cards
- HR
- Rewards and Recognition
---
