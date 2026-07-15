---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 10
api_specs:
- filename: smile-io-openapi.yml
  format: yaml
  label: Smile.io Customers API
  slug: smile-io-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smile-io/refs/heads/main/openapi/smile-io-openapi.yml
- filename: smile-io-openapi.yml
  format: yaml
  label: Smile.io Points Transactions API
  slug: smile-io-points-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smile-io/refs/heads/main/openapi/smile-io-openapi.yml
- filename: smile-io-openapi.yml
  format: yaml
  label: Smile.io Points Products API
  slug: smile-io-points-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smile-io/refs/heads/main/openapi/smile-io-openapi.yml
- filename: smile-io-openapi.yml
  format: yaml
  label: Smile.io Reward Fulfillments API
  slug: smile-io-rewards-fulfillments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smile-io/refs/heads/main/openapi/smile-io-openapi.yml
- filename: smile-io-openapi.yml
  format: yaml
  label: Smile.io Earning Rules API
  slug: smile-io-earning-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smile-io/refs/heads/main/openapi/smile-io-openapi.yml
- filename: smile-io-openapi.yml
  format: yaml
  label: Smile.io VIP Tiers API
  slug: smile-io-vip-tiers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smile-io/refs/heads/main/openapi/smile-io-openapi.yml
- filename: smile-io-openapi.yml
  format: yaml
  label: Smile.io Activities API
  slug: smile-io-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smile-io/refs/heads/main/openapi/smile-io-openapi.yml
consequence_counts:
  physical: 1
  read: 10
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Smile Io Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /points_products/{id}/purchase
operation_count: 14
overview: 'Smile.io exposes 14 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read, 3 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Smile.io
provider_slug: smile-io
slug: smile-io-agentic-access
source_filename: smile-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/smile-io-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    acting: 4\n    connected: 10\n  by_consequence:\n    write: 3\n    read: 10\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /activities\n  method: post\n  operationId: post__activities\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /earning_rules\n  method: get\n  operationId: get__earning_rules\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reward_fulfillments\n  method: get\n  operationId: get__reward_fulfillments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer_identities/create_or_update\n  method: post\n  operationId: post__customer_identities_create_or_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /points_products/{id}/purchase\n  method: post\n  operationId: post__points_products_id_purchase\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n    \
  \  exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /points_products\n  method: get\n  operationId: get__points_products\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /points_products/{id}\n  method: get\n  operationId: get__points_products_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /points_transactions\n  method: post\n  operationId: post__points_transactions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /points_transactions\n  method: get\n  operationId: get__points_transactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /points_transactions/{id}\n  method: get\n  operationId: get__points_transactions_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vip_tiers\n  method: get\n  operationId: get__vip_tiers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /points_settings\n  method: get\n  operationId: get__points_settings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{id}\n  method: get\n  operationId: get__customers_id\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers\n  method: get\n  operationId: get__customers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smile-io/refs/heads/main/agentic-access/smile-io-agentic-access.yml
summary_line: 14 operations · 4 acting
tags:
- Loyalty
- Rewards
- Referrals
- E-commerce
- Points
- Customer Retention
- Shopify
---
