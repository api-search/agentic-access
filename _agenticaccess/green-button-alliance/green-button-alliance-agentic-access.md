---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 16
api_specs:
- filename: green-button-alliance-applicationinformation-api-openapi.yml
  format: yaml
  label: Green Button Alliance Application Information API
  slug: green-button-alliance-applicationinformation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-button-alliance/refs/heads/main/openapi/green-button-alliance-applicationinformation-api-openapi.yml
- filename: green-button-alliance-authorization-api-openapi.yml
  format: yaml
  label: Green Button Alliance Authorization API
  slug: green-button-alliance-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-button-alliance/refs/heads/main/openapi/green-button-alliance-authorization-api-openapi.yml
- filename: green-button-alliance-batch-api-openapi.yml
  format: yaml
  label: Green Button Alliance Batch API
  slug: green-button-alliance-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-button-alliance/refs/heads/main/openapi/green-button-alliance-batch-api-openapi.yml
- filename: green-button-alliance-datacustodian-integration-api-openapi.yml
  format: yaml
  label: Green Button Alliance DataCustodian Integration API
  slug: green-button-alliance-datacustodian-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-button-alliance/refs/heads/main/openapi/green-button-alliance-datacustodian-integration-api-openapi.yml
- filename: green-button-alliance-oauth2-client-management-api-openapi.yml
  format: yaml
  label: Green Button Alliance OAuth2 Client Management API
  slug: green-button-alliance-oauth2-client-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-button-alliance/refs/heads/main/openapi/green-button-alliance-oauth2-client-management-api-openapi.yml
- filename: green-button-alliance-oauth2-standard-api-openapi.yml
  format: yaml
  label: Green Button Alliance OAuth2 Standard API
  slug: green-button-alliance-oauth2-standard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-button-alliance/refs/heads/main/openapi/green-button-alliance-oauth2-standard-api-openapi.yml
- filename: green-button-alliance-oidc-api-openapi.yml
  format: yaml
  label: Green Button Alliance OIDC API
  slug: green-button-alliance-oidc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-button-alliance/refs/heads/main/openapi/green-button-alliance-oidc-api-openapi.yml
- filename: green-button-alliance-usagepoint-api-openapi.yml
  format: yaml
  label: Green Button Alliance Usage Point API
  slug: green-button-alliance-usagepoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-button-alliance/refs/heads/main/openapi/green-button-alliance-usagepoint-api-openapi.yml
consequence_counts:
  read: 16
  safety-critical: 1
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Green Button Alliance Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /oauth2/revoke
operation_count: 23
overview: 'Green Button Alliance exposes 23 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read, 6 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Green Button Alliance
provider_slug: green-button-alliance
slug: green-button-alliance-agentic-access
source_filename: green-button-alliance-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/green-button-alliance-applicationinformation-api-openapi.yml, openapi/green-button-alliance-authorization-api-openapi.yml,\n  openapi/green-button-alliance-batch-api-openapi.yml, openapi/green-button-alliance-datacustodian-integration-api-openapi.yml,\n  openapi/green-button-alliance-oauth2-client-management-api-openapi.yml, openapi/green-button-alliance-oauth2-standard-api-openapi.yml,\n  openapi/green-button-alliance-oidc-api-openapi.yml, openapi/green-button-alliance-usagepoint-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 16\n    acting: 7\n  by_consequence:\n    read: 16\n    write: 6\n    safety-critical: 1\n  human_in_the_loop_required:\
  \ 1\noperations:\n- path: /espi/1_1/resource/ApplicationInformation\n  method: get\n  operationId: findApplicationInformations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /espi/1_1/resource/ApplicationInformation/{applicationInformationId}\n  method: get\n  operationId: getApplicationInformation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /espi/1_1/resource/Authorization\n  method: get\n  operationId: findAuthorizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /espi/1_1/resource/Authorization/{authorizationId}\n  method: get\n  operationId: getAuthorization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /espi/1_1/resource/Batch/Bulk/{bulkId}\n  method: get\n  operationId: downloadBulkData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/datacustodian/verify-user\n  method: post\n  operationId: postApiV1DatacustodianVerifyUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/datacustodian/customers/{customerId}\n  method: get\n  operationId: getApiV1DatacustodianCustomersByCustomerId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/datacustodian/customers/{customerId}/usage-points\n\
  \  method: get\n  operationId: getApiV1DatacustodianCustomersByCustomerIdUsagePoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/datacustodian/health\n  method: get\n  operationId: getApiV1DatacustodianHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/oauth2/clients\n  method: get\n  operationId: getApiV1Oauth2Clients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/oauth2/clients\n  method: post\n  operationId: postApiV1Oauth2Clients\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n     \
  \ triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/oauth2/clients/{clientId}\n  method: get\n  operationId: getApiV1Oauth2ClientsByClientId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/oauth2/clients/{clientId}\n  method: put\n  operationId: putApiV1Oauth2ClientsByClientId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/oauth2/clients/{clientId}\n  method: delete\n  operationId: deleteApiV1Oauth2ClientsByClientId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/oauth2/clients/{clientId}/metrics\n  method: get\n  operationId: getApiV1Oauth2ClientsByClientIdMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth2/authorize\n  method: get\n  operationId: getOauth2Authorize\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth2/token\n  method: post\n  operationId: postOauth2Token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth2/introspect\n  method: post\n  operationId: postOauth2Introspect\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth2/revoke\n  method: post\n  operationId: postOauth2Revoke\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /userinfo\n  method: get\n  operationId: getUserinfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - openid\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /userinfo\n  method: post\n  operationId: postUserinfo\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    scope:\n    - openid\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /espi/1_1/resource/UsagePoint\n  method: get\n  operationId: findUsagePoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /espi/1_1/resource/UsagePoint/{usagePointId}\n  method: get\n  operationId: getUsagePoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/green-button-alliance/refs/heads/main/agentic-access/green-button-alliance-agentic-access.yml
summary_line: 23 operations · 7 acting · 1 human-in-the-loop
tags:
- Energy
- United States
- Utilities
- Electricity
- Gas
- Water
- Smart Metering
- Green Button
- ESPI
- Standards Body
- Certification
- Consumer Energy Data
---
