---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 6
api_specs:
- filename: loyaltylion-openapi.yml
  format: yaml
  label: LoyaltyLion Customers API
  slug: loyaltylion-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loyaltylion/refs/heads/main/openapi/loyaltylion-openapi.yml
- filename: loyaltylion-openapi.yml
  format: yaml
  label: LoyaltyLion Activities API
  slug: loyaltylion-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loyaltylion/refs/heads/main/openapi/loyaltylion-openapi.yml
- filename: loyaltylion-openapi.yml
  format: yaml
  label: LoyaltyLion Points API
  slug: loyaltylion-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loyaltylion/refs/heads/main/openapi/loyaltylion-openapi.yml
- filename: loyaltylion-openapi.yml
  format: yaml
  label: LoyaltyLion Rewards API
  slug: loyaltylion-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loyaltylion/refs/heads/main/openapi/loyaltylion-openapi.yml
- filename: loyaltylion-openapi.yml
  format: yaml
  label: LoyaltyLion Redemptions API
  slug: loyaltylion-redemptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loyaltylion/refs/heads/main/openapi/loyaltylion-openapi.yml
consequence_counts:
  physical: 1
  read: 6
  safety-critical: 1
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Loyaltylion Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /rewards/{reward_id}/disable
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /customers/{merchant_id}/claimed_rewards/{claimed_reward_id}/refund
operation_count: 15
overview: 'LoyaltyLion exposes 15 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 7 write, 1 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: LoyaltyLion
provider_slug: loyaltylion
slug: loyaltylion-agentic-access
source_filename: loyaltylion-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/loyaltylion-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 6\n    acting: 9\n  by_consequence:\n    read: 6\n    write: 7\n    physical: 1\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /whoami\n  method: get\n  operationId: whoAmI\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers\n  method: get\n  operationId: listCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{merchant_id}\n\
  \  method: put\n  operationId: updateCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{merchant_id}/transactions\n  method: get\n  operationId: listCustomerTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{merchant_id}/points\n  method: post\n  operationId: addPoints\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{merchant_id}/remove_points\n  method: post\n  operationId:\
  \ removePoints\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{merchant_id}/available_rewards\n  method: get\n  operationId: listAvailableRewards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{merchant_id}/claimed_rewards\n  method: post\n  operationId: redeemReward\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{merchant_id}/claimed_rewards/{claimed_reward_id}/refund\n  method:\
  \ post\n  operationId: refundReward\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /activities\n  method: get\n  operationId: listActivities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /activities\n  method: post\n  operationId: createActivity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /activities/{merchant_id}\n  method: put\n  operationId: updateActivity\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transactions\n  method: get\n  operationId: listTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rewards/{reward_id}/enable\n  method: post\n  operationId: enableReward\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rewards/{reward_id}/disable\n  method: post\n  operationId: disableReward\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loyaltylion/refs/heads/main/agentic-access/loyaltylion-agentic-access.yml
summary_line: 15 operations · 9 acting · 1 human-in-the-loop
tags:
- Loyalty
- Rewards
- E-commerce
- Points
- Shopify
- Retention
---
