---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 2
api_specs:
- filename: telefonica-number-verification-openapi.yml
  format: yaml
  label: Telefónica Number Verification API
  slug: number-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefonica/refs/heads/main/openapi/telefonica-number-verification-openapi.yml
- filename: telefonica-sim-swap-openapi.yml
  format: yaml
  label: Telefónica SIM Swap API
  slug: sim-swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefonica/refs/heads/main/openapi/telefonica-sim-swap-openapi.yml
- filename: telefonica-kyc-match-openapi.yml
  format: yaml
  label: Telefónica Know Your Customer Match API
  slug: kyc-match-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefonica/refs/heads/main/openapi/telefonica-kyc-match-openapi.yml
- filename: telefonica-location-verification-openapi.yml
  format: yaml
  label: Telefónica Location Verification API
  slug: location-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefonica/refs/heads/main/openapi/telefonica-location-verification-openapi.yml
- filename: telefonica-quality-on-demand-openapi.yml
  format: yaml
  label: Telefónica Quality on Demand API
  slug: quality-on-demand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefonica/refs/heads/main/openapi/telefonica-quality-on-demand-openapi.yml
- filename: telefonica-device-roaming-openapi.yml
  format: yaml
  label: Telefónica Device Roaming Status API
  slug: device-roaming-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefonica/refs/heads/main/openapi/telefonica-device-roaming-openapi.yml
consequence_counts:
  read: 2
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Telefonica Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'Telefónica exposes 11 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Telefónica
provider_slug: telefonica
slug: telefonica-agentic-access
source_filename: telefonica-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/telefonica-device-roaming-openapi.yml, openapi/telefonica-kyc-match-openapi.yml,\n  openapi/telefonica-location-verification-openapi.yml, openapi/telefonica-number-verification-openapi.yml,\n  openapi/telefonica-quality-on-demand-openapi.yml, openapi/telefonica-sim-swap-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    acting: 9\n    connected: 2\n  by_consequence:\n    write: 9\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /device-roaming/retrieve\n  method: post\n  operationId: getDeviceRoamingStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - device-roaming-status:read\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /kyc-match\n  method: post\n  operationId: matchKyc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - kyc-match:match\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /location-verification/verify\n  method: post\n  operationId: verifyDeviceLocation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - location-verification:verify\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /number-verification/verify\n\
  \  method: post\n  operationId: verifyPhoneNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - number-verification:verify\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /number-verification/share\n  method: post\n  operationId: getPhoneNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - number-verification:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /qod/sessions\n  method: post\n  operationId: createQodSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - qod:sessions:write\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /qod/sessions\n  method: get\n  operationId: listQodSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - qod:sessions:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /qod/sessions/{sessionId}\n  method: get\n  operationId: getQodSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - qod:sessions:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /qod/sessions/{sessionId}\n  method: delete\n  operationId: deleteQodSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - qod:sessions:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sim-swap/check\n  method: post\n  operationId: checkSimSwap\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - sim-swap:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sim-swap/retrieve-date\n  method: post\n  operationId: getSimSwapDate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - sim-swap:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telefonica/refs/heads/main/agentic-access/telefonica-agentic-access.yml
summary_line: 11 operations · 9 acting
tags:
- Telecommunications
- Mobile Network
- CAMARA
- Open Gateway
- Authentication
- Fraud Prevention
- Location Services
---
