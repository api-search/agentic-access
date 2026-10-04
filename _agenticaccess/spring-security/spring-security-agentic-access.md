---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 8
api_specs:
- filename: spring-security-authorization-api-openapi.yml
  format: yaml
  label: Spring Security Authorization API
  slug: spring-security-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-security/refs/heads/main/openapi/spring-security-authorization-api-openapi.yml
- filename: spring-security-client-management-api-openapi.yml
  format: yaml
  label: Spring Security Client Management API
  slug: spring-security-client-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-security/refs/heads/main/openapi/spring-security-client-management-api-openapi.yml
- filename: spring-security-device-api-openapi.yml
  format: yaml
  label: Spring Security Device API
  slug: spring-security-device-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-security/refs/heads/main/openapi/spring-security-device-api-openapi.yml
- filename: spring-security-discovery-api-openapi.yml
  format: yaml
  label: Spring Security Discovery API
  slug: spring-security-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-security/refs/heads/main/openapi/spring-security-discovery-api-openapi.yml
- filename: spring-security-keys-api-openapi.yml
  format: yaml
  label: Spring Security Keys API
  slug: spring-security-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-security/refs/heads/main/openapi/spring-security-keys-api-openapi.yml
- filename: spring-security-openid-connect-api-openapi.yml
  format: yaml
  label: Spring Security OpenID Connect API
  slug: spring-security-openid-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-security/refs/heads/main/openapi/spring-security-openid-connect-api-openapi.yml
- filename: spring-security-session-api-openapi.yml
  format: yaml
  label: Spring Security Session API
  slug: spring-security-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-security/refs/heads/main/openapi/spring-security-session-api-openapi.yml
- filename: spring-security-token-api-openapi.yml
  format: yaml
  label: Spring Security Token API
  slug: spring-security-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-security/refs/heads/main/openapi/spring-security-token-api-openapi.yml
consequence_counts:
  read: 8
  safety-critical: 1
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Spring Security Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /oauth2/revoke
operation_count: 15
overview: 'Spring Security exposes 15 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 6 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Spring Security
provider_slug: spring-security
slug: spring-security-agentic-access
source_filename: spring-security-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/spring-security-authorization-api-openapi.yml, openapi/spring-security-client-management-api-openapi.yml,\n  openapi/spring-security-device-api-openapi.yml, openapi/spring-security-discovery-api-openapi.yml,\n  openapi/spring-security-keys-api-openapi.yml, openapi/spring-security-openid-connect-api-openapi.yml,\n  openapi/spring-security-session-api-openapi.yml, openapi/spring-security-token-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 8\n    acting: 7\n  by_consequence:\n    read: 8\n    write: 6\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /oauth2/authorize\n  method: get\n  operationId: authorizationRequest\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connect/register\n  method: post\n  operationId: registerClient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth2/device_authorization\n  method: post\n  operationId: deviceAuthorization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /.well-known/openid-configuration\n  method: get\n  operationId: getOidcDiscovery\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-authorization-server\n  method: get\n  operationId: getOAuthMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth2/jwks\n  method: get\n  operationId: getJwks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /userinfo\n  method: get\n  operationId: getUserInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /userinfo\n  method: post\n  operationId: getUserInfoPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connect/logout\n  method:\
  \ get\n  operationId: oidcLogout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /logout\n  method: post\n  operationId: logout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /login\n  method: get\n  operationId: getLoginPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /login\n  method: post\n  operationId: processLogin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n \
  \     - abnormal\n      - high-value\n    audit: required\n- path: /oauth2/token\n  method: post\n  operationId: tokenRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth2/introspect\n  method: post\n  operationId: tokenIntrospection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth2/revoke\n  method: post\n  operationId: tokenRevocation\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange:\
  \ true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spring-security/refs/heads/main/agentic-access/spring-security-agentic-access.yml
summary_line: 15 operations · 7 acting · 1 human-in-the-loop
tags:
- Authentication
- Authorization
- Java
- JWT
- OpenID Connect
- SAML
- Security
- Spring Framework
- Identity Federation
---
