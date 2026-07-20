---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 13
api_specs:
- filename: coinlist-passage-openapi-original.json
  format: json
  label: CoinList Passage (Frontline API)
  slug: coinlist-passage-frontline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinlist/refs/heads/main/openapi/coinlist-passage-openapi-original.json
consequence_counts:
  physical: 1
  read: 13
  safety-critical: 3
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Coinlist Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /oauth/introspect
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /oauth/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /oauth/token
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/wallet-ownership
operation_count: 22
overview: 'CoinList exposes 22 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read, 5 write, 1 physical, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CoinList
provider_slug: coinlist
slug: coinlist-agentic-access
source_filename: coinlist-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/coinlist-passage-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    acting: 9\n    connected: 13\n  by_consequence:\n    safety-critical: 3\n    write: 5\n    read: 13\n    physical: 1\n  human_in_the_loop_required: 3\noperations:\n- path: /oauth/introspect\n  method: post\n  operationId: FrontlineAPIWeb.Oauth.IntrospectController.OpenApiSpec.introspect\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n\
  \    audit: required\n- path: /oauth/revoke\n  method: post\n  operationId: FrontlineAPIWeb.Oauth.RevokeController.OpenApiSpec.revoke\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /oauth/token\n  method: post\n  operationId: FrontlineAPIWeb.Oauth.TokenController.OpenApiSpec.token\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/documents/{document_type}/submission\n  method: post\n  operationId: createDocumentSubmission\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/kyc-token\n  method: post\n  operationId: createKycToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/offers\n  method: get\n  operationId: listPartnerOffers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/offers/{id}\n  method: get\n  operationId: getPartnerOffer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/offers/{offer_id}/allow-wallet\n  method: post\n  operationId: allowWallet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/offers/{offer_id}/requirements\n  method: get\n  operationId: listOfferRequirements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/offers/{offer_id}/requirements/statuses\n  method: get\n  operationId: listOfferRequirementStatuses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/offers/{offer_id}/submit-addresses\n  method: post\n  operationId: createOfferOptionAddress\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/participations\n  method: get\n  operationId: listPartnerParticipations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/participations\n  method: post\n  operationId: createPartnerParticipation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/participations/{id}\n  method: get\n  operationId: getPartnerParticipation\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/pii\n  method: get\n  operationId: getPii\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/swap/output-token\n  method: get\n  operationId: getSwapOutputToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/swap/preview\n  method: get\n  operationId: getSwapPreview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/swap/status\n  method: get\n  operationId: getSwapStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/token/allowance\n\
  \  method: get\n  operationId: getTokenAllowance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/token/balance\n  method: get\n  operationId: getTokenBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/wallet-ownership\n  method: post\n  operationId: createWalletOwnershipChallenge\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/wallet/authorized\n  method: get\n  operationId: getWalletAuthorized\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n   \
  \ subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coinlist/refs/heads/main/agentic-access/coinlist-agentic-access.yml
summary_line: 22 operations · 9 acting · 3 human-in-the-loop
tags:
- Company
- Fintech
- Cryptocurrency
- Token Sales
- Tokenized Equities
- KYC
- OAuth
- Blockchain
- Digital Assets
- Embedded Finance
---
