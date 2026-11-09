---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 1
api_specs:
- filename: amzscout-net-discovery-api-openapi.yml
  format: yaml
  label: AMZScout Discovery API
  slug: amzscout-net-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amzscout-net/openapi/amzscout-net-discovery-api-openapi.yml
- filename: amzscout-net-dispatch-api-openapi.yml
  format: yaml
  label: AMZScout Dispatch API
  slug: amzscout-net-dispatch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amzscout-net/openapi/amzscout-net-dispatch-api-openapi.yml
- filename: amzscout-net-tools-api-openapi.yml
  format: yaml
  label: AMZScout Tools API
  slug: amzscout-net-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amzscout-net/openapi/amzscout-net-tools-api-openapi.yml
consequence_counts:
  physical: 3
  read: 1
  safety-critical: 1
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Amzscout Net Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/tools/call
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/tools/call/amzscout_reseller_amazon
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/tools/call/amzscout_search_products
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/tools/call/amzscout_usage
operation_count: 16
overview: 'AMZScout exposes 16 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read, 11 write, 3 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AMZScout
provider_slug: amzscout-net
slug: amzscout-net-agentic-access
source_filename: amzscout-net-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/chatbot-amzscout-net-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 1\n    acting: 15\n  by_consequence:\n    read: 1\n    safety-critical: 1\n    write: 11\n    physical: 3\n  human_in_the_loop_required: 1\noperations:\n- path: /api/v1/tools/list\n  method: post\n  operationId: listTools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tools/call\n  method: post\n  operationId: callTool\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/tools/call/amzscout_analyze_product\n  method: post\n  operationId: call_amzscout_analyze_product\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/call/amzscout_analyze_niche\n  method: post\n  operationId: call_amzscout_analyze_niche\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/call/amzscout_compare_products\n\
  \  method: post\n  operationId: call_amzscout_compare_products\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/call/amzscout_compare_niches\n  method: post\n  operationId: call_amzscout_compare_niches\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/call/amzscout_analyze_product_set\n  method: post\n  operationId: call_amzscout_analyze_product_set\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/call/amzscout_reseller_amazon\n  method: post\n  operationId: call_amzscout_reseller_amazon\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/call/amzscout_advanced_product_data\n  method: post\n  operationId: call_amzscout_advanced_product_data\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/call/amzscout_search_products\n\
  \  method: post\n  operationId: call_amzscout_search_products\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/call/amzscout_find_by_brand\n  method: post\n  operationId: call_amzscout_find_by_brand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/call/amzscout_get_keywords\n  method: post\n  operationId: call_amzscout_get_keywords\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/call/amzscout_search_knowledge\n  method: post\n  operationId: call_amzscout_search_knowledge\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/call/amzscout_recommend_tool\n  method: post\n  operationId: call_amzscout_recommend_tool\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/call/amzscout_usage\n \
  \ method: post\n  operationId: call_amzscout_usage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/call/amzscout_locate_asin\n  method: post\n  operationId: call_amzscout_locate_asin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/amzscout-net/agentic-access/amzscout-net-agentic-access.yml
summary_line: 16 operations · 15 acting · 1 human-in-the-loop
tags:
- Amazon
- FBA
- Product Research
- Software-as-a-Service
- E-Commerce
- Company
---
