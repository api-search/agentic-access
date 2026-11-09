---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 17
api_specs:
- filename: chainflip-broker-io-assets-api-openapi.yml
  format: yaml
  label: Chainflip Broker as a Service Assets API
  slug: chainflip-broker-io-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chainflip-broker-io/openapi/chainflip-broker-io-assets-api-openapi.yml
- filename: chainflip-broker-io-fees-api-openapi.yml
  format: yaml
  label: Chainflip Broker as a Service Fees API
  slug: chainflip-broker-io-fees-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chainflip-broker-io/openapi/chainflip-broker-io-fees-api-openapi.yml
- filename: chainflip-broker-io-networks-api-openapi.yml
  format: yaml
  label: Chainflip Broker as a Service Networks API
  slug: chainflip-broker-io-networks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chainflip-broker-io/openapi/chainflip-broker-io-networks-api-openapi.yml
- filename: chainflip-broker-io-onboarding-api-openapi.yml
  format: yaml
  label: Chainflip Broker as a Service Onboarding API
  slug: chainflip-broker-io-onboarding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chainflip-broker-io/openapi/chainflip-broker-io-onboarding-api-openapi.yml
- filename: chainflip-broker-io-quote-api-openapi.yml
  format: yaml
  label: Chainflip Broker as a Service Quote API
  slug: chainflip-broker-io-quote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chainflip-broker-io/openapi/chainflip-broker-io-quote-api-openapi.yml
- filename: chainflip-broker-io-rpc-api-openapi.yml
  format: yaml
  label: Chainflip Broker as a Service Rpc API
  slug: chainflip-broker-io-rpc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chainflip-broker-io/openapi/chainflip-broker-io-rpc-api-openapi.yml
- filename: chainflip-broker-io-status-api-openapi.yml
  format: yaml
  label: Chainflip Broker as a Service Status API
  slug: chainflip-broker-io-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chainflip-broker-io/openapi/chainflip-broker-io-status-api-openapi.yml
- filename: chainflip-broker-io-swap-api-openapi.yml
  format: yaml
  label: Chainflip Broker as a Service Swap API
  slug: chainflip-broker-io-swap-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chainflip-broker-io/openapi/chainflip-broker-io-swap-api-openapi.yml
- filename: chainflip-broker-io-swaps-api-openapi.yml
  format: yaml
  label: Chainflip Broker as a Service Swaps API
  slug: chainflip-broker-io-swaps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chainflip-broker-io/openapi/chainflip-broker-io-swaps-api-openapi.yml
consequence_counts:
  read: 17
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Chainflip Broker Io Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 19
overview: 'Chainflip Broker as a Service exposes 19 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Chainflip Broker as a Service
provider_slug: chainflip-broker-io
slug: chainflip-broker-io-agentic-access
source_filename: chainflip-broker-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/chainflip-broker-io-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 17\n    acting: 2\n  by_consequence:\n    read: 17\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /assets\n  method: get\n  operationId: listAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/{network}\n  method: get\n  operationId: listNetworkAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/{asset}/logo.svg\n\
  \  method: get\n  operationId: getAssetLogo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fees\n  method: get\n  operationId: getEarnedFees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /networks\n  method: get\n  operationId: listNetworks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /networks/{network}/logo.svg\n  method: get\n  operationId: getNetworkLogo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /quote-native\n  method: get\n  operationId: getNativeQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /quotes-native\n  method: get\n  operationId: getNativeQuotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /quote\n  method: get\n  operationId: getQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /quotes\n  method: get\n  operationId: getQuotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rpc/{apiKey}\n  method: post\n  operationId: brokerRpc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /status-by-deposit-channel\n  method: get\n  operationId: getStatusByDepositChannel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status-by-id\n  method: get\n  operationId: getStatusById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status-by-transaction-hash\n  method: get\n  operationId: getStatusByTransactionHash\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /swap\n  method: get\n  operationId: startSwap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /swap\n  method: post\n  operationId: startAdvancedSwap\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feed\n  method: get\n  operationId: getSwapFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /swaps\n  method: get\n  operationId: listSwaps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /onboarding\n  method: get\n  operationId: getOnboarding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/chainflip-broker-io/agentic-access/chainflip-broker-io-agentic-access.yml
summary_line: 19 operations · 2 acting
tags:
- Finance
- DeFi
- Cryptocurrency
- Brokerage
- Infrastructure
- Company
---
