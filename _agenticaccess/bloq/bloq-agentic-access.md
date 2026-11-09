---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 13
api_specs:
- filename: bloq-auth-api-openapi.yml
  format: yaml
  label: Bloq Auth API
  slug: bloq-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bloq/openapi/bloq-auth-api-openapi.yml
- filename: bloq-bloq-api-api-openapi.yml
  format: yaml
  label: Bloq Bloq API
  slug: bloq-bloq-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bloq/openapi/bloq-bloq-api-api-openapi.yml
- filename: bloq-chains-api-openapi.yml
  format: yaml
  label: Bloq Chains API
  slug: bloq-chains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bloq/openapi/bloq-chains-api-openapi.yml
- filename: bloq-logs-api-openapi.yml
  format: yaml
  label: Bloq Logs API
  slug: bloq-logs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bloq/openapi/bloq-logs-api-openapi.yml
- filename: bloq-staking-api-openapi.yml
  format: yaml
  label: Bloq Staking API
  slug: bloq-staking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bloq/openapi/bloq-staking-api-openapi.yml
- filename: bloq-status-api-openapi.yml
  format: yaml
  label: Bloq Status API
  slug: bloq-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bloq/openapi/bloq-status-api-openapi.yml
- filename: bloq-users-api-openapi.yml
  format: yaml
  label: Bloq Users API
  slug: bloq-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bloq/openapi/bloq-users-api-openapi.yml
consequence_counts:
  physical: 1
  read: 13
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bloq Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /staking/ethereum/{chain}/validators/{pubkey}/validatorExit
operation_count: 25
overview: 'Bloq exposes 25 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read, 11 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bloq
provider_slug: bloq
slug: bloq-agentic-access
source_filename: bloq-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/bloq-auth-api-openapi.yml, openapi/bloq-bloq-api-api-openapi.yml, openapi/bloq-chains-api-openapi.yml,\n  openapi/bloq-logs-api-openapi.yml, openapi/bloq-staking-api-openapi.yml, openapi/bloq-status-api-openapi.yml,\n  openapi/bloq-users-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    acting: 12\n    connected: 13\n  by_consequence:\n    write: 11\n    read: 13\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /auth\n  method: post\n  operationId: post_auth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/token\n  method: post\n  operationId: post_auth_token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/users/{publicaddress}\n  method: post\n  operationId: post_auth_users_publicaddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /\n  method: get\n  operationId: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /\n  method: post\n  operationId: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chains\n  method: get\n  operationId: get_chains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /logs\n  method: get\n  operationId: get_logs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /staking/ethereum/{chain}/validators\n  method: post\n  operationId: post_staking_ethereum_chain_validators\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /staking/ethereum/{chain}/validators/{pubkey}\n  method: delete\n  operationId: delete_staking_ethereum_chain_validators_pubkey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /staking/ethereum/{chain}/validators/{pubkey}\n  method: get\n  operationId: get_staking_ethereum_chain_validators_pubkey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /staking/ethereum/{chain}/validators/{pubkey}\n  method: put\n  operationId: put_staking_ethereum_chain_validators_pubkey\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /staking/ethereum/{chain}/validators/{pubkey}/performance\n  method: get\n  operationId: get_staking_ethereum_chain_validators_pubkey_performance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /staking/ethereum/{chain}/validators/{pubkey}/validatorExit\n  method: post\n  operationId: post_staking_ethereum_chain_validators_pubkey_validatorExit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /staking/ethereum/{chain}/{id}\n  method: get\n  operationId: get_staking_ethereum_chain_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /staking/ethereum/{ethereumid}\n  method: get\n  operationId: get_staking_ethereum_ethereumid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /staking/ethereum/{ethereumid}/report\n  method: get\n  operationId: get_staking_ethereum_ethereumid_report\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status\n  method: get\n  operationId: get_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /users/me\n  method: get\n  operationId: get_users_me\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/me/nodes/{id}\n  method: get\n  operationId: get_users_me_nodes_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/me/password\n  method: put\n  operationId: put_users_me_password\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/me/{meid}\n  method: get\n  operationId: get_users_me_meid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /users/me/{meid}\n  method: post\n  operationId: post_users_me_meid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/me/{meid}/{id}\n  method: delete\n  operationId: delete_users_me_meid_id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{publicaddress}/nonce\n  method: post\n  operationId: post_users_publicaddress_nonce\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{userid}/token/{token}\n\
  \  method: put\n  operationId: put_users_userid_token_token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/bloq/agentic-access/bloq-agentic-access.yml
summary_line: 25 operations · 12 acting
tags:
- Company
- Web3
- Infrastructure
- DeFi
- Blockchain
---
