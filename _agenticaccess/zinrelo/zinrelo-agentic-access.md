---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 13
api_specs:
- filename: zinrelo-openapi.yml
  format: yaml
  label: Zinrelo Members API
  slug: zinrelo-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zinrelo/refs/heads/main/openapi/zinrelo-openapi.yml
- filename: zinrelo-openapi.yml
  format: yaml
  label: Zinrelo Points API
  slug: zinrelo-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zinrelo/refs/heads/main/openapi/zinrelo-openapi.yml
- filename: zinrelo-openapi.yml
  format: yaml
  label: Zinrelo Transactions API
  slug: zinrelo-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zinrelo/refs/heads/main/openapi/zinrelo-openapi.yml
- filename: zinrelo-openapi.yml
  format: yaml
  label: Zinrelo Rewards API
  slug: zinrelo-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zinrelo/refs/heads/main/openapi/zinrelo-openapi.yml
- filename: zinrelo-openapi.yml
  format: yaml
  label: Zinrelo Redemptions API
  slug: zinrelo-redemptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zinrelo/refs/heads/main/openapi/zinrelo-openapi.yml
consequence_counts:
  physical: 1
  read: 13
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Zinrelo Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/loyalty/purchase
operation_count: 22
overview: 'Zinrelo exposes 22 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read, 8 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Zinrelo
provider_slug: zinrelo
slug: zinrelo-agentic-access
source_filename: zinrelo-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/zinrelo-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 13\n    acting: 9\n  by_consequence:\n    read: 13\n    write: 8\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/loyalty/users\n  method: get\n  operationId: listMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/loyalty/users\n  method: post\n  operationId: createMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n   \
  \   human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/loyalty/users/{user_email}\n  method: get\n  operationId: getMember\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/loyalty/users/{user_email}/transactions\n  method: get\n  operationId: listMemberTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/loyalty/users/{user_email}/eligible_activities\n  method: get\n  operationId: listMemberEligibleActivities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/loyalty/users/{user_email}/redemptions\n  method: get\n  operationId: listMemberRedemptions\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/loyalty/users/{user_email}/next_tier\n  method: get\n  operationId: getMemberNextTier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/loyalty/users/{user_email}/block\n  method: put\n  operationId: blockMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/loyalty/update_user_email\n  method: post\n  operationId: updateMemberEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/loyalty/unsubscribe_email\n  method: post\n  operationId: unsubscribeMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/loyalty/unsubscribed_users\n  method: get\n  operationId: listUnsubscribedMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/loyalty/award\n  method: post\n  operationId: awardPoints\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/loyalty/users/deduct\n  method: post\n  operationId: deductPoints\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/loyalty/purchase\n  method: post\n  operationId: recordPurchase\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/loyalty/transaction/return\n  method: post\n  operationId: recordReturn\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/loyalty/transactions\n  method: get\n  operationId: listTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/loyalty-storefront/transactions\n  method: get\n  operationId: listStorefrontTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/loyalty/rewards\n  method: get\n  operationId: listRewards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/loyalty/redemptions\n  method: get\n  operationId: listRedemptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/loyalty/redeem\n  method: post\n  operationId: redeemPoints\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/loyalty/tiers\n  method: get\n  operationId: listTiers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/events/{id}\n  method: get\n  operationId: getEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zinrelo/refs/heads/main/agentic-access/zinrelo-agentic-access.yml
summary_line: 22 operations · 9 acting
tags:
- Loyalty
- Rewards
- Points
- Customer Retention
- Ecommerce
- SaaS
---
