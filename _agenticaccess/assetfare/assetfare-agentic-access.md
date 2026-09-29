---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 11
api_specs:
- filename: assetfare-auth-api-openapi.yml
  format: yaml
  label: AssetFare Auth API
  slug: assetfare-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assetfare/refs/heads/main/openapi/assetfare-auth-api-openapi.yml
- filename: assetfare-quote-api-openapi.yml
  format: yaml
  label: AssetFare Quote API
  slug: assetfare-quote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assetfare/refs/heads/main/openapi/assetfare-quote-api-openapi.yml
- filename: assetfare-session-api-openapi.yml
  format: yaml
  label: AssetFare Session API
  slug: assetfare-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assetfare/refs/heads/main/openapi/assetfare-session-api-openapi.yml
- filename: assetfare-status-api-openapi.yml
  format: yaml
  label: AssetFare Status API
  slug: assetfare-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assetfare/refs/heads/main/openapi/assetfare-status-api-openapi.yml
- filename: assetfare-well-known-api-openapi.yml
  format: yaml
  label: AssetFare .well Known API
  slug: assetfare-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assetfare/refs/heads/main/openapi/assetfare-well-known-api-openapi.yml
- filename: assetfare-app-store-api-openapi.yml
  format: yaml
  label: AssetFare App Store API
  slug: assetfare-app-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assetfare/refs/heads/main/openapi/assetfare-app-store-api-openapi.yml
- filename: assetfare-capabilities-api-openapi.yml
  format: yaml
  label: AssetFare Capabilities API
  slug: assetfare-capabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assetfare/refs/heads/main/openapi/assetfare-capabilities-api-openapi.yml
- filename: assetfare-events-api-openapi.yml
  format: yaml
  label: AssetFare Events API
  slug: assetfare-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assetfare/refs/heads/main/openapi/assetfare-events-api-openapi.yml
- filename: assetfare-google-play-api-openapi.yml
  format: yaml
  label: AssetFare Google Play API
  slug: assetfare-google-play-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assetfare/refs/heads/main/openapi/assetfare-google-play-api-openapi.yml
- filename: assetfare-jobs-api-openapi.yml
  format: yaml
  label: AssetFare Jobs API
  slug: assetfare-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assetfare/refs/heads/main/openapi/assetfare-jobs-api-openapi.yml
- filename: assetfare-prepare-api-openapi.yml
  format: yaml
  label: AssetFare Prepare API
  slug: assetfare-prepare-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assetfare/refs/heads/main/openapi/assetfare-prepare-api-openapi.yml
- filename: assetfare-search-filter-v-2-api-openapi.yml
  format: yaml
  label: AssetFare Search Filter v.2 API
  slug: assetfare-search-filter-v-2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assetfare/refs/heads/main/openapi/assetfare-search-filter-v-2-api-openapi.yml
- filename: assetfare-suggestions-api-openapi.yml
  format: yaml
  label: AssetFare Suggestions API
  slug: assetfare-suggestions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assetfare/refs/heads/main/openapi/assetfare-suggestions-api-openapi.yml
consequence_counts:
  read: 11
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Assetfare Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 25
overview: 'AssetFare exposes 25 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 14 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AssetFare
provider_slug: assetfare
slug: assetfare-agentic-access
source_filename: assetfare-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: generated\nsource: openapi/assetfare-auth-api-openapi.yml, openapi/assetfare-openapi.json, openapi/assetfare-quote-api-openapi.yml,\n  openapi/assetfare-session-api-openapi.yml, openapi/assetfare-status-api-openapi.yml, openapi/assetfare-well-known-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    acting: 14\n    connected: 11\n  by_consequence:\n    write: 14\n    read: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/auth/challenge\n  method: post\n  operationId: createWalletChallenge\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/verify\n  method: post\n  operationId: verifyWalletSignature\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/capabilities\n  method: get\n  operationId: getMultichainCapabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/prepare\n  method: post\n  operationId: prepareMultichainAction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/quote\n  method: post\n  operationId: quoteMultichainRoute\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/session\n  method: post\n  operationId: createMultichainSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/session/{session_id}\n  method: get\n  operationId: getMultichainSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/session/{session_id}/observe-output\n  method: post\n  operationId: observeOutputReceipt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/session/{session_id}/observe-source\n  method: post\n  operationId: observeSourceReceipt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/session/{session_id}/refresh-action\n  method: post\n  operationId: refreshMultichainAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/status\n  method: get\n\
  \  operationId: getMultichainStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/quote\n  method: post\n  operationId: getQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/session\n  method: post\n  operationId: createSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/session/{session_id}\n  method: get\n  operationId: getSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/session/{session_id}/next-action\n\
  \  method: get\n  operationId: getNextAction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/session/{session_id}/observe-cctp\n  method: post\n  operationId: observeCctp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/session/{session_id}/observe-destination\n  method: post\n  operationId: observeDestination\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/session/{session_id}/prepare-cctp-action\n  method:\
  \ post\n  operationId: prepareCctpAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/session/{session_id}/prepare-destination-action\n  method: post\n  operationId: prepareDestinationAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/session/{session_id}/prepare-source-action\n  method: post\n  operationId: prepareSourceAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/session/{session_id}/receipt\n  method: get\n  operationId: getReceipt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/session/{session_id}/verify-source\n  method: post\n  operationId: verifySourceReceipt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/session/{session_id}/workflow\n  method: get\n  operationId: getWorkflow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/status\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/assetfare-manifest.json\n  method: get\n  operationId: getSignedManifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/assetfare/refs/heads/main/agentic-access/assetfare-agentic-access.yml
summary_line: 25 operations · 14 acting
tags:
- AI Agents
- Asset Transfer
- Bridge
- Cross-Chain
- Non-Custodial
- Cryptocurrency
- Solana
- Base
- OpenAPI
- MCP
- Agent Skills
---
