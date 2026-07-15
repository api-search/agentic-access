---
acting_count: 75
action_class_counts:
  acting: 75
  connected: 208
api_specs:
- filename: akash-console-deployment-api.json
  format: json
  label: Akash Console Deployment API
  slug: akash-console-deployment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akash/refs/heads/main/openapi/akash-console-deployment-api.json
- filename: akash-blockchain-rest-api.yaml
  format: yaml
  label: Akash Blockchain REST API
  slug: akash-blockchain-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akash/refs/heads/main/openapi/akash-blockchain-rest-api.yaml
consequence_counts:
  physical: 31
  read: 208
  write: 44
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Akash Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /bank/accounts/{address}/transfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /distribution/delegators/{delegatorAddr}/rewards
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /distribution/delegators/{delegatorAddr}/rewards/{validatorAddr}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /distribution/delegators/{delegatorAddr}/withdraw_address
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /distribution/validators/{validatorAddr}/rewards
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /gov/proposals/{proposalId}/deposits
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /txs/decode
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /txs/encode
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/auth/signup
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/bid-screening
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/deployment-alerts/{dseq}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/deployment-alerts/{dseq}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/deployment-settings
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/deployment-settings/{userId}/{dseq}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/deployments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/deployments/{dseq}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/deployments/{dseq}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/deposit-deployment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/leases
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/pricing
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/send-verification-code
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/send-verification-email
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/stripe/coupons/apply
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/stripe/customers/organization
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/stripe/payment-methods/default
operation_count: 283
overview: 'Akash Network exposes 283 API operations that an AI agent could call, of which 75 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 208 read, 44 write, and 31 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Akash Network
provider_slug: akash
slug: akash-agentic-access
source_filename: akash-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/akash-blockchain-rest-api.yaml, openapi/akash-console-deployment-api.json, openapi/akash-notifications-api.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 283\n  by_action_class:\n    connected: 208\n    acting: 75\n  by_consequence:\n    read: 208\n    write: 44\n    physical: 31\n  human_in_the_loop_required: 0\noperations:\n- path: /akash/audit/v1beta3/audit/attributes/list\n  method: get\n  operationId: AllProvidersAttributes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /akash/audit/v1beta3/audit/attributes/{auditor}/{owner}\n  method: get\n  operationId: ProviderAuditorAttributes\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /akash/audit/v1beta3/audit/attributes/{owner}/list\n  method: get\n  operationId: ProviderAttributes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /akash/provider/v1beta3/auditor/{auditor}/list\n  method: get\n  operationId: AuditorAttributes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /akash/cert/v1beta3/certificates/list\n  method: get\n  operationId: Certificates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /akash/deployment/v1beta3/deployments/info\n  method: get\n  operationId: Deployment\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /akash/deployment/v1beta3/deployments/list\n  method: get\n  operationId: Deployments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /akash/deployment/v1beta3/groups/info\n  method: get\n  operationId: Group\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /akash/market/v1beta3/bids/info\n  method: get\n  operationId: Bid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /akash/market/v1beta3/bids/list\n  method: get\n  operationId: Bids\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /akash/market/v1beta3/leases/info\n  method: get\n  operationId: Lease\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /akash/market/v1beta3/leases/list\n  method: get\n  operationId: Leases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /akash/market/v1beta3/orders/info\n  method: get\n  operationId: Order\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /akash/market/v1beta3/orders/list\n  method: get\n  operationId: Orders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /akash/provider/v1beta3/providers\n  method: get\n\
  \  operationId: Providers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /akash/provider/v1beta3/providers/{owner}\n  method: get\n  operationId: Provider\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /node_info\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /syncing\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /blocks/latest\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /blocks/{height}\n  method: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /validatorsets/latest\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /validatorsets/{height}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /txs/{hash}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /txs\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /txs\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /txs/encode\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /txs/decode\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bank/balances/{address}\n  method: get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bank/accounts/{address}/transfers\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bank/total\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bank/total/{denomination}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/accounts/{address}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /staking/delegators/{delegatorAddr}/delegations\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /staking/delegators/{delegatorAddr}/delegations\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /staking/delegators/{delegatorAddr}/delegations/{validatorAddr}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /staking/delegators/{delegatorAddr}/unbonding_delegations\n  method: get\n  x-agentic-access:\n    action-class: connected\n   \
  \ consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /staking/delegators/{delegatorAddr}/unbonding_delegations\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /staking/delegators/{delegatorAddr}/unbonding_delegations/{validatorAddr}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /staking/redelegations\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /staking/delegators/{delegatorAddr}/redelegations\n  method: post\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /staking/delegators/{delegatorAddr}/validators\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /staking/delegators/{delegatorAddr}/validators/{validatorAddr}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /staking/validators\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /staking/validators/{validatorAddr}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /staking/validators/{validatorAddr}/delegations\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /staking/validators/{validatorAddr}/unbonding_delegations\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /staking/pool\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /staking/parameters\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /slashing/signing_infos\n  method: get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /slashing/validators/{validatorAddr}/unjail\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /slashing/parameters\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gov/proposals\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gov/proposals\n  method: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gov/proposals/param_change\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gov/proposals/{proposalId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gov/proposals/{proposalId}/proposer\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gov/proposals/{proposalId}/deposits\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gov/proposals/{proposalId}/deposits\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gov/proposals/{proposalId}/deposits/{depositor}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gov/proposals/{proposalId}/votes\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gov/proposals/{proposalId}/votes\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gov/proposals/{proposalId}/votes/{voter}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gov/proposals/{proposalId}/tally\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gov/parameters/deposit\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gov/parameters/tallying\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /gov/parameters/voting\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /distribution/delegators/{delegatorAddr}/rewards\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /distribution/delegators/{delegatorAddr}/rewards\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /distribution/delegators/{delegatorAddr}/rewards/{validatorAddr}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n \
  \   subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /distribution/delegators/{delegatorAddr}/rewards/{validatorAddr}\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /distribution/delegators/{delegatorAddr}/withdraw_address\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /distribution/delegators/{delegatorAddr}/withdraw_address\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /distribution/validators/{validatorAddr}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /distribution/validators/{validatorAddr}/outstanding_rewards\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /distribution/validators/{validatorAddr}/rewards\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /distribution/validators/{validatorAddr}/rewards\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /distribution/community_pool\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /distribution/parameters\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /minting/parameters\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /minting/inflation\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /minting/annual-provisions\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/auth/v1beta1/accounts\n  method: get\n  operationId: Accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/auth/v1beta1/accounts/{address}\n  method: get\n  operationId: Account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/auth/v1beta1/params\n  method: get\n  operationId: AuthParams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/bank/v1beta1/balances/{address}\n  method: get\n  operationId: AllBalances\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/bank/v1beta1/balances/{address}/{denom}\n  method: get\n  operationId: Balance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/bank/v1beta1/denom_owners/{denom}\n  method: get\n  operationId: DenomOwners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/bank/v1beta1/denoms_metadata\n  method: get\n  operationId: DenomsMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/bank/v1beta1/denoms_metadata/{denom}\n  method: get\n  operationId: DenomMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/bank/v1beta1/params\n  method: get\n  operationId: BankParams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/bank/v1beta1/supply\n  method: get\n  operationId: TotalSupply\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/bank/v1beta1/supply/{denom}\n  method: get\n  operationId: SupplyOf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/base/tendermint/v1beta1/blocks/latest\n  method: get\n  operationId: GetLatestBlock\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/base/tendermint/v1beta1/blocks/{height}\n\
  \  method: get\n  operationId: GetBlockByHeight\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/base/tendermint/v1beta1/node_info\n  method: get\n  operationId: GetNodeInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/base/tendermint/v1beta1/syncing\n  method: get\n  operationId: GetSyncing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/base/tendermint/v1beta1/validatorsets/latest\n  method: get\n  operationId: GetLatestValidatorSet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/base/tendermint/v1beta1/validatorsets/{height}\n  method:\
  \ get\n  operationId: GetValidatorSetByHeight\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/distribution/v1beta1/community_pool\n  method: get\n  operationId: CommunityPool\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/distribution/v1beta1/delegators/{delegator_address}/rewards\n  method: get\n  operationId: DelegationTotalRewards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/distribution/v1beta1/delegators/{delegator_address}/rewards/{validator_address}\n  method: get\n  operationId: DelegationRewards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /cosmos/distribution/v1beta1/delegators/{delegator_address}/validators\n  method: get\n  operationId: DelegatorValidators\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/distribution/v1beta1/delegators/{delegator_address}/withdraw_address\n  method: get\n  operationId: DelegatorWithdrawAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/distribution/v1beta1/params\n  method: get\n  operationId: DistributionParams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/distribution/v1beta1/validators/{validator_address}/commission\n  method: get\n  operationId: ValidatorCommission\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/distribution/v1beta1/validators/{validator_address}/outstanding_rewards\n  method: get\n  operationId: ValidatorOutstandingRewards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/distribution/v1beta1/validators/{validator_address}/slashes\n  method: get\n  operationId: ValidatorSlashes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/evidence/v1beta1/evidence\n  method: get\n  operationId: AllEvidence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/evidence/v1beta1/evidence/{evidence_hash}\n  method: get\n  operationId: Evidence\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/gov/v1beta1/params/{params_type}\n  method: get\n  operationId: GovParams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/gov/v1beta1/proposals\n  method: get\n  operationId: Proposals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/gov/v1beta1/proposals/{proposal_id}\n  method: get\n  operationId: Proposal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/gov/v1beta1/proposals/{proposal_id}/deposits\n  method: get\n  operationId: Deposits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/gov/v1beta1/proposals/{proposal_id}/deposits/{depositor}\n  method: get\n  operationId: Deposit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/gov/v1beta1/proposals/{proposal_id}/tally\n  method: get\n  operationId: TallyResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/gov/v1beta1/proposals/{proposal_id}/votes\n  method: get\n  operationId: Votes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/gov/v1beta1/proposals/{proposal_id}/votes/{voter}\n  method: get\n  operationId: Vote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/mint/v1beta1/annual_provisions\n  method: get\n  operationId: AnnualProvisions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/mint/v1beta1/inflation\n  method: get\n  operationId: Inflation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/mint/v1beta1/params\n  method: get\n  operationId: MintParams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/params/v1beta1/params\n  method: get\n  operationId: Params\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/slashing/v1beta1/params\n\
  \  method: get\n  operationId: SlashingParams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/slashing/v1beta1/signing_infos\n  method: get\n  operationId: SigningInfos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/slashing/v1beta1/signing_infos/{cons_address}\n  method: get\n  operationId: SigningInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/staking/v1beta1/delegations/{delegator_addr}\n  method: get\n  operationId: DelegatorDelegations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/staking/v1beta1/delegators/{delegator_addr}/redelegations\n\
  \  method: get\n  operationId: Redelegations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/staking/v1beta1/delegators/{delegator_addr}/unbonding_delegations\n  method: get\n  operationId: DelegatorUnbondingDelegations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/staking/v1beta1/delegators/{delegator_addr}/validators\n  method: get\n  operationId: StakingDelegatorValidators\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/staking/v1beta1/delegators/{delegator_addr}/validators/{validator_addr}\n  method: get\n  operationId: DelegatorValidator\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /cosmos/staking/v1beta1/historical_info/{height}\n  method: get\n  operationId: HistoricalInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/staking/v1beta1/params\n  method: get\n  operationId: StakingParams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/staking/v1beta1/pool\n  method: get\n  operationId: Pool\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/staking/v1beta1/validators\n  method: get\n  operationId: Validators\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/staking/v1beta1/validators/{validator_addr}\n\
  \  method: get\n  operationId: Validator\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/staking/v1beta1/validators/{validator_addr}/delegations\n  method: get\n  operationId: ValidatorDelegations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/staking/v1beta1/validators/{validator_addr}/delegations/{delegator_addr}\n  method: get\n  operationId: Delegation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/staking/v1beta1/validators/{validator_addr}/delegations/{delegator_addr}/unbonding_delegation\n  method: get\n  operationId: UnbondingDelegation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optiona\n\n# ---\
  \ truncated at 32 KB (68 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/akash/refs/heads/main/agentic-access/akash-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akash/refs/heads/main/agentic-access/akash-agentic-access.yml
summary_line: 283 operations · 75 acting
tags:
- Cloud Computing
- Decentralized
- Blockchain
- Kubernetes
- GPU
- AI Inference
- Cosmos
- Web3
---
