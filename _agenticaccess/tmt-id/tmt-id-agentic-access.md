---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 6
api_specs:
- filename: tmt-id-authenticate-api-openapi.yml
  format: yaml
  label: TMT ID Authenticate API
  slug: tmt-id-authenticate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tmt-id/refs/heads/main/openapi/tmt-id-authenticate-api-openapi.yml
- filename: tmt-id-http-api-api-openapi.yml
  format: yaml
  label: TMT ID HTTP API
  slug: tmt-id-http-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tmt-id/refs/heads/main/openapi/tmt-id-http-api-api-openapi.yml
- filename: tmt-id-http-api-v1-3-api-openapi.yml
  format: yaml
  label: TMT ID HTTP API v1.3 API
  slug: tmt-id-http-api-v1-3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tmt-id/refs/heads/main/openapi/tmt-id-http-api-v1-3-api-openapi.yml
- filename: tmt-id-http-api-v2-0-api-openapi.yml
  format: yaml
  label: TMT ID HTTP API v2.0 API
  slug: tmt-id-http-api-v2-0-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tmt-id/refs/heads/main/openapi/tmt-id-http-api-v2-0-api-openapi.yml
- filename: tmt-id-network-biometrics-api-openapi.yml
  format: yaml
  label: TMT ID Network Biometrics API
  slug: tmt-id-network-biometrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tmt-id/refs/heads/main/openapi/tmt-id-network-biometrics-api-openapi.yml
- filename: tmt-id-service-api-openapi.yml
  format: yaml
  label: TMT ID Service API
  slug: tmt-id-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tmt-id/refs/heads/main/openapi/tmt-id-service-api-openapi.yml
- filename: tmt-id-standard-api-call-api-openapi.yml
  format: yaml
  label: TMT ID Standard API Call API
  slug: tmt-id-standard-api-call-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tmt-id/refs/heads/main/openapi/tmt-id-standard-api-call-api-openapi.yml
- filename: tmt-id-v2-deprecated-api-openapi.yml
  format: yaml
  label: TMT ID v2 (deprecated) API
  slug: tmt-id-v2-deprecated-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tmt-id/refs/heads/main/openapi/tmt-id-v2-deprecated-api-openapi.yml
consequence_counts:
  read: 6
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tmt Id Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'TMT ID exposes 17 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 11 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: TMT ID
provider_slug: tmt-id
slug: tmt-id-agentic-access
source_filename: tmt-id-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/tmt-id-authenticate-api-openapi.yml, openapi/tmt-id-http-api-api-openapi.yml,\n  openapi/tmt-id-http-api-v1-3-api-openapi.yml, openapi/tmt-id-http-api-v2-0-api-openapi.yml,\n  openapi/tmt-id-network-biometrics-api-openapi.yml, openapi/tmt-id-service-api-openapi.yml,\n  openapi/tmt-id-standard-api-call-api-openapi.yml, openapi/tmt-id-v2-deprecated-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    acting: 11\n    connected: 6\n  by_consequence:\n    write: 11\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /oauth/token\n  method: post\n  operationId: getAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /get_config\n  method: post\n  operationId: getConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /validate\n  method: post\n  operationId: validateUserSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{format}/{key}/{secret}/{number}\n  method: get\n  operationId: GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /score/{number}\n  method: get\n  operationId: GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /standard/{format}/{key}/{secret}/{number}\n  method: get\n  operationId: GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /teleshield/{number}\n  method: post\n  operationId: POST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /e-teleshield/{number v1.3}\n  method: post\n  operationId: POST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n  \
  \  escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /r-teleshield/{number}\n  method: post\n  operationId: POST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /f-teleshield/{number}\n  method: post\n  operationId: POST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /e-teleshield/{number v2.0}\n  method: post\n  operationId: POST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /network-biometrics\n  method: post\n  operationId: post-network-biometrics\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /authenticate\n  method: get\n  operationId: authenticateUserWithMNO\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authenticate/otp\n  method: get\n  operationId: authenticateUserWithOtp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/\n\
  \  method: post\n  operationId: POST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /core/v2/NumberAssurance/AssuredRegistration\n  method: post\n  operationId: post-assured-registration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /core/v2/NumberAssurance/AssuredAge\n  method: post\n  operationId: post-assured-age\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tmt-id/refs/heads/main/agentic-access/tmt-id-agentic-access.yml
summary_line: 17 operations · 11 acting
tags:
- Telecommunications
- United Kingdom
- Identity Verification
- Mobile Identity
- SIM Swap
- Fraud Prevention
- Number Intelligence
- Silent Network Authentication
- GSMA Open Gateway
- Network APIs
- ENUM
- KYC
---
