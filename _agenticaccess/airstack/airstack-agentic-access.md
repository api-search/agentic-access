---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 22
api_specs:
- filename: farcaster-hub-rest-api.json
  format: json
  label: Airstack Farcaster Hub API
  slug: airstack-farcaster-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airstack/refs/heads/main/openapi/farcaster-hub-rest-api.json
- filename: farcaster-webhooks-api.json
  format: json
  label: Airstack Farcaster Webhooks API
  slug: airstack-farcaster-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airstack/refs/heads/main/openapi/farcaster-webhooks-api.json
consequence_counts:
  read: 22
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Airstack Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 27
overview: 'Airstack exposes 27 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Airstack
provider_slug: airstack
slug: airstack-agentic-access
source_filename: airstack-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/farcaster-hub-rest-api.json, openapi/farcaster-webhooks-api.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 27\n  by_action_class:\n    connected: 22\n    acting: 5\n  by_consequence:\n    read: 22\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/castById\n  method: get\n  operationId: GetCastById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/castsByFid\n  method: get\n  operationId: ListCastsByFid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/castsByMention\n  method: get\n  operationId: ListCastsByMention\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/castsByParent\n  method: get\n  operationId: ListCastsByParent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reactionById\n  method: get\n  operationId: GetReactionById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reactionsByCast\n  method: get\n  operationId: ListReactionsByCast\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reactionsByFid\n  method: get\n  operationId: ListReactionsByFid\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reactionsByTarget\n  method: get\n  operationId: ListReactionsByTarget\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/linkById\n  method: get\n  operationId: GetLinkById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/linksByFid\n  method: get\n  operationId: ListLinksByFid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/linksByTargetFid\n  method: get\n  operationId: ListLinksByTargetFid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/userDataByFid\n  method: get\n  operationId: GetUserDataByFid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fids\n  method: get\n  operationId: ListFids\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/storageLimitsByFid\n  method: get\n  operationId: GetStorageLimitsByFid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/userNameProofsByFid\n  method: get\n  operationId: ListUsernameProofsByFid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/userNameProofByName\n  method: get\n  operationId: GetUsernameProof\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/verificationsByFid\n  method: get\n  operationId: ListVerificationsByFid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/onChainIdRegistryEventByAddress\n  method: get\n  operationId: GetOnChainIdRegistrationByAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/onChainEventsByFid\n  method: get\n  operationId: ListOnChainEventsByFid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/onChainSignersByFid\n  method: get\n  operationId: ListOnChainSignersByFid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/submitMessage\n  method: post\n  operationId: SubmitMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/validateMessage\n  method: post\n  operationId: ValidateMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/events\n  method: get\n  operationId: ListEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/eventById\n  method:\
  \ get\n  operationId: GetEventById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/webhooks\n  method: post\n  operationId: subscriptionsCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/filters/test\n  method: post\n  operationId: subscriptionsTestFilter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/webhooks/{webhook_id}\n  method: delete\n  operationId: subscriptionsDelete\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airstack/refs/heads/main/agentic-access/airstack-agentic-access.yml
summary_line: 27 operations · 5 acting
tags:
- Web3
- Blockchain
- GraphQL
- NFT
- Tokens
- On-Chain Data
- Ethereum
- Polygon
- Base
- ENS
- POAP
- Social Graph
- Wallet
- Identity
---
