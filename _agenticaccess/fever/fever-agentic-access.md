---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 6
api_specs:
- filename: fever-reporting-api-openapi-original.json
  format: json
  label: Fever Reporting API
  slug: fever-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fever/refs/heads/main/openapi/fever-reporting-api-openapi-original.json
consequence_counts:
  physical: 1
  read: 6
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Fever Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /reports/order-items/search
operation_count: 13
overview: 'Fever exposes 13 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 6 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Fever
provider_slug: fever
slug: fever-agentic-access
source_filename: fever-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/fever-reporting-api-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    acting: 7\n    connected: 6\n  by_consequence:\n    write: 6\n    read: 6\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /auth/token\n  method: post\n  operationId: create_token_auth_token_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /plans/search\n  method: post\n  operationId: search_plans_plans_search_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /plans/search/{search_id}\n  method: get\n  operationId: get_plans_search_page_plans_search__search_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions/search\n  method: post\n  operationId: search_sessions_sessions_search_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/search/{search_id}\n  method: get\n  operationId: get_sessions_search_page_sessions_search__search_id__get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feverzone/sales-summary/search\n  method: post\n  operationId: search_sales_summary_feverzone_sales_summary_search_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feverzone/sales-summary/search/{search_id}\n  method: get\n  operationId: get_search_sales_summary_page_feverzone_sales_summary_search__search_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feverzone/sales-by-ticket-type/search\n  method: post\n  operationId: search_sales_by_ticket_type_feverzone_sales_by_ticket_type_search_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feverzone/sales-by-ticket-type/search/{search_id}\n  method: get\n  operationId: get_search_sales_by_ticket_type_page_feverzone_sales_by_ticket_type_search__search_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feverzone/sales-by-reseller/search\n  method: post\n  operationId: search_resellers_feverzone_sales_by_reseller_search_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n   \
  \ audit: required\n- path: /feverzone/sales-by-reseller/search/{search_id}\n  method: get\n  operationId: get_resellers_search_page_feverzone_sales_by_reseller_search__search_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/order-items/search\n  method: post\n  operationId: search_order_items_reports_order_items_search_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reports/order-items/search/{search_id}\n  method: get\n  operationId: get_order_items_search_page_reports_order_items_search__search_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fever/refs/heads/main/agentic-access/fever-agentic-access.yml
summary_line: 13 operations · 7 acting
tags:
- Company
- Consumer
- Live Entertainment
- Events
- Ticketing
- Experiences
- Reporting
- MCP
---
