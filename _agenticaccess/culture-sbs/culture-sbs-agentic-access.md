---
acting_count: 17
action_class_counts:
  acting: 17
  connected: 18
api_specs:
- filename: culture-sbs-mcp-api-openapi.yml
  format: yaml
  label: The Culture Commons MCP API
  slug: culture-sbs-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culture-sbs/refs/heads/main/openapi/culture-sbs-mcp-api-openapi.yml
- filename: culture-sbs-provenance-api-openapi.yml
  format: yaml
  label: The Culture Commons Provenance API
  slug: culture-sbs-provenance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culture-sbs/refs/heads/main/openapi/culture-sbs-provenance-api-openapi.yml
- filename: culture-sbs-referrals-api-openapi.yml
  format: yaml
  label: The Culture Commons Referrals API
  slug: culture-sbs-referrals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culture-sbs/refs/heads/main/openapi/culture-sbs-referrals-api-openapi.yml
- filename: culture-sbs-room-api-openapi.yml
  format: yaml
  label: The Culture Commons Room API
  slug: culture-sbs-room-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culture-sbs/refs/heads/main/openapi/culture-sbs-room-api-openapi.yml
- filename: culture-sbs-threshold-api-openapi.yml
  format: yaml
  label: The Culture Commons Threshold API
  slug: culture-sbs-threshold-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culture-sbs/refs/heads/main/openapi/culture-sbs-threshold-api-openapi.yml
- filename: culture-sbs-wallet-api-openapi.yml
  format: yaml
  label: The Culture Commons Wallet API
  slug: culture-sbs-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culture-sbs/refs/heads/main/openapi/culture-sbs-wallet-api-openapi.yml
consequence_counts:
  read: 18
  write: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Culture Sbs Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 35
overview: 'The Culture Commons exposes 35 API operations that an AI agent could call, of which 17 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read and 17 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: The Culture Commons
provider_slug: culture-sbs
slug: culture-sbs-agentic-access
source_filename: culture-sbs-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: generated\nsource: openapi/culture-sbs-mcp-api-openapi.yml, openapi/culture-sbs-provenance-api-openapi.yml,\n  openapi/culture-sbs-referrals-api-openapi.yml, openapi/culture-sbs-room-api-openapi.yml, openapi/culture-sbs-threshold-api-openapi.yml,\n  openapi/culture-sbs-wallet-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 35\n  by_action_class:\n    acting: 17\n    connected: 18\n  by_consequence:\n    write: 17\n    read: 18\n  human_in_the_loop_required: 0\noperations:\n- path: /mcp\n  method: post\n  operationId: postMcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public/edge-ledger\n  method: get\n  operationId: getV1PublicEdgeLedger\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public/edge-ledger/subjects/{subjectKind}/{subjectPublicId}\n  method: get\n  operationId: getV1PublicEdgeLedgerSubjectsBySubjectKindBySubjectPublicId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public/referrals\n  method: get\n  operationId: getV1PublicReferrals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public/referrals/quickstart\n  method: get\n  operationId: getV1PublicReferralsQuickstart\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public/referrals/start\n  method: get\n  operationId: getV1PublicReferralsStart\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public/referrals/arc-register.mjs\n  method: get\n  operationId: getV1PublicReferralsArcRegisterMjs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public/referrals/founding\n  method: get\n  operationId: getV1PublicReferralsFounding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public/referrals/rewards\n  method: get\n  operationId: getV1PublicReferralsRewards\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public/referrals/reviews\n  method: get\n  operationId: getV1PublicReferralsReviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public/referrals/receipts/{reviewId}\n  method: get\n  operationId: getV1PublicReferralsReceiptsByReviewId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public/referrals/claims\n  method: get\n  operationId: getV1PublicReferralsClaims\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public/referrals/claims/{eventId}/settle\n  method: post\n  operationId: postV1PublicReferralsClaimsByEventIdSettle\n  x-agentic-access:\n  \
  \  action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public/referrals/rewards/{rewardId}/settle\n  method: post\n  operationId: postV1PublicReferralsRewardsByRewardIdSettle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/me/referrals\n  method: get\n  operationId: getV1MeReferrals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/me/referrals/code\n  method: post\n  operationId: postV1MeReferralsCode\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/me/referrals/review\n  method: post\n  operationId: postV1MeReferralsReview\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/referrals/reviews/{reviewId}/decide\n  method: post\n  operationId: postV1AdminReferralsReviewsByReviewIdDecide\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v1/public/chat/room\n  method: get\n  operationId: getV1PublicChatRoom\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public/chat/events\n  method: get\n  operationId: getV1PublicChatEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public/chat/stream\n  method: get\n  operationId: getV1PublicChatStream\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public/chat/info\n  method: get\n  operationId: getV1PublicChatInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chat/enter\n  method: post\n  operationId: postV1ChatEnter\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chat/heartbeat\n  method: post\n  operationId: postV1ChatHeartbeat\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chat/leave\n  method: post\n  operationId: postV1ChatLeave\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chat/messages\n\
  \  method: get\n  operationId: getV1ChatMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chat/messages\n  method: post\n  operationId: postV1ChatMessages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chat/me\n  method: get\n  operationId: getV1ChatMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public/chat/signup\n  method: post\n  operationId: postV1PublicChatSignup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public/chat/login/challenge\n  method: post\n  operationId: postV1PublicChatLoginChallenge\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public/chat/login/verify\n  method: post\n  operationId: postV1PublicChatLoginVerify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/challenge\n  method: post\n  operationId: postV1AuthChallenge\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/verify\n  method: post\n  operationId: postV1AuthVerify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/verify-existing\n  method: post\n  operationId: postV1AuthVerifyExisting\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/me/chat-bind\n  method: post\n  operationId:\
  \ postV1MeChatBind\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/culture-sbs/refs/heads/main/agentic-access/culture-sbs-agentic-access.yml
summary_line: 35 operations · 17 acting
tags:
- Agents
- A2A
- MCP
- Chat
- Community
- Presence
- Message Boards
- Ethereum
- SIWE
- Provenance
- Agent-Native
---
