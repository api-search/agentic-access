---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 5
consequence_counts:
  physical: 1
  read: 5
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Salesforce Commerce Cloud Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /shopper/orders/v1/organizations/{organizationId}/orders
operation_count: 10
overview: 'Salesforce Commerce Cloud exposes 10 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read, 4 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Salesforce Commerce Cloud
provider_slug: salesforce-commerce-cloud
slug: salesforce-commerce-cloud-agentic-access
source_filename: salesforce-commerce-cloud-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/salesforce-commerce-cloud-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    acting: 5\n    connected: 5\n  by_consequence:\n    write: 4\n    read: 5\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /shopper/auth/v1/organizations/{organizationId}/oauth2/token\n  method: post\n  operationId: getSlasToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shopper/products/v1/organizations/{organizationId}/products\n\
  \  method: get\n  operationId: getProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shopper/products/v1/organizations/{organizationId}/products/{id}\n  method: get\n  operationId: getProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shopper/search/v1/organizations/{organizationId}/product-search\n  method: get\n  operationId: productSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shopper/baskets/v1/organizations/{organizationId}/baskets\n  method: post\n  operationId: createBasket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n     \
  \ human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shopper/baskets/v1/organizations/{organizationId}/baskets/{basketId}\n  method: get\n  operationId: getBasket\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shopper/baskets/v1/organizations/{organizationId}/baskets/{basketId}\n  method: delete\n  operationId: deleteBasket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shopper/baskets/v1/organizations/{organizationId}/baskets/{basketId}/items\n  method: post\n  operationId: addItemsToBasket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shopper/orders/v1/organizations/{organizationId}/orders\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shopper/orders/v1/organizations/{organizationId}/orders/{orderNo}\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salesforce-commerce-cloud/refs/heads/main/agentic-access/salesforce-commerce-cloud-agentic-access.yml
summary_line: 10 operations · 5 acting
tags:
- Commerce
- E-Commerce
- Headless Commerce
- Salesforce
- B2C Commerce
- B2B Commerce
- Demandware
---
