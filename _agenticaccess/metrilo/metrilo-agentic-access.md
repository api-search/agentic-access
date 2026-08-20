---
acting_count: 10
action_class_counts:
  acting: 10
api_specs:
- filename: metrilo-categories-api-openapi.yml
  format: yaml
  label: Metrilo Categories API
  slug: metrilo-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metrilo/refs/heads/main/openapi/metrilo-categories-api-openapi.yml
- filename: metrilo-customers-api-openapi.yml
  format: yaml
  label: Metrilo Customers API
  slug: metrilo-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metrilo/refs/heads/main/openapi/metrilo-customers-api-openapi.yml
- filename: metrilo-orders-api-openapi.yml
  format: yaml
  label: Metrilo Orders API
  slug: metrilo-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metrilo/refs/heads/main/openapi/metrilo-orders-api-openapi.yml
- filename: metrilo-products-api-openapi.yml
  format: yaml
  label: Metrilo Products API
  slug: metrilo-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metrilo/refs/heads/main/openapi/metrilo-products-api-openapi.yml
- filename: metrilo-tracking-api-openapi.yml
  format: yaml
  label: Metrilo Tracking API
  slug: metrilo-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metrilo/refs/heads/main/openapi/metrilo-tracking-api-openapi.yml
consequence_counts:
  physical: 2
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Metrilo Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /order/batch
operation_count: 10
overview: 'Metrilo exposes 10 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 write and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Metrilo
provider_slug: metrilo
slug: metrilo-agentic-access
source_filename: metrilo-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: generated\nsource: openapi/metrilo-categories-api-openapi.yml, openapi/metrilo-customers-api-openapi.yml,\n  openapi/metrilo-orders-api-openapi.yml, openapi/metrilo-products-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    acting: 10\n  by_consequence:\n    write: 8\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /category\n  method: post\n  operationId: createCategory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /category/batch\n  method: post\n  operationId: batchCategories\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer\n  method: post\n  operationId: createCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer/batch\n  method: post\n  operationId: batchCustomers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /customer/tag\n  method: post\n  operationId: tagCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer/untag\n  method: post\n  operationId: untagCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /order\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /order/batch\n  method: post\n  operationId: batchOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /product\n  method: post\n  operationId: createProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /product/batch\n  method: post\n  operationId: batchProducts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metrilo/refs/heads/main/agentic-access/metrilo-agentic-access.yml
summary_line: 10 operations · 10 acting
tags:
- Company
- E-Commerce
- Analytics
- CRM
- Email Marketing
- Customer Retention
- Tracking
- Marketing
---
