---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 9
api_specs:
- filename: stay-ai-openapi.yml
  format: yaml
  label: Stay AI Subscriptions API
  slug: stay-ai-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stay-ai/refs/heads/main/openapi/stay-ai-openapi.yml
- filename: stay-ai-openapi.yml
  format: yaml
  label: Stay AI Subscription Orders API
  slug: stay-ai-subscription-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stay-ai/refs/heads/main/openapi/stay-ai-openapi.yml
- filename: stay-ai-openapi.yml
  format: yaml
  label: Stay AI Selling Plans API
  slug: stay-ai-selling-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stay-ai/refs/heads/main/openapi/stay-ai-openapi.yml
- filename: stay-ai-openapi.yml
  format: yaml
  label: Stay AI Catalog API
  slug: stay-ai-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stay-ai/refs/heads/main/openapi/stay-ai-openapi.yml
- filename: stay-ai-openapi.yml
  format: yaml
  label: Stay AI Customer Portal API
  slug: stay-ai-customer-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stay-ai/refs/heads/main/openapi/stay-ai-openapi.yml
- filename: stay-ai-openapi.yml
  format: yaml
  label: Stay AI Webhooks API
  slug: stay-ai-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stay-ai/refs/heads/main/openapi/stay-ai-openapi.yml
- filename: stay-ai-openapi.yml
  format: yaml
  label: Stay AI Account and Data API
  slug: stay-ai-account-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stay-ai/refs/heads/main/openapi/stay-ai-openapi.yml
consequence_counts:
  physical: 3
  read: 9
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Stay Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /subscriptions/{subscriptionId}/get-order-now
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /subscriptions/{subscriptionId}/order-notes
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /subscriptions/{subscriptionId}/set-shipping-address
operation_count: 23
overview: 'Stay AI exposes 23 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 11 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Stay AI
provider_slug: stay-ai
slug: stay-ai-agentic-access
source_filename: stay-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/stay-ai-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 9\n    acting: 14\n  by_consequence:\n    read: 9\n    write: 11\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /subscriptions\n  method: get\n  operationId: query-all-subscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/{subscriptionId}\n  method: get\n  operationId: query-subscription-by-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /subscriptions/{subscriptionId}/cancel\n  method: post\n  operationId: cancel-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/{subscriptionId}/change-frequency\n  method: post\n  operationId: change-frequency\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/{subscriptionId}/get-order-now\n  method: post\n  operationId: create-subscription-order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/{subscriptionId}/lines/{lineId}\n  method: put\n  operationId: update-line\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/{subscriptionId}/remove-lines\n  method: post\n  operationId: remove-lines\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/{subscriptionId}/order-notes\n\
  \  method: put\n  operationId: update-order-notes\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/{subscriptionId}/meta-data\n  method: post\n  operationId: add-meta-data\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/{subscriptionId}/set-shipping-address\n  method: post\n  operationId: set-shipping-address\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/generate-portal-link\n  method: post\n  operationId: generate-portal-link\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders\n  method: get\n  operationId: query-orders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /selling-plan-groups\n  method: get\n  operationId: query-selling-plan-groups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /selling-plan-groups\n  method: post\n  operationId: create-selling-plan-group\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /selling-plan-groups/{sellingPlanGroupId}\n  method: get\n  operationId: query-selling-plan-group-by-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /selling-plan-groups/{sellingPlanGroupId}\n  method: put\n  operationId: update-selling-plan-group\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /products/catalog\n  method: get\n  operationId: get-catalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/{productId}\n  method: get\n  operationId: get-catalog-product-by-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /settings\n  method: get\n  operationId: query-account-settings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/export\n  method: post\n  operationId: export-data\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /webhooks\n  method: get\n  operationId: get-webhook-subscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: post\n  operationId: create-webhook-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{webhookId}\n  method: delete\n  operationId: delete-webhook-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stay-ai/refs/heads/main/agentic-access/stay-ai-agentic-access.yml
summary_line: 23 operations · 14 acting
tags:
- Subscriptions
- Retention
- Churn
- Shopify
- Ecommerce
- DTC
---
