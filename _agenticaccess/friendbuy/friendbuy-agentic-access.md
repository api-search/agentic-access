---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 19
api_specs:
- filename: friendbuy-openapi.yml
  format: yaml
  label: Friendbuy Customers API
  slug: friendbuy-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/friendbuy/refs/heads/main/openapi/friendbuy-openapi.yml
- filename: friendbuy-openapi.yml
  format: yaml
  label: Friendbuy Referrals API
  slug: friendbuy-referrals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/friendbuy/refs/heads/main/openapi/friendbuy-openapi.yml
- filename: friendbuy-openapi.yml
  format: yaml
  label: Friendbuy Events API
  slug: friendbuy-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/friendbuy/refs/heads/main/openapi/friendbuy-openapi.yml
- filename: friendbuy-openapi.yml
  format: yaml
  label: Friendbuy Analytics API
  slug: friendbuy-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/friendbuy/refs/heads/main/openapi/friendbuy-openapi.yml
- filename: friendbuy-openapi.yml
  format: yaml
  label: Friendbuy Rewards & Loyalty API
  slug: friendbuy-rewards-loyalty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/friendbuy/refs/heads/main/openapi/friendbuy-openapi.yml
consequence_counts:
  physical: 1
  read: 19
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Friendbuy Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /postPurchaseEvent
operation_count: 31
overview: 'Friendbuy exposes 31 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read, 11 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Friendbuy
provider_slug: friendbuy
slug: friendbuy-agentic-access
source_filename: friendbuy-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/friendbuy-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 31\n  by_action_class:\n    acting: 12\n    connected: 19\n  by_consequence:\n    write: 11\n    read: 19\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /authorization\n  method: post\n  operationId: createAuthorization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /postCustomer\n  method: post\n  operationId: postCustomer\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getCustomer\n  method: get\n  operationId: getCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getMemberTierCustomer\n  method: get\n  operationId: getMemberTierCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getUserData\n  method: get\n  operationId: getUserData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deleteUserData\n  method: delete\n  operationId: deleteUserData\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /postPersonalReferralLink\n  method: post\n  operationId: postPersonalReferralLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /postPersonalReferralLinkBatch\n  method: post\n  operationId: postPersonalReferralLinkBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getReferralStatus\n\
  \  method: get\n  operationId: getReferralStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /postPurchaseEvent\n  method: post\n  operationId: postPurchaseEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /postSignUpEvent\n  method: post\n  operationId: postSignUpEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /postCustomEvent\n  method: post\n\
  \  operationId: postCustomEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analytics/widget-views\n  method: get\n  operationId: getWidgetViews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/shares\n  method: get\n  operationId: getShares\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/clicks\n  method: get\n  operationId: getClicks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/account-sign-ups\n\
  \  method: get\n  operationId: getAccountSignUps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/purchases\n  method: get\n  operationId: getPurchasesAnalytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/distributed-advocate-rewards\n  method: get\n  operationId: getDistributedAdvocateRewards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/distributed-friend-incentives\n  method: get\n  operationId: getDistributedFriendIncentives\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/rewards/referral\n  method: get\n  operationId:\
  \ getReferralRewards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/email-captures\n  method: get\n  operationId: getEmailCaptures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/email-metrics\n  method: get\n  operationId: getEmailMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/loyalty/ledger-heads\n  method: get\n  operationId: getLedgerHeads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ledger-balance\n  method: get\n  operationId: getLedgerBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ledger-balance-custom\n  method: get\n  operationId: getLedgerBalanceCustom\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /postLedgerAdjustment\n  method: post\n  operationId: postLedgerAdjustment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /postLedgerAdjustmentCustom\n  method: post\n  operationId: postLedgerAdjustmentCustom\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /reward/redemption-options\n  method: get\n  operationId: getRedemptionOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reward/redeem\n  method: post\n  operationId: redeemReward\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reward/coupons\n  method: get\n  operationId: getCoupons\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /postBlockUsers\n  method: post\n  operationId: postBlockUsers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/friendbuy/refs/heads/main/agentic-access/friendbuy-agentic-access.yml
summary_line: 31 operations · 12 acting
tags:
- Referral Marketing
- Loyalty
- Rewards
- Ecommerce
- Marketing
- Advocacy
---
