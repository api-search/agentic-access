---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 12
api_specs:
- filename: ab5d-xyz-artist-tdh-api-openapi.yml
  format: yaml
  label: AB5D Artist Tdh API
  slug: ab5d-xyz-artist-tdh-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ab5d-xyz/openapi/ab5d-xyz-artist-tdh-api-openapi.yml
- filename: ab5d-xyz-artists-api-openapi.yml
  format: yaml
  label: AB5D Artists API
  slug: ab5d-xyz-artists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ab5d-xyz/openapi/ab5d-xyz-artists-api-openapi.yml
- filename: ab5d-xyz-bounties-api-openapi.yml
  format: yaml
  label: AB5D Bounties API
  slug: ab5d-xyz-bounties-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ab5d-xyz/openapi/ab5d-xyz-bounties-api-openapi.yml
- filename: ab5d-xyz-eligibility-api-openapi.yml
  format: yaml
  label: AB5D Eligibility API
  slug: ab5d-xyz-eligibility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ab5d-xyz/openapi/ab5d-xyz-eligibility-api-openapi.yml
- filename: ab5d-xyz-holdings-api-openapi.yml
  format: yaml
  label: AB5D Holdings API
  slug: ab5d-xyz-holdings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ab5d-xyz/openapi/ab5d-xyz-holdings-api-openapi.yml
- filename: ab5d-xyz-otdh-api-openapi.yml
  format: yaml
  label: AB5D Otdh API
  slug: ab5d-xyz-otdh-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ab5d-xyz/openapi/ab5d-xyz-otdh-api-openapi.yml
- filename: ab5d-xyz-receipts-json-api-openapi.yml
  format: yaml
  label: AB5D Receipts.json API
  slug: ab5d-xyz-receipts-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ab5d-xyz/openapi/ab5d-xyz-receipts-json-api-openapi.yml
- filename: ab5d-xyz-reputation-api-openapi.yml
  format: yaml
  label: AB5D Reputation API
  slug: ab5d-xyz-reputation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ab5d-xyz/openapi/ab5d-xyz-reputation-api-openapi.yml
consequence_counts:
  read: 12
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ab5D Xyz Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'AB5D exposes 16 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AB5D
provider_slug: ab5d-xyz
slug: ab5d-xyz-agentic-access
source_filename: ab5d-xyz-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/ab5d-xyz-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 12\n    acting: 4\n  by_consequence:\n    read: 12\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/artists\n  method: get\n  operationId: listArtistDossiers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/artists/{slug}\n  method: get\n  operationId: getArtistDossier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/otdh\n\
  \  method: get\n  operationId: listArtistOtdh\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/otdh/{slug}\n  method: get\n  operationId: getArtistOtdh\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/artist-tdh\n  method: get\n  operationId: listArtistCollectorTdhRegisters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/artist-tdh/{slug}\n  method: get\n  operationId: getArtistCollectorTdhRegister\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/holdings\n  method: get\n  operationId: listTreasuryHoldings\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/bounties\n  method: get\n  operationId: listBounties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/bounties/{taskId}/challenge\n  method: post\n  operationId: createBountyChallenge\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/bounties/{taskId}/claim\n  method: get\n  operationId: getBountyClaimStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/bounties/{taskId}/claim\n  method: post\n  operationId:\
  \ createBountyClaim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/bounties/{taskId}/release\n  method: post\n  operationId: releaseBountyClaim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/bounties/{taskId}/submission\n  method: post\n  operationId: submitBountyEvidence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/v1/receipts.json\n  method: get\n  operationId: listContributionReceipts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/eligibility/verify\n  method: get\n  operationId: verifyAgentEligibility\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/reputation/verify\n  method: get\n  operationId: getAgentReputation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/ab5d-xyz/agentic-access/ab5d-xyz-agentic-access.yml
summary_line: 16 operations · 4 acting
tags:
- Company
- Art
- Blockchain
- Generative Art
- Archives
- NFT
---
