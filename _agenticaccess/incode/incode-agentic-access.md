---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 5
api_specs:
- filename: incode-openapi.yml
  format: yaml
  label: Incode Onboarding Sessions API
  slug: incode-onboarding-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/incode/refs/heads/main/openapi/incode-openapi.yml
- filename: incode-openapi.yml
  format: yaml
  label: Incode ID Verification API
  slug: incode-id-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/incode/refs/heads/main/openapi/incode-openapi.yml
- filename: incode-openapi.yml
  format: yaml
  label: Incode Face and Liveness API
  slug: incode-face-liveness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/incode/refs/heads/main/openapi/incode-openapi.yml
- filename: incode-openapi.yml
  format: yaml
  label: Incode Government Validation API
  slug: incode-government-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/incode/refs/heads/main/openapi/incode-openapi.yml
- filename: incode-openapi.yml
  format: yaml
  label: Incode Watchlist and AML API
  slug: incode-watchlist-aml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/incode/refs/heads/main/openapi/incode-openapi.yml
- filename: incode-openapi.yml
  format: yaml
  label: Incode Results API
  slug: incode-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/incode/refs/heads/main/openapi/incode-openapi.yml
- filename: incode-openapi.yml
  format: yaml
  label: Incode Webhooks API
  slug: incode-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/incode/refs/heads/main/openapi/incode-openapi.yml
consequence_counts:
  read: 5
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Incode Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'Incode exposes 14 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Incode
provider_slug: incode
slug: incode-agentic-access
source_filename: incode-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/incode-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    acting: 9\n    connected: 5\n  by_consequence:\n    write: 9\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /omni/start\n  method: post\n  operationId: startOnboarding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /omni/add/front-id/v2\n  method: post\n  operationId: addFrontId\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /omni/add/back-id/v2\n  method: post\n  operationId: addBackId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /omni/process/id\n  method: post\n  operationId: processId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /omni/add/face/third-party\n  method: post\n  operationId: addFace\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /omni/process/face\n  method: post\n  operationId: processFace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /omni/process/government-validation\n  method: post\n  operationId: processGovernmentValidation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /omni/process/global-watchlist\n\
  \  method: post\n  operationId: processGlobalWatchlist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /omni/watchlist-result\n  method: post\n  operationId: watchlistResult\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /omni/updated-watchlist-result\n  method: get\n  operationId: updatedWatchlistResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /omni/finish-status\n  method: get\n  operationId: finishStatus\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /omni/get/score\n  method: get\n  operationId: getScore\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /omni/get/ocr-data\n  method: get\n  operationId: getOcrData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /omni/get/images\n  method: get\n  operationId: getImages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/incode/refs/heads/main/agentic-access/incode-agentic-access.yml
summary_line: 14 operations · 9 acting
tags:
- Identity Verification
- Biometrics
- KYC
- Liveness
- Onboarding
---
