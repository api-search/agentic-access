---
acting_count: 32
action_class_counts:
  acting: 32
api_specs:
- filename: gallop-data-openapi.json
  format: json
  label: Gallop Data API
  slug: gallop-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gallop/refs/heads/main/openapi/gallop-data-openapi.json
- filename: gallop-analytics-openapi.json
  format: json
  label: Gallop Analytics API
  slug: gallop-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gallop/refs/heads/main/openapi/gallop-analytics-openapi.json
- filename: gallop-insights-openapi.json
  format: json
  label: Gallop Insights API
  slug: gallop-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gallop/refs/heads/main/openapi/gallop-insights-openapi.json
consequence_counts:
  physical: 6
  write: 26
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Gallop Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /analytics/eth/getWashTrade
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /analytics/eth/getWashTransactions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /analytics/pol/getWashTrade
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /analytics/pol/getWashTransactions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /analytics/sol/getWashTrade
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /analytics/sol/getWashTransactions
operation_count: 32
overview: 'Gallop exposes 32 API operations that an AI agent could call, of which 32 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 26 write and 6 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Gallop
provider_slug: gallop
slug: gallop-agentic-access
source_filename: gallop-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/gallop-analytics-openapi.json, openapi/gallop-insights-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 32\n  by_action_class:\n    acting: 32\n  by_consequence:\n    write: 26\n    physical: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /analytics/eth/getCollectionListingsOHLC\n  method: post\n  operationId: getEthCollectionListingsOHLC\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analytics/eth/getCollectionPriceDiff\n  method:\
  \ post\n  operationId: getEthCollectionPriceDiff\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analytics/eth/getCollectionSalesOHLC\n  method: post\n  operationId: getEthCollectionSalesOHLC\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analytics/eth/getCollectionSummary\n  method: post\n  operationId: getEthCollectionSummary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analytics/eth/getDailyCollectionFloor\n  method: post\n  operationId: getEthDailyCollectionFloor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analytics/eth/getLeaderBoard\n  method: post\n  operationId: getEthLeaderBoard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analytics/eth/getRarity\n  method: post\n  operationId: getEthRarity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analytics/eth/getTokenSummary\n  method: post\n  operationId: getEthTokenSummary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analytics/eth/getWalletPnL\n  method: post\n  operationId: getEthWalletPnL\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analytics/eth/getWashTrade\n  method: post\n  operationId: getEthWashTrade\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analytics/eth/getWashTransactions\n  method: post\n  operationId: getEthWashTransactions\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analytics/pol/getCollectionPriceDiff\n  method: post\n  operationId: getPolCollectionPriceDiff\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n    \
  \  max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analytics/pol/getCollectionSalesOHLC\n  method: post\n  operationId: getPolCollectionSalesOHLC\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analytics/pol/getCollectionSummary\n  method: post\n  operationId: getPolCollectionSummary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analytics/pol/getLeaderBoard\n  method: post\n  operationId: getPolLeaderBoard\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analytics/pol/getRarity\n  method: post\n  operationId: getPolRarity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analytics/pol/getTokenSummary\n  method: post\n  operationId: getPolTokenSummary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analytics/pol/getWashTrade\n\
  \  method: post\n  operationId: getPolWashTrade\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analytics/pol/getWashTransactions\n  method: post\n  operationId: getPolWashTransactions\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analytics/sol/getCollectionPriceDiff\n  method: post\n  operationId: getSolCollectionPriceDiff\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analytics/sol/getCollectionSalesOHLC\n  method: post\n  operationId: getSolCollectionSalesOHLC\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analytics/sol/getCollectionSummary\n  method: post\n  operationId: getSolCollectionSummary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analytics/sol/getRarity\n  method: post\n\
  \  operationId: getSolRarity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analytics/sol/getTokenSummary\n  method: post\n  operationId: getSolTokenSummary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analytics/sol/getWashTrade\n  method: post\n  operationId: getSolWashTrade\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analytics/sol/getWashTransactions\n  method: post\n  operationId: getSolWashTransactions\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /insights/eth/getTokenAppraisal\n  method: post\n  operationId: getEthTokenAppraisal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /insights/eth/getWalletLabels\n  method: post\n  operationId: getEthWalletLabels\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /insights/eth/getWalletValuation\n  method: post\n  operationId: getEthWalletValuation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /insights/pol/getTokenAppraisal\n  method: post\n  operationId: getPolTokenAppraisal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /insights/pol/getWalletLabels\n  method: post\n  operationId: getPolWalletLabels\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /insights/sol/getTokenAppraisal\n  method: post\n  operationId: getSolTokenAppraisal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gallop/refs/heads/main/agentic-access/gallop-agentic-access.yml
summary_line: 32 operations · 32 acting
tags:
- Company
- Developer Tools
- NFT
- Blockchain
- Web3
- Data
- Analytics
- Crypto
- Ethereum
- Solana
---
