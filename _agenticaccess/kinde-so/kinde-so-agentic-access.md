---
acting_count: 111
action_class_counts:
  acting: 111
  connected: 64
api_specs:
- filename: kinde-so-openapi.yml
  format: yaml
  label: Kinde Users API
  slug: kinde-so-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinde-so/refs/heads/main/openapi/kinde-so-openapi.yml
- filename: kinde-so-openapi.yml
  format: yaml
  label: Kinde Organizations API
  slug: kinde-so-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinde-so/refs/heads/main/openapi/kinde-so-openapi.yml
- filename: kinde-so-openapi.yml
  format: yaml
  label: Kinde Roles API
  slug: kinde-so-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinde-so/refs/heads/main/openapi/kinde-so-openapi.yml
- filename: kinde-so-openapi.yml
  format: yaml
  label: Kinde Permissions API
  slug: kinde-so-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinde-so/refs/heads/main/openapi/kinde-so-openapi.yml
- filename: kinde-so-openapi.yml
  format: yaml
  label: Kinde Feature Flags API
  slug: kinde-so-feature-flags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinde-so/refs/heads/main/openapi/kinde-so-openapi.yml
- filename: kinde-so-openapi.yml
  format: yaml
  label: Kinde Applications API
  slug: kinde-so-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinde-so/refs/heads/main/openapi/kinde-so-openapi.yml
- filename: kinde-so-openapi.yml
  format: yaml
  label: Kinde Connections API
  slug: kinde-so-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinde-so/refs/heads/main/openapi/kinde-so-openapi.yml
- filename: kinde-so-openapi.yml
  format: yaml
  label: Kinde APIs and Scopes API
  slug: kinde-so-apis-scopes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinde-so/refs/heads/main/openapi/kinde-so-openapi.yml
- filename: kinde-so-openapi.yml
  format: yaml
  label: Kinde Subscribers API
  slug: kinde-so-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinde-so/refs/heads/main/openapi/kinde-so-openapi.yml
- filename: kinde-so-openapi.yml
  format: yaml
  label: Kinde Business API
  slug: kinde-so-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinde-so/refs/heads/main/openapi/kinde-so-openapi.yml
- filename: kinde-so-openapi.yml
  format: yaml
  label: Kinde Properties API
  slug: kinde-so-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinde-so/refs/heads/main/openapi/kinde-so-openapi.yml
- filename: kinde-so-openapi.yml
  format: yaml
  label: Kinde Webhooks API
  slug: kinde-so-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinde-so/refs/heads/main/openapi/kinde-so-openapi.yml
- filename: kinde-so-openapi.yml
  format: yaml
  label: Kinde Billing API
  slug: kinde-so-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kinde-so/refs/heads/main/openapi/kinde-so-openapi.yml
