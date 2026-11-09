---
acting_count: 10
action_class_counts:
  acting: 10
api_specs:
- filename: 402oracle-com-verify-api-openapi.yml
  format: yaml
  label: 402 Oracle Verify API
  slug: 402oracle-com-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/402oracle-com/openapi/402oracle-com-verify-api-openapi.yml
consequence_counts:
  physical: 6
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: 402Oracle Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /verify/business
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /verify/business
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /verify/business/batch
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /verify/business/batch
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /verify/price
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /verify/price
operation_count: 10
overview: '402 Oracle exposes 10 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 write and 6 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: 402 Oracle
provider_slug: 402oracle-com
slug: 402oracle-com-agentic-access
source_filename: 402oracle-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/402oracle-com-openapi.json, openapi/402oracle-com.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    acting: 10\n  by_consequence:\n    physical: 6\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /verify/business\n  method: post\n  operationId: verify_business\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verify/price\n  method: post\n  operationId:\
  \ verify_price\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verify/freshness\n  method: post\n  operationId: verify_freshness\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verify/claim\n  method: post\n  operationId: verify_claim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /verify/business/batch\n  method: post\n  operationId: verify_business_batch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verify/business\n  method: post\n  operationId: verify_business\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verify/price\n  method: post\n  operationId: verify_price\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verify/freshness\n  method: post\n  operationId: verify_freshness\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verify/claim\n  method: post\n  operationId: verify_claim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verify/business/batch\n  method: post\n\
  \  operationId: verify_business_batch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/402oracle-com/agentic-access/402oracle-com-agentic-access.yml
summary_line: 10 operations · 10 acting
tags:
- Verification
- Blockchain
- Artificial Intelligence
- Trust
- Finance
---
