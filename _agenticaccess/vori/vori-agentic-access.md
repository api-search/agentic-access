---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 6
api_specs:
- filename: vori-openapi.yml
  format: yaml
  label: Vori API
  slug: vori-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vori/refs/heads/main/openapi/vori-openapi.yml
consequence_counts:
  read: 6
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Vori Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Vori exposes 9 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Vori
provider_slug: vori
slug: vori-agentic-access
source_filename: vori-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/vori-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    acting: 3\n    connected: 6\n  by_consequence:\n    write: 3\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/store-products\n  method: post\n  operationId: createStoreProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/store-products\n  method: get\n  operationId: listStoreProducts\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/store-products/{id}/rules\n  method: get\n  operationId: getProcessedStoreProductRule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/store-products/{id}\n  method: get\n  operationId: getStoreProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/store-products/{id}\n  method: patch\n  operationId: updateStoreProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/store-products/rules\n  method: get\n  operationId: listProcessedStoreProductRules\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/store-products/{id}/history\n  method: get\n  operationId: listStoreProductHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/store-products/{id}/restore\n  method: post\n  operationId: restoreStoreProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/store-products/search\n  method: get\n  operationId: searchStoreProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vori/refs/heads/main/agentic-access/vori-agentic-access.yml
summary_line: 9 operations · 3 acting
tags:
- Company
- Applications
- Grocery
- Point of Sale
- Retail
- Inventory
- Payments
- Commerce
---
