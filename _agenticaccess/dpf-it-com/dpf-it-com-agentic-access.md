---
acting_count: 28
action_class_counts:
  acting: 28
  connected: 8
api_specs:
- filename: dpf-it-com-account-api-openapi.yml
  format: yaml
  label: DPF Account API
  slug: dpf-it-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dpf-it-com/openapi/dpf-it-com-account-api-openapi.yml
- filename: dpf-it-com-authentication-api-openapi.yml
  format: yaml
  label: DPF Authentication API
  slug: dpf-it-com-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dpf-it-com/openapi/dpf-it-com-authentication-api-openapi.yml
- filename: dpf-it-com-connections-api-openapi.yml
  format: yaml
  label: DPF Connections API
  slug: dpf-it-com-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dpf-it-com/openapi/dpf-it-com-connections-api-openapi.yml
- filename: dpf-it-com-contact-api-openapi.yml
  format: yaml
  label: DPF Contact API
  slug: dpf-it-com-contact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dpf-it-com/openapi/dpf-it-com-contact-api-openapi.yml
- filename: dpf-it-com-data-specs-api-openapi.yml
  format: yaml
  label: DPF Data Specs API
  slug: dpf-it-com-data-specs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dpf-it-com/openapi/dpf-it-com-data-specs-api-openapi.yml
- filename: dpf-it-com-iceberg-rest-catalog-api-openapi.yml
  format: yaml
  label: DPF Iceberg REST Catalog API
  slug: dpf-it-com-iceberg-rest-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dpf-it-com/openapi/dpf-it-com-iceberg-rest-catalog-api-openapi.yml
- filename: dpf-it-com-job-triggers-api-openapi.yml
  format: yaml
  label: DPF Job Triggers API
  slug: dpf-it-com-job-triggers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dpf-it-com/openapi/dpf-it-com-job-triggers-api-openapi.yml
- filename: dpf-it-com-mcp-api-openapi.yml
  format: yaml
  label: DPF MCP API
  slug: dpf-it-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dpf-it-com/openapi/dpf-it-com-mcp-api-openapi.yml
- filename: dpf-it-com-oauth-2-1-authorization-server-api-openapi.yml
  format: yaml
  label: DPF OAuth 2.1 Authorization Server API
  slug: dpf-it-com-oauth-2-1-authorization-server-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dpf-it-com/openapi/dpf-it-com-oauth-2-1-authorization-server-api-openapi.yml
- filename: dpf-it-com-query-api-openapi.yml
  format: yaml
  label: DPF Query API
  slug: dpf-it-com-query-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dpf-it-com/openapi/dpf-it-com-query-api-openapi.yml
- filename: dpf-it-com-workspaces-api-openapi.yml
  format: yaml
  label: DPF Workspaces API
  slug: dpf-it-com-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dpf-it-com/openapi/dpf-it-com-workspaces-api-openapi.yml
consequence_counts:
  physical: 1
  read: 8
  safety-critical: 4
  write: 23
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 4
kind: agentic-access
layout: agentic-access
method: generated
name: Dpf It Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /auth/notification-preferences
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /auth/request-password-reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /auth/reset-password
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /oauth/clients/revoke
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /auth/resend-otp
operation_count: 36
overview: 'DPF exposes 36 API operations that an AI agent could call, of which 28 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 23 write, 1 physical, and 4 safety-critical.


  4 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: DPF
provider_slug: dpf-it-com
slug: dpf-it-com-agentic-access
source_filename: dpf-it-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: generated\nsource: openapi/dpf-it-com-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 36\n  by_action_class:\n    acting: 28\n    connected: 8\n  by_consequence:\n    write: 23\n    physical: 1\n    safety-critical: 4\n    read: 8\n  human_in_the_loop_required: 4\noperations:\n- path: /auth/register\n  method: post\n  operationId: registerUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/verify-otp\n  method: post\n  operationId: verifyOtp\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/resend-otp\n  method: post\n  operationId: resendOtp\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/login\n  method: post\n  operationId: loginUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /auth/refresh\n  method: post\n  operationId: refreshToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/request-password-reset\n  method: post\n  operationId: requestPasswordReset\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /auth/reset-password\n  method: post\n  operationId: resetPassword\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n \
  \     purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /auth/settings\n  method: get\n  operationId: getSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/settings\n  method: put\n  operationId: updateSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/notification-preferences\n  method: get\n  operationId: listNotificationPreferences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/notification-preferences\n  method: put\n  operationId:\
  \ setNotificationPreference\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/notification-preferences\n  method: delete\n  operationId: deleteNotificationPreference\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /auth/billing\n  method: post\n  operationId: billing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces\n  method: post\n  operationId: manageWorkspaces\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connections\n  method: post\n  operationId: manageConnections\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /job-triggers\n  method: post\n  operationId: manageJobTriggers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data-specs\n  method: post\n  operationId: manageDataSpecs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iceberg/v1/config\n  method: get\n  operationId: icebergRestCatalogConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/authorize\n  method: get\n  operationId: oauthAuthorizeGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/authorize\n  method: post\n  operationId: oauthAuthorizePost\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/token\n  method: post\n  operationId: oauthToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/register\n  method: post\n  operationId: oauthRegister\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/clients\n  method: post\n  operationId: oauthCreateClient\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/clients\n  method: get\n  operationId: oauthListClients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/clients/revoke\n  method: post\n  operationId: oauthRevokeClient\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /mcp\n  method: post\n  operationId: mcpRemote\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iceberg/v1/namespaces\n  method: get\n  operationId: icebergListNamespaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iceberg/v1/namespaces\n  method: post\n  operationId: icebergCreateNamespace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iceberg/v1/namespaces/{namespace}/tables\n  method: get\n  operationId: icebergListTables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /iceberg/v1/namespaces/{namespace}/tables\n  method: post\n  operationId: icebergCreateTable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iceberg/v1/namespaces/{namespace}/tables/{table}\n  method: get\n  operationId: icebergLoadTable\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iceberg/v1/namespaces/{namespace}/tables/{table}\n  method: post\n  operationId: icebergUpdateTable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n     \
  \ triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iceberg/v1/namespaces/{namespace}/tables/{table}\n  method: delete\n  operationId: icebergDropTable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /query\n  method: post\n  operationId: executeQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /query-large\n  method: post\n  operationId: executeQueryLarge\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n    \
  \  max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contact\n  method: post\n  operationId: submitContactForm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/dpf-it-com/agentic-access/dpf-it-com-agentic-access.yml
summary_line: 36 operations · 28 acting · 4 human-in-the-loop
tags:
- Data
- Artificial Intelligence
- ETL
- Apache Iceberg
- Platform
- Company
---
