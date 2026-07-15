---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 13
api_specs:
- filename: openapi.yml
  format: yaml
  label: DEGIRO Trading API
  slug: degiro-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/degiro/refs/heads/main/openapi.yml
consequence_counts:
  physical: 3
  read: 13
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Degiro Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /trading/secure/v5/checkOrder;jsessionid={sessionId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /trading/secure/v5/order/{confirmationId};jsessionid={sessionId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /trading/secure/v5/order/{confirmationId};jsessionid={sessionId}
operation_count: 17
overview: 'DEGIRO exposes 17 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read, 1 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: DEGIRO
provider_slug: degiro
slug: degiro-agentic-access
source_filename: degiro-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/degiro-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    acting: 4\n    connected: 13\n  by_consequence:\n    write: 1\n    read: 13\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /login/secure/login\n  method: post\n  operationId: login\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /login/secure/config\n  method: get\n  operationId: config\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pa/secure/client\n  method: get\n  operationId: client\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pa/secure/clienttasks\n  method: get\n  operationId: clienttasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pa/secure/clienttasks/taskmanager/count\n  method: get\n  operationId: clienttasks-taskmanager-count\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pa/secure/settings/beta-test\n  method: get\n  operationId: beta-test\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /pa/secure/settings/iex\n  method: get\n  operationId: iex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pa/secure/settings/user\n  method: get\n  operationId: user\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pa/secure/settings/web\n  method: get\n  operationId: web\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reporting/secure/v4\n  method: get\n  operationId: reporting\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reporting/secure/v4/order_history\n  method: get\n  operationId: orderhistory\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /product_search/secure/v5/products/lookup\n  method: get\n  operationId: lookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trading/secure/v5/account/info/{intAccount};jsessionid={sessionId}\n  method: get\n  operationId: accountInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trading/secure/v5/update/{intAccount};jsessionid={sessionId}\n  method: get\n  operationId: update\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trading/secure/v5/checkOrder;jsessionid={sessionId}\n  method: post\n  operationId: checkOrder\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /trading/secure/v5/order/{confirmationId};jsessionid={sessionId}\n  method: post\n  operationId: confirmOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /trading/secure/v5/order/{confirmationId};jsessionid={sessionId}\n  method: delete\n  operationId: deleteOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/degiro/refs/heads/main/agentic-access/degiro-agentic-access.yml
summary_line: 17 operations · 4 acting
tags:
- Trading
- Brokerage
- Stocks
- ETFs
- Portfolio
- Market Data
- Finance
---
