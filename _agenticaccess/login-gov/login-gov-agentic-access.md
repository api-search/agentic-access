---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 7
api_specs:
- filename: login-gov-oidc-openapi.yml
  format: yaml
  label: Login.gov OpenID Connect API
  slug: login-gov-oidc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/login-gov/refs/heads/main/openapi/login-gov-oidc-openapi.yml
- filename: login-gov-saml-openapi.yml
  format: yaml
  label: Login.gov SAML 2.0 API
  slug: login-gov-saml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/login-gov/refs/heads/main/openapi/login-gov-saml-openapi.yml
consequence_counts:
  read: 7
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Login Gov Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Login.gov exposes 9 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Login.gov
provider_slug: login-gov
slug: login-gov-agentic-access
source_filename: login-gov-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/login-gov-oidc-openapi.yml, openapi/login-gov-saml-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 7\n    acting: 2\n  by_consequence:\n    read: 7\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /.well-known/openid-configuration\n  method: get\n  operationId: getOpenidConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/openid_connect/certs\n  method: get\n  operationId: getJwks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /openid_connect/authorize\n  method: get\n  operationId: authorize\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/openid_connect/token\n  method: post\n  operationId: exchangeToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/openid_connect/userinfo\n  method: get\n  operationId: getUserInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openid_connect/logout\n  method: get\n  operationId: logout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n \
  \   token:\n      max-ttl: 3600\n    audit: none\n- path: /api/saml/metadata2026\n  method: get\n  operationId: getSamlMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/saml/auth2026\n  method: get\n  operationId: samlSso\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/saml/logout2026\n  method: post\n  operationId: samlSlo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/login-gov/refs/heads/main/agentic-access/login-gov-agentic-access.yml
summary_line: 9 operations · 2 acting
tags:
- Government
- Federal
- GSA
- Identity
- Authentication
- SSO
- OIDC
- SAML
- IAL2
- AAL2
---
