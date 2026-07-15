---
acting_count: 21
action_class_counts:
  acting: 21
  connected: 15
api_specs:
- filename: open-loyalty-openapi.yml
  format: yaml
  label: Open Loyalty Customer API
  slug: open-loyalty-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-loyalty/refs/heads/main/openapi/open-loyalty-openapi.yml
- filename: open-loyalty-openapi.yml
  format: yaml
  label: Open Loyalty Transactions API
  slug: open-loyalty-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-loyalty/refs/heads/main/openapi/open-loyalty-openapi.yml
- filename: open-loyalty-openapi.yml
  format: yaml
  label: Open Loyalty Points Transfers API
  slug: open-loyalty-points-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-loyalty/refs/heads/main/openapi/open-loyalty-openapi.yml
- filename: open-loyalty-openapi.yml
  format: yaml
  label: Open Loyalty Reward Campaigns API
  slug: open-loyalty-reward-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-loyalty/refs/heads/main/openapi/open-loyalty-openapi.yml
- filename: open-loyalty-openapi.yml
  format: yaml
  label: Open Loyalty Levels API
  slug: open-loyalty-levels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-loyalty/refs/heads/main/openapi/open-loyalty-openapi.yml
- filename: open-loyalty-openapi.yml
  format: yaml
  label: Open Loyalty Earning Rules API
  slug: open-loyalty-earning-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-loyalty/refs/heads/main/openapi/open-loyalty-openapi.yml
consequence_counts:
  physical: 4
  read: 15
  write: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Open Loyalty Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{storeCode}/customer/points/p2p-transfer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{storeCode}/points/transfer/add
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{storeCode}/points/transfer/spend
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{storeCode}/points/transfer/{transfer}/cancel
operation_count: 36
overview: 'Open Loyalty exposes 36 API operations that an AI agent could call, of which 21 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read, 17 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Open Loyalty
provider_slug: open-loyalty
slug: open-loyalty-agentic-access
source_filename: open-loyalty-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/open-loyalty-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 36\n  by_action_class:\n    acting: 21\n    connected: 15\n  by_consequence:\n    write: 17\n    read: 15\n    physical: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /admin/login_check\n  method: post\n  operationId: adminLogin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{storeCode}/customer/login_check\n  method: post\n  operationId: customerLogin\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{storeCode}/customer/register\n  method: post\n  operationId: registerCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{storeCode}/customer\n  method: get\n  operationId: listCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{storeCode}/customer/check\n  method: get\n  operationId: checkCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{storeCode}/customer/{customer}\n  method: get\n  operationId: getCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{storeCode}/customer/{customer}\n  method: put\n  operationId: updateCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{storeCode}/customer/{customer}/level\n  method: post\n  operationId: assignCustomerLevel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /{storeCode}/admin/customer/{customer}/history\n  method: get\n  operationId: getCustomerHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{storeCode}/transaction\n  method: get\n  operationId: listTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{storeCode}/transaction\n  method: post\n  operationId: registerTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{storeCode}/transaction/simulate\n  method: post\n  operationId: simulateTransaction\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{storeCode}/transaction/{transaction}\n  method: get\n  operationId: getTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{storeCode}/customer/transaction/customer/assign\n  method: post\n  operationId: assignTransactionToCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{storeCode}/points/transfer\n  method: get\n  operationId: listPointsTransfers\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{storeCode}/points/transfer/add\n  method: post\n  operationId: addPoints\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{storeCode}/points/transfer/spend\n  method: post\n  operationId: spendPoints\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{storeCode}/customer/points/p2p-transfer\n\
  \  method: post\n  operationId: p2pTransferPoints\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{storeCode}/points/transfer/{transfer}/cancel\n  method: post\n  operationId: cancelPointsTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{storeCode}/campaign\n  method: get\n  operationId: listCampaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /{storeCode}/campaign\n  method: post\n  operationId: createCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{storeCode}/campaign/active\n  method: get\n  operationId: listActiveCampaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{storeCode}/campaign/{campaign}\n  method: get\n  operationId: getCampaign\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{storeCode}/campaign/{campaign}\n  method: put\n  operationId: updateCampaign\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{storeCode}/admin/customer/{customer}/campaign/{campaign}/buy\n  method: post\n  operationId: buyCampaignForCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{storeCode}/level\n  method: get\n  operationId: listLevels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{storeCode}/level/create\n  method: post\n  operationId: createLevel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{storeCode}/level/{level}\n  method: get\n  operationId: getLevel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{storeCode}/level/{level}\n  method: put\n  operationId: updateLevel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{storeCode}/level/{level}\n  method: delete\n  operationId: deleteLevel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{storeCode}/level/{level}/customers\n  method: get\n  operationId: listLevelCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{storeCode}/earningRule\n  method: get\n  operationId: listEarningRules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{storeCode}/earningRule\n  method: post\n  operationId: createEarningRule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{storeCode}/earningRule/{earningRule}\n\
  \  method: get\n  operationId: getEarningRule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{storeCode}/earningRule/{earningRule}\n  method: put\n  operationId: updateEarningRule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{storeCode}/earningRule/{earningRule}/activate\n  method: post\n  operationId: activateEarningRule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-loyalty/refs/heads/main/agentic-access/open-loyalty-agentic-access.yml
summary_line: 36 operations · 21 acting
tags:
- Loyalty
- Gamification
- Rewards
- Points
- Loyalty Program
- Customer Engagement
- Headless
- API First
---
