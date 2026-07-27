---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 5
api_specs:
- filename: tmt-id-verify.yml
  format: yaml
  label: TMT Verify API
  slug: tmt-id-verify
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tmt-id/refs/heads/main/openapi/tmt-id-verify.yml
- filename: tmt-id-velocity.yml
  format: yaml
  label: TMT Velocity API
  slug: tmt-id-velocity
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tmt-id/refs/heads/main/openapi/tmt-id-velocity.yml
- filename: tmt-id-live.yml
  format: yaml
  label: TMT Live API
  slug: tmt-id-live
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tmt-id/refs/heads/main/openapi/tmt-id-live.yml
- filename: tmt-id-teleshield.yml
  format: yaml
  label: TMT TeleShield API
  slug: tmt-id-teleshield
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tmt-id/refs/heads/main/openapi/tmt-id-teleshield.yml
- filename: tmt-id-score.yml
  format: yaml
  label: TMT Score API
  slug: tmt-id-score
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tmt-id/refs/heads/main/openapi/tmt-id-score.yml
- filename: tmt-id-authenticate.yml
  format: yaml
  label: TMT Authenticate API
  slug: tmt-id-authenticate
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tmt-id/refs/heads/main/openapi/tmt-id-authenticate.yml
- filename: tmt-id-network-biometrics.yml
  format: yaml
  label: Network Biometrics API
  slug: tmt-id-network-biometrics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tmt-id/refs/heads/main/openapi/tmt-id-network-biometrics.yml
consequence_counts:
  physical: 2
  read: 5
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tmt Id Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /get_config
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /validate
operation_count: 17
overview: 'TMT ID exposes 17 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read, 10 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: TMT ID
provider_slug: tmt-id
slug: tmt-id-agentic-access
source_filename: tmt-id-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: generated\nsource: openapi/tmt-id-authenticate.yml, openapi/tmt-id-live.yml, openapi/tmt-id-network-biometrics.yml,\n  openapi/tmt-id-score.yml, openapi/tmt-id-teleshield.yml, openapi/tmt-id-velocity.yml, openapi/tmt-id-verify.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    acting: 12\n    connected: 5\n  by_consequence:\n    write: 10\n    physical: 2\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /oauth/token\n  method: post\n  operationId: getAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /get_config\n  method: post\n  operationId: getConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /validate\n  method: post\n  operationId: validateUserSession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /authenticate\n  method: get\n  operationId: authenticateUserWithMNO\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authenticate/otp\n  method: get\n  operationId: authenticateUserWithOtp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{format}/{key}/{secret}/{number}\n  method: get\n  operationId: GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /network-biometrics\n  method: post\n  operationId: post-network-biometrics\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /core/v2/NumberAssurance/AssuredRegistration\n  method: post\n  operationId: post-assured-registration\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /core/v2/NumberAssurance/AssuredAge\n  method: post\n  operationId: post-assured-age\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /score/{number}\n  method: get\n  operationId: GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /r-teleshield/{number}\n  method: post\n  operationId: POST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /f-teleshield/{number}\n  method: post\n  operationId: POST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /e-teleshield/{number v2.0}\n  method: post\n  operationId: POST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /teleshield/{number}\n  method: post\n  operationId: POST\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /e-teleshield/{number v1.3}\n  method: post\n  operationId: POST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /standard/{format}/{key}/{secret}/{number}\n  method: get\n  operationId: GET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/\n  method: post\n  operationId: POST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tmt-id/refs/heads/main/agentic-access/tmt-id-agentic-access.yml
summary_line: 17 operations · 12 acting
tags:
- Telecommunications
- United Kingdom
- Identity Verification
- Mobile Identity
- SIM Swap
- Anti-Fraud
- Number Intelligence
- Silent Network Authentication
- GSMA Open Gateway
- Network APIs
- ENUM
- KYC
---
