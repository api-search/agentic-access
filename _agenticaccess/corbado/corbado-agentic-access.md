---
acting_count: 20
action_class_counts:
  acting: 20
  connected: 9
api_specs:
- filename: corbado-openapi.yml
  format: yaml
  label: Corbado Users API
  slug: corbado-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/corbado/refs/heads/main/openapi/corbado-openapi.yml
- filename: corbado-openapi.yml
  format: yaml
  label: Corbado Identifiers API
  slug: corbado-identifiers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/corbado/refs/heads/main/openapi/corbado-openapi.yml
- filename: corbado-openapi.yml
  format: yaml
  label: Corbado Sessions API
  slug: corbado-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/corbado/refs/heads/main/openapi/corbado-openapi.yml
- filename: corbado-openapi.yml
  format: yaml
  label: Corbado Passkeys API
  slug: corbado-passkeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/corbado/refs/heads/main/openapi/corbado-openapi.yml
- filename: corbado-openapi.yml
  format: yaml
  label: Corbado Connect Tokens API
  slug: corbado-connect-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/corbado/refs/heads/main/openapi/corbado-openapi.yml
- filename: corbado-openapi.yml
  format: yaml
  label: Corbado Projects API
  slug: corbado-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/corbado/refs/heads/main/openapi/corbado-openapi.yml
consequence_counts:
  read: 9
  safety-critical: 1
  write: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Corbado Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /sessions/{sessionID}/revoke
operation_count: 29
overview: 'Corbado exposes 29 API operations that an AI agent could call, of which 20 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 19 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Corbado
provider_slug: corbado
slug: corbado-agentic-access
source_filename: corbado-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/corbado-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 29\n  by_action_class:\n    acting: 20\n    connected: 9\n  by_consequence:\n    write: 19\n    read: 9\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /users\n  method: post\n  operationId: userCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users\n  method: get\n  operationId: userList\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{userID}\n  method: get\n  operationId: userGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{userID}\n  method: patch\n  operationId: userUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{userID}\n  method: delete\n  operationId: userDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{userID}/credentials\n\
  \  method: get\n  operationId: userCredentialList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{userID}/credentials/{credentialID}\n  method: delete\n  operationId: userCredentialDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{userID}/identifiers\n  method: post\n  operationId: identifierCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{userID}/identifiers/{identifierID}\n  method:\
  \ patch\n  operationId: identifierUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{userID}/identifiers/{identifierID}\n  method: delete\n  operationId: identifierDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identifiers\n  method: get\n  operationId: identifierList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions\n  method: get\n  operationId: sessionList\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions/{sessionID}/revoke\n  method: post\n  operationId: sessionRevoke\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /passkey/append/start\n  method: post\n  operationId: passkeyAppendStart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /passkey/append/finish\n  method: post\n  operationId: passkeyAppendFinish\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /passkey/login/start\n  method: post\n  operationId: passkeyLoginStart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /passkey/login/finish\n  method: post\n  operationId: passkeyLoginFinish\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /passkey/mediation/start\n  method:\
  \ post\n  operationId: passkeyMediationStart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /passkey/mediation/finish\n  method: post\n  operationId: passkeyMediationFinish\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /passkey/verifySignedData\n  method: post\n  operationId: passkeyVerifySignedData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /users/{userID}/passkeyEvents\n  method: post\n  operationId: passkeyEventCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{userID}/passkeyEvents\n  method: get\n  operationId: passkeyEventList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{userID}/passkeyEvents/{passkeyEventID}\n  method: delete\n  operationId: passkeyEventDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /connectTokens\n  method: post\n  operationId: connectTokenCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connectTokens\n  method: get\n  operationId: connectTokenList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connectTokens/{connectTokenID}\n  method: patch\n  operationId: connectTokenUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connectTokens/{connectTokenID}\n\
  \  method: delete\n  operationId: connectTokenDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /exports/{exportType}\n  method: get\n  operationId: exportList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exports/{exportType}/{filename}/downloadLink\n  method: get\n  operationId: exportDownloadLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/corbado/refs/heads/main/agentic-access/corbado-agentic-access.yml
summary_line: 29 operations · 20 acting · 1 human-in-the-loop
tags:
- Authentication
- Passkeys
- WebAuthn
- Passwordless
- CIAM
- Identity
---