consequence_counts:
  read: 64
  safety-critical: 12
  write: 99
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 12
kind: agentic-access
layout: agentic-access
method: generated
name: Kinde So Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/connected_apps/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/environment/feature_flags
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/v1/environment/feature_flags/{feature_flag_key}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/environment/feature_flags/{feature_flag_key}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/organizations/{org_code}/feature_flags
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/v1/organizations/{org_code}/feature_flags/{feature_flag_key}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/organizations/{org_code}/feature_flags/{feature_flag_key}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/organizations/{org_code}/users/{user_id}/mfa
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/organizations/{org_code}/users/{user_id}/mfa/{factor_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/v1/users/{user_id}/feature_flags/{feature_flag_key}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/users/{user_id}/mfa
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/users/{user_id}/mfa/{factor_id}
operation_count: 175
overview: 'Kinde exposes 175 API operations that an AI agent could call, of which 111 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 64 read, 99 write, and 12 safety-critical.


  12 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Kinde
provider_slug: kinde-so
slug: kinde-so-agentic-access
source_filename: kinde-so-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/kinde-so-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 175\n  by_action_class:\n    connected: 64\n    acting: 111\n  by_consequence:\n    read: 64\n    write: 99\n    safety-critical: 12\n  human_in_the_loop_required: 12\noperations:\n- path: /api/v1/api_keys\n  method: get\n  operationId: getApiKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/api_keys\n  method: post\n  operationId: createApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/api_keys/{key_id}\n  method: get\n  operationId: getApiKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/api_keys/{key_id}\n  method: put\n  operationId: rotateApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/api_keys/{key_id}\n  method: delete\n  operationId: deleteApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /api/v1/api_keys/verify\n  method: post\n  operationId: verifyApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/apis\n  method: get\n  operationId: getAPIs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/apis\n  method: post\n  operationId: addAPIs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/apis/{api_id}\n  method: get\n\
  \  operationId: getAPI\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/apis/{api_id}\n  method: delete\n  operationId: deleteAPI\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/apis/{api_id}/scopes\n  method: get\n  operationId: getAPIScopes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/apis/{api_id}/scopes\n  method: post\n  operationId: addAPIScope\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n    \
  \  human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/apis/{api_id}/scopes/{scope_id}\n  method: get\n  operationId: getAPIScope\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/apis/{api_id}/scopes/{scope_id}\n  method: patch\n  operationId: updateAPIScope\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/apis/{api_id}/scopes/{scope_id}\n  method: delete\n  operationId: deleteAPIScope\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/apis/{api_id}/applications\n  method: patch\n  operationId: updateAPIApplications\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/apis/{api_id}/applications/{application_id}/scopes/{scope_id}\n  method: post\n  operationId: addAPIApplicationScope\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/apis/{api_id}/applications/{application_id}/scopes/{scope_id}\n  method: delete\n  operationId: deleteAPIApplicationScope\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/applications\n  method: get\n  operationId: getApplications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/applications\n  method: post\n  operationId: createApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/applications/{application_id}\n  method: get\n  operationId: getApplication\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/applications/{application_id}\n  method: patch\n  operationId: updateApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/applications/{application_id}\n  method: delete\n  operationId: deleteApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/applications/{application_id}/connections\n  method: get\n  operationId: GetApplicationConnections\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/applications/{application_id}/connections/{connection_id}\n  method: post\n  operationId: EnableConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/applications/{application_id}/connections/{connection_id}\n  method: delete\n  operationId: RemoveConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/applications/{application_id}/properties\n  method: get\n  operationId:\
  \ getApplicationPropertyValues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/applications/{application_id}/properties/{property_key}\n  method: put\n  operationId: updateApplicationsProperty\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/applications/{application_id}/tokens\n  method: patch\n  operationId: updateApplicationTokens\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/billing/entitlements\n\
  \  method: get\n  operationId: getBillingEntitlements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/billing/agreements\n  method: get\n  operationId: getBillingAgreements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/billing/agreements\n  method: post\n  operationId: createBillingAgreement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/billing/meter_usage\n  method: post\n  operationId: createMeterUsageRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/business\n  method: get\n  operationId: getBusiness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/business\n  method: patch\n  operationId: updateBusiness\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/industries\n  method: get\n  operationId: getIndustries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/timezones\n  method: get\n \
  \ operationId: getTimezones\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/applications/{app_id}/auth_redirect_urls\n  method: get\n  operationId: getCallbackURLs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/applications/{app_id}/auth_redirect_urls\n  method: post\n  operationId: addRedirectCallbackURLs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/applications/{app_id}/auth_redirect_urls\n  method: put\n  operationId: replaceRedirectCallbackURLs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/applications/{app_id}/auth_redirect_urls\n  method: delete\n  operationId: deleteCallbackURLs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/applications/{app_id}/auth_logout_urls\n  method: get\n  operationId: getLogoutURLs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/applications/{app_id}/auth_logout_urls\n  method: post\n  operationId: addLogoutRedirectURLs\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/applications/{app_id}/auth_logout_urls\n  method: put\n  operationId: replaceLogoutRedirectURLs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/applications/{app_id}/auth_logout_urls\n  method: delete\n  operationId: deleteLogoutURLs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/v1/connected_apps/auth_url\n  method: get\n  operationId: GetConnectedAppAuthUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/connected_apps/token\n  method: get\n  operationId: GetConnectedAppToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/connected_apps/revoke\n  method: post\n  operationId: RevokeConnectedAppToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/connections\n  method: get\n  operationId: GetConnections\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/connections\n  method: post\n  operationId: CreateConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/connections/{connection_id}\n  method: get\n  operationId: GetConnection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/connections/{connection_id}\n  method: put\n  operationId: ReplaceConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n    \
  \  triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/connections/{connection_id}\n  method: patch\n  operationId: UpdateConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/connections/{connection_id}\n  method: delete\n  operationId: deleteConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/directories\n  method: get\n  operationId: getDirectories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/v1/directories\n  method: post\n  operationId: createDirectory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/directories/{directory_id}\n  method: get\n  operationId: getDirectory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/directories/{directory_id}\n  method: patch\n  operationId: updateDirectory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /api/v1/directories/{directory_id}\n  method: delete\n  operationId: deleteDirectory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/environment\n  method: get\n  operationId: getEnvironment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/environment/feature_flags\n  method: get\n  operationId: GetEnvironementFeatureFlags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/environment/feature_flags\n  method: delete\n  operationId: DeleteEnvironementFeatureFlagOverrides\n  x-agentic-access:\n    action-class: acting\n  \
  \  consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/environment/feature_flags/{feature_flag_key}\n  method: patch\n  operationId: UpdateEnvironementFeatureFlagOverride\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/environment/feature_flags/{feature_flag_key}\n  method: delete\n  operationId: DeleteEnvironementFeatureFlagOverride\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n\
  \      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/environment/logos\n  method: get\n  operationId: ReadLogo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/environment/logos/{type}\n  method: put\n  operationId: AddLogo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/environment/logos/{type}\n  method: delete\n  operationId: DeleteLogo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/environment_variables\n  method: get\n  operationId: getEnvironmentVariables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/environment_variables\n  method: post\n  operationId: createEnvironmentVariable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/environment_variables/{variable_id}\n  method: get\n  operationId: getEnvironmentVariable\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/environment_variables/{variable_id}\n\
  \  method: patch\n  operationId: updateEnvironmentVariable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/environment_variables/{variable_id}\n  method: delete\n  operationId: deleteEnvironmentVariable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/feature_flags\n  method: post\n  operationId: CreateFeatureFlag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/feature_flags/{feature_flag_key}\n  method: put\n  operationId: UpdateFeatureFlag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/feature_flags/{feature_flag_key}\n  method: delete\n  operationId: DeleteFeatureFlag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/identities/{identity_id}\n  method: get\n  operationId: GetIdentity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/identities/{identity_id}\n  method: patch\n  operationId: UpdateIdentity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/identities/{identity_id}\n  method: delete\n  operationId: DeleteIdentity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/organization/{org_code}/invites\n  method: get\n  operationId: getOrganizationInvites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/organization/{org_code}/invites\n  method: post\n  operationId: createOrganizationInvite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/organization/{org_code}/invites/{invite_code}\n  method: get\n  operationId: getOrganizationInvite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/organization/{org_code}/invites/{invite_code}\n  method: delete\n  operationId: deleteOrganizationInvite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/mfa\n  method: put\n  operationId: ReplaceMFA\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/organization\n  method: get\n  operationId: getOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/organization\n  method: post\n  operationId: createOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /api/v1/organizations\n  method: get\n  operationId: getOrganizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/organization/{org_code}\n  method: patch\n  operationId: updateOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/organization/{org_code}\n  method: delete\n  operationId: deleteOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/organizations/{org_code}/users\n\
  \  method: get\n  operationId: GetOrganizationUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/organizations/{org_code}/users\n  method: post\n  operationId: AddOrganizationUsers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/organizations/{org_code}/users\n  method: patch\n  operationId: UpdateOrganizationUsers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/organizations/{org_code}/users/{user_id}/roles\n\
  \  method: get\n  operationId: GetOrganizationUserRoles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/organizations/{org_code}/users/{user_id}/roles\n  method: post\n  operationId: CreateOrganizationUserRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/organizations/{org_code}/users/{user_id}/roles/{role_id}\n  method: delete\n  operationId: DeleteOrganizationUserRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /api/v1/organizations/{org_code}/roles/{role_id}/users\n  method: get\n  operationId: GetOrganizationRoleUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/organizations/{org_code}/users/{user_id}/permissions\n  method: get\n  operationId: GetOrganizationUserPermissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/organizations/{org_code}/users/{user_id}/permissions\n  method: post\n  operationId: CreateOrganizationUserPermission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/organizations/{org_code}/users/{user_id}/permissions/{permission_id}\n\
  \  method: delete\n  operationId: DeleteOrganizationUserPermission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/organizations/{org_code}/users/{user_id}\n  method: delete\n  operationId: RemoveOrganizationUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/organizations/{org_code}/users/{user_id}/apis/{api_id}/scopes/{scope_id}\n  method: post\n  operationId: addOrganizationUserAPIScope\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/organizations/{org_code}/users/{user_id}/apis/{api_id}/scopes/{scope_id}\n  method: delete\n  operationId: deleteOrganizationUserAPIScope\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/organizations/{org_code}/users/{user_id}/mfa\n  method: get\n  operationId: GetOrgUserMFA\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/organizations/{org_code}/users/{user_id}/mfa\n  method: delete\n  operationId: ResetOrgUserMFAAll\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: saf\n\n# --- truncated at 32 KB (54 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/kinde-so/refs/heads/main/agentic-access/kinde-so-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kinde-so/refs/heads/main/agentic-access/kinde-so-agentic-access.yml
summary_line: 175 operations · 111 acting · 12 human-in-the-loop
tags:
- Authentication
- User Management
- Identity
- Authorization
- SaaS
- CIAM
---
