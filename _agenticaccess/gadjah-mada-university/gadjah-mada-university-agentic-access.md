---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 17
api_specs:
- filename: gadjah-mada-university-discovery-api-openapi.yml
  format: yaml
  label: Gadjah Mada University Discovery API
  slug: gadjah-mada-university-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gadjah-mada-university/refs/heads/main/openapi/gadjah-mada-university-discovery-api-openapi.yml
- filename: gadjah-mada-university-infra-api-openapi.yml
  format: yaml
  label: Gadjah Mada University Infra API
  slug: gadjah-mada-university-infra-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gadjah-mada-university/refs/heads/main/openapi/gadjah-mada-university-infra-api-openapi.yml
- filename: gadjah-mada-university-oai-pmh-api-openapi.yml
  format: yaml
  label: Gadjah Mada University OAI PMH API
  slug: gadjah-mada-university-oai-pmh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gadjah-mada-university/refs/heads/main/openapi/gadjah-mada-university-oai-pmh-api-openapi.yml
- filename: gadjah-mada-university-social-login-api-openapi.yml
  format: yaml
  label: Gadjah Mada University Social Login API
  slug: gadjah-mada-university-social-login-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gadjah-mada-university/refs/heads/main/openapi/gadjah-mada-university-social-login-api-openapi.yml
- filename: gadjah-mada-university-oauth2-api-openapi.yml
  format: yaml
  label: Gadjah Mada University O Auth2 API
  slug: gadjah-mada-university-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gadjah-mada-university/refs/heads/main/openapi/gadjah-mada-university-oauth2-api-openapi.yml
- filename: gadjah-mada-university-me-api-openapi.yml
  format: yaml
  label: Gadjah Mada University Me API
  slug: gadjah-mada-university-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gadjah-mada-university/refs/heads/main/openapi/gadjah-mada-university-me-api-openapi.yml
- filename: gadjah-mada-university-user-api-openapi.yml
  format: yaml
  label: Gadjah Mada University User API
  slug: gadjah-mada-university-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gadjah-mada-university/refs/heads/main/openapi/gadjah-mada-university-user-api-openapi.yml
consequence_counts:
  read: 17
  safety-critical: 1
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Gadjah Mada University Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /oauth/revoke
operation_count: 21
overview: 'Gadjah Mada University exposes 21 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read, 3 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Gadjah Mada University
provider_slug: gadjah-mada-university
slug: gadjah-mada-university-agentic-access
source_filename: gadjah-mada-university-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: generated\nsource: openapi/gadjah-mada-university-discovery-api-openapi.yml, openapi/gadjah-mada-university-infra-api-openapi.yml,\n  openapi/gadjah-mada-university-me-api-openapi.yml, openapi/gadjah-mada-university-oai-pmh-api-openapi.yml,\n  openapi/gadjah-mada-university-oauth2-api-openapi.yml, openapi/gadjah-mada-university-social-login-api-openapi.yml,\n  openapi/gadjah-mada-university-user-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    connected: 17\n    acting: 4\n  by_consequence:\n    read: 17\n    write: 3\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /.well-known/jwks.json\n  method: get\n  operationId: getJwks\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-authorization-server\n  method: get\n  operationId: getOAuthMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/openid-configuration\n  method: get\n  operationId: getOidcConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: healthCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/me\n  method: get\n  operationId: getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /index/oai\n  method: get\n  operationId: oaiRequestAllJournals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oai2\n  method: get\n  operationId: oaiRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/authorize\n  method: get\n  operationId: authorizeUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/introspect\n  method: post\n  operationId: introspectToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /oauth/logout\n  method: get\n  operationId: logoutUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/revoke\n  method: post\n  operationId: revokeToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /oauth/token\n  method: post\n  operationId: getToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /userinfo\n  method: get\n  operationId: getUserInfo\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorize/apple\n  method: get\n  operationId: authorizeApple\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorize/facebook\n  method: get\n  operationId: authorizeFacebook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorize/google\n  method: get\n  operationId: authorizeGoogle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorize/linkedin\n  method: get\n  operationId: authorizeLinkedin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /authorize/microsoft\n  method: get\n  operationId: authorizeMicrosoft\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /callback/apple\n  method: post\n  operationId: callbackApple\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/me\n  method: get\n  operationId: getUserMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/username/{username}\n  method: get\n  operationId: getUserByUsername\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gadjah-mada-university/refs/heads/main/agentic-access/gadjah-mada-university-agentic-access.yml
summary_line: 21 operations · 4 acting · 1 human-in-the-loop
tags:
- University
- Higher Education
- Education
- Indonesia
- Research
- Identity Federation
- Authentication
- Research Repository
- Scholarly Publishing
- OAI-PMH
- Library
---
