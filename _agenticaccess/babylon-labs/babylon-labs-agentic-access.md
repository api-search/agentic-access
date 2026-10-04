---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 18
api_specs:
- filename: babylon-labs-shared-api-openapi.yml
  format: yaml
  label: Babylon Labs Shared API
  slug: babylon-labs-shared-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/babylon-labs/refs/heads/main/openapi/babylon-labs-shared-api-openapi.yml
- filename: babylon-labs-apr-api-openapi.yml
  format: yaml
  label: Babylon Labs Apr API
  slug: babylon-labs-apr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/babylon-labs/refs/heads/main/openapi/babylon-labs-apr-api-openapi.yml
- filename: babylon-labs-delegation-api-openapi.yml
  format: yaml
  label: Babylon Labs Delegation API
  slug: babylon-labs-delegation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/babylon-labs/refs/heads/main/openapi/babylon-labs-delegation-api-openapi.yml
- filename: babylon-labs-delegations-api-openapi.yml
  format: yaml
  label: Babylon Labs Delegations API
  slug: babylon-labs-delegations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/babylon-labs/refs/heads/main/openapi/babylon-labs-delegations-api-openapi.yml
- filename: babylon-labs-finality-providers-api-openapi.yml
  format: yaml
  label: Babylon Labs Finality Providers API
  slug: babylon-labs-finality-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/babylon-labs/refs/heads/main/openapi/babylon-labs-finality-providers-api-openapi.yml
- filename: babylon-labs-global-params-api-openapi.yml
  format: yaml
  label: Babylon Labs Global Params API
  slug: babylon-labs-global-params-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/babylon-labs/refs/heads/main/openapi/babylon-labs-global-params-api-openapi.yml
- filename: babylon-labs-network-info-api-openapi.yml
  format: yaml
  label: Babylon Labs Network Info API
  slug: babylon-labs-network-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/babylon-labs/refs/heads/main/openapi/babylon-labs-network-info-api-openapi.yml
- filename: babylon-labs-prices-api-openapi.yml
  format: yaml
  label: Babylon Labs Prices API
  slug: babylon-labs-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/babylon-labs/refs/heads/main/openapi/babylon-labs-prices-api-openapi.yml
- filename: babylon-labs-staker-api-openapi.yml
  format: yaml
  label: Babylon Labs Staker API
  slug: babylon-labs-staker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/babylon-labs/refs/heads/main/openapi/babylon-labs-staker-api-openapi.yml
- filename: babylon-labs-stats-api-openapi.yml
  format: yaml
  label: Babylon Labs Stats API
  slug: babylon-labs-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/babylon-labs/refs/heads/main/openapi/babylon-labs-stats-api-openapi.yml
- filename: babylon-labs-unbonding-api-openapi.yml
  format: yaml
  label: Babylon Labs Unbonding API
  slug: babylon-labs-unbonding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/babylon-labs/refs/heads/main/openapi/babylon-labs-unbonding-api-openapi.yml
consequence_counts:
  read: 18
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Babylon Labs Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 19
overview: 'Babylon Labs exposes 19 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Babylon Labs
provider_slug: babylon-labs
slug: babylon-labs-agentic-access
source_filename: babylon-labs-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/babylon-labs-staking-api-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 18\n    acting: 1\n  by_consequence:\n    read: 18\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /healthcheck\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/delegation\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/finality-providers\n  method: get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/global-params\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/staker/delegation/check\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/staker/delegations\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/staker/pubkey-lookup\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stats\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stats/staker\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/unbonding\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/unbonding/eligibility\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/apr\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/delegation\n  method: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/delegations\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/finality-providers\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/network-info\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/prices\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/staker/stats\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/stats\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/babylon-labs/refs/heads/main/agentic-access/babylon-labs-agentic-access.yml
summary_line: 19 operations · 1 acting
tags:
- Company
- Crypto Defi
- Bitcoin
- Bitcoin Staking
- Blockchain
- Cosmos
- Proof of Stake
- DeFi
- Staking
---
