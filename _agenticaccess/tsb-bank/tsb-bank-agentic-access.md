---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 25
api_specs:
- filename: tsb-bank-atm-api-openapi.yml
  format: yaml
  label: TSB Bank ATM API
  slug: tsb-bank-atm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tsb-bank/refs/heads/main/openapi/tsb-bank-atm-api-openapi.yml
- filename: tsb-bank-authorization-server-apis-api-openapi.yml
  format: yaml
  label: TSB Bank Authorization Server APIs API
  slug: tsb-bank-authorization-server-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tsb-bank/refs/heads/main/openapi/tsb-bank-authorization-server-apis-api-openapi.yml
- filename: tsb-bank-bca-api-openapi.yml
  format: yaml
  label: TSB Bank BCA API
  slug: tsb-bank-bca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tsb-bank/refs/heads/main/openapi/tsb-bank-bca-api-openapi.yml
- filename: tsb-bank-branch-api-openapi.yml
  format: yaml
  label: TSB Bank Branch API
  slug: tsb-bank-branch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tsb-bank/refs/heads/main/openapi/tsb-bank-branch-api-openapi.yml
- filename: tsb-bank-ccc-api-openapi.yml
  format: yaml
  label: TSB Bank CCC API
  slug: tsb-bank-ccc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tsb-bank/refs/heads/main/openapi/tsb-bank-ccc-api-openapi.yml
- filename: tsb-bank-pca-api-openapi.yml
  format: yaml
  label: TSB Bank PCA API
  slug: tsb-bank-pca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tsb-bank/refs/heads/main/openapi/tsb-bank-pca-api-openapi.yml
- filename: tsb-bank-resource-server-apis-api-openapi.yml
  format: yaml
  label: TSB Bank Resource Server APIs API
  slug: tsb-bank-resource-server-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tsb-bank/refs/heads/main/openapi/tsb-bank-resource-server-apis-api-openapi.yml
- filename: tsb-bank-sme-api-openapi.yml
  format: yaml
  label: TSB Bank SME API
  slug: tsb-bank-sme-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tsb-bank/refs/heads/main/openapi/tsb-bank-sme-api-openapi.yml
- filename: tsb-bank-token-server-apis-api-openapi.yml
  format: yaml
  label: TSB Bank Token Server APIs API
  slug: tsb-bank-token-server-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tsb-bank/refs/heads/main/openapi/tsb-bank-token-server-apis-api-openapi.yml
consequence_counts:
  read: 25
  safety-critical: 1
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Tsb Bank Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /auth/oauth/v2/token/revoke
operation_count: 31
overview: 'TSB Bank exposes 31 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 25 read, 5 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: TSB Bank
provider_slug: tsb-bank
slug: tsb-bank-agentic-access
source_filename: tsb-bank-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: generated\nsource: openapi/obie-open-data-openapi.json, openapi/tsb-bank-oauth-server-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 31\n  by_action_class:\n    connected: 25\n    acting: 6\n  by_consequence:\n    read: 25\n    write: 5\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /branches\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /branches\n  method: head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /atms\n  method: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /atms\n  method: head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /personal-current-accounts\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /personal-current-accounts\n  method: head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /business-current-accounts\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /business-current-accounts\n  method: head\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /unsecured-sme-loans\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /unsecured-sme-loans\n  method: head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /commercial-credit-cards\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /commercial-credit-cards\n  method: head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/oauth/v2/authorize\n  method: get\n  operationId: Get_request_authorization\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openid/connect/v1/userinfo\n  method: get\n  operationId: Get_userinfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/oauth/health\n  method: get\n  operationId: Get_request_health_check\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/oauth/v2/authorize/login\n  method: get\n  operationId: Get_request_authorize_login\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/oauth/v2/authorize/login\n  method: post\n  operationId: Post_request_authorize_login\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/oauth/v2/authorize/consent\n  method: post\n  operationId: Post_request_authorize_consent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/oauth/v2/token\n  method: post\n  operationId: Create_request_token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/oauth/v2/token/revoke\n  method: post\n  operationId: revoke_token\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /auth/oauth/v2/client/export\n  method: get\n  operationId: Get_client_details_export_\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connect/session/status\n  method: get\n  operationId: Get_resource_owner_session_status_\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connect/session/logout\n  method: post\n  operationId: Create_resource_owner_logout_\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /.well-known/openid-configuration\n  method: options\n  operationId: Options_getOpenIDDiscovery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/openid-configuration\n  method: get\n  operationId: Get_OpenIDDiscovery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openid/connect/register\n  method: options\n  operationId: Options_oidc_register\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openid/connect/register\n  method: post\n  operationId: Post_oidc_register\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openid/connect/register/{client_id}\n  method: options\n  operationId: Options_oidc_register_config\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openid/connect/register/{client_id}\n  method: get\n  operationId: Get_oidc_register_config\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openid/connect/jwks.json\n  method: options\n  operationId: Options_jwk_set_\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openid/connect/jwks.json\n\
  \  method: get\n  operationId: Get_jwk_set_\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tsb-bank/refs/heads/main/agentic-access/tsb-bank-agentic-access.yml
summary_line: 31 operations · 6 acting · 1 human-in-the-loop
tags:
- Financial-Services
- Banking
- Open Banking
- PSD2
- OBIE
- United Kingdom
- Payments
- Account Information
- FAPI
- Fintech
---
