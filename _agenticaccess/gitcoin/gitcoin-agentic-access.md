---
acting_count: 0
action_class_counts:
  connected: 13
api_specs:
- filename: gitcoin-core-api-openapi.json
  format: json
  label: Gitcoin Core API
  slug: gitcoin-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitcoin/refs/heads/main/openapi/gitcoin-core-api-openapi.json
- filename: gitcoin-grants-api-openapi.json
  format: json
  label: Gitcoin Grants API
  slug: gitcoin-grants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitcoin/refs/heads/main/openapi/gitcoin-grants-api-openapi.json
- filename: gitcoin-passport-stamps-api-openapi.json
  format: json
  label: Gitcoin Passport Stamps API
  slug: gitcoin-passport-stamps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitcoin/refs/heads/main/openapi/gitcoin-passport-stamps-api-openapi.json
consequence_counts:
  read: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Gitcoin Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'Gitcoin exposes 13 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Gitcoin
provider_slug: gitcoin
slug: gitcoin-agentic-access
source_filename: gitcoin-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/gitcoin-core-api-openapi.json, openapi/gitcoin-grants-api-openapi.json, openapi/gitcoin-passport-stamps-api-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 13\n  by_consequence:\n    read: 13\n  human_in_the_loop_required: 0\noperations:\n- path: /bounties/\n  method: get\n  operationId: listBounties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /grants/\n  method: get\n  operationId: listGrants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /grants/grants.json\n  method: get\n  operationId: getAllGrants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /grants/v1/api/export_addresses/all.json\n  method: get\n  operationId: getAllContributorAddresses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /grants/v1/api/export_addresses/{roundId}.json\n  method: get\n  operationId: getContributorsByRound\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /grants/v1/api/export_addresses/{grantId}.json\n  method: get\n  operationId: getContributorsByGrant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /grants/v1/api/export_addresses/{grantRoundId}.json\n  method: get\n  operationId: getContributorsByGrantAndRound\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /grants/v1/api/export_info/{grantRoundId}.json\n  method: get\n  operationId: getContributorInfoByGrantAndRound\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/models/score/{address}\n  method: get\n  operationId: v2_api_api_models_get_analysis\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/stamps/{scorer_id}/score/{address}\n  method: get\n  operationId: v2_api_api_stamps_a_submit_passport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v2/stamps/{scorer_id}/score/{address}/history\n  method: get\n  operationId: v2_api_api_stamps_get_score_history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/stamps/metadata\n  method: get\n  operationId: v2_api_api_stamps_stamp_display\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/stamps/{address}\n  method: get\n  operationId: v2_api_api_stamps_get_passport_stamps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gitcoin/refs/heads/main/agentic-access/gitcoin-agentic-access.yml
summary_line: 13 operations
tags:
- Public Goods
- Grants
- Bounties
- Quadratic Funding
- Web3
- Verifiable Credentials
- Identity
- Open Source
---
