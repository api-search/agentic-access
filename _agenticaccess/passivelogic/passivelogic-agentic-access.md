---
acting_count: 92
action_class_counts:
  acting: 92
  connected: 105
api_specs:
- filename: passivelogic-account-api-openapi.yml
  format: yaml
  label: PassiveLogic Account API
  slug: passivelogic-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-account-api-openapi.yml
- filename: passivelogic-api-api-openapi.yml
  format: yaml
  label: PassiveLogic API
  slug: passivelogic-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-api-api-openapi.yml
- filename: passivelogic-app-api-openapi.yml
  format: yaml
  label: PassiveLogic App API
  slug: passivelogic-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-app-api-openapi.yml
- filename: passivelogic-auth-groups-api-openapi.yml
  format: yaml
  label: PassiveLogic Auth Groups API
  slug: passivelogic-auth-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-auth-groups-api-openapi.yml
- filename: passivelogic-authentication-api-openapi.yml
  format: yaml
  label: PassiveLogic Authentication API
  slug: passivelogic-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-authentication-api-openapi.yml
- filename: passivelogic-bindings-api-openapi.yml
  format: yaml
  label: PassiveLogic Bindings API
  slug: passivelogic-bindings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-bindings-api-openapi.yml
- filename: passivelogic-default-api-openapi.yml
  format: yaml
  label: PassiveLogic Default API
  slug: passivelogic-default-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-default-api-openapi.yml
- filename: passivelogic-export-api-openapi.yml
  format: yaml
  label: PassiveLogic Export API
  slug: passivelogic-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-export-api-openapi.yml
- filename: passivelogic-graphql-api-openapi.yml
  format: yaml
  label: PassiveLogic Graph QL API
  slug: passivelogic-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-graphql-api-openapi.yml
- filename: passivelogic-health-api-openapi.yml
  format: yaml
  label: PassiveLogic Health API
  slug: passivelogic-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-health-api-openapi.yml
- filename: passivelogic-images-api-openapi.yml
  format: yaml
  label: PassiveLogic Images API
  slug: passivelogic-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-images-api-openapi.yml
- filename: passivelogic-organization-api-openapi.yml
  format: yaml
  label: PassiveLogic Organization API
  slug: passivelogic-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-organization-api-openapi.yml
- filename: passivelogic-passivelogic-device-api-openapi.yml
  format: yaml
  label: PassiveLogic PassiveLogic Device API
  slug: passivelogic-passivelogic-device-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-passivelogic-device-api-openapi.yml
- filename: passivelogic-quantum-sync-api-openapi.yml
  format: yaml
  label: PassiveLogic Quantum Sync API
  slug: passivelogic-quantum-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-quantum-sync-api-openapi.yml
- filename: passivelogic-site-api-openapi.yml
  format: yaml
  label: PassiveLogic Site API
  slug: passivelogic-site-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-site-api-openapi.yml
- filename: passivelogic-tunnel-api-openapi.yml
  format: yaml
  label: PassiveLogic Tunnel API
  slug: passivelogic-tunnel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-tunnel-api-openapi.yml
- filename: passivelogic-utility-api-openapi.yml
  format: yaml
  label: PassiveLogic Utility API
  slug: passivelogic-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-utility-api-openapi.yml
consequence_counts:
  physical: 8
  read: 105
  safety-critical: 6
  write: 78
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 6
kind: agentic-access
layout: agentic-access
method: generated
name: Passivelogic Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/auth/password/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/auth/password/reset/change
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v0.19/auth/password/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v0.19/auth/password/reset/change
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v0.20/auth/password/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v0.20/auth/password/reset/change
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/auth/register/initiate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/authgroup/invite
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/organization/invite
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v0.19/auth/register/initiate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v0.19/organization/invite
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v0.20/auth/register/initiate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v0.20/authgroup/invite
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v0.20/organization/invite
operation_count: 197
overview: 'PassiveLogic exposes 197 API operations that an AI agent could call, of which 92 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 105 read, 78 write, 8 physical, and 6 safety-critical.


  6 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: PassiveLogic
provider_slug: passivelogic
slug: passivelogic-agentic-access
source_filename: passivelogic-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: generated\nsource: openapi/passivelogic-rest-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 197\n  by_action_class:\n    connected: 105\n    acting: 92\n  by_consequence:\n    read: 105\n    write: 78\n    safety-critical: 6\n    physical: 8\n  human_in_the_loop_required: 6\noperations:\n- path: /app/lp/**\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0.20/auth/email/change/verify\n  method: get\n  operationId: getApiV0.20AuthEmailChangeVerify\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /app/qs/**\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0.19/util/externalauthconfig\n  method: get\n  operationId: getApiV0.19UtilExternalauthconfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0.19/util/quantumlens\n  method: post\n  operationId: postApiV0.19UtilQuantumlens\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v0.20/util/externalauthconfig\n  method: get\n  operationId: getApiV0.20UtilExternalauthconfig\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/auth/magic-link-generate\n  method: post\n  operationId: postApiAuthMagic-link-generate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v0.20/authgroup/decline\n  method: post\n  operationId: postApiV0.20AuthgroupDecline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v0.19/auth/email/change/verify\n  method: get\n  operationId: getApiV0.19AuthEmailChangeVerify\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/auth/email/change/verify\n  method: get\n  operationId: getApiAuthEmailChangeVerify\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app/qe/*\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app/login/userAuth\n  method: get\n  operationId: getAppLoginUserAuth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/auth/password/change\n  method: post\n  operationId: postApiAuthPasswordChange\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/password/change\n  method: get\n  operationId: getApiAuthPasswordChange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0.19/util/ping\n  method: get\n  operationId: getApiV0.19UtilPing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/authgroup/remove/{authGroupID}/{userID}\n  method: post\n  operationId: postApiAuthgroupRemoveByAuthGroupIDByUserID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v0.19/auth/password/reset\n\
  \  method: post\n  operationId: postApiV0.19AuthPasswordReset\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /app/login/password\n  method: get\n  operationId: getAppLoginPassword\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app/bs/**\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0.20/util/quantumversion\n  method: get\n  operationId: getApiV0.20UtilQuantumversion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/util/quantumversion\n  method: get\n  operationId: getApiUtilQuantumversion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0.19/quantumsync\n  method: get\n  operationId: getApiV0.19Quantumsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/datasync\n  method: get\n  operationId: getApiDatasync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0.20/auth/login\n  method: get\n  operationId: getApiV0.20AuthLogin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0.19/auth/login\n  method: get\n  operationId: getApiV0.19AuthLogin\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0.20/auth/api-key\n  method: delete\n  operationId: deleteApiV0.20AuthApi-key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /app/login/eula\n  method: get\n  operationId: getAppLoginEula\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/auth/register\n  method: post\n  operationId: postApiAuthRegister\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/login\n  method: get\n  operationId: getApiAuthLogin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app/as/**\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/util/externalauthconfig\n  method: get\n  operationId: getApiUtilExternalauthconfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app/al/**\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0.20/auth/logout\n  method: post\n  operationId: postApiV0.20AuthLogout\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v0.20/device/login\n  method: get\n  operationId: getApiV0.20DeviceLogin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/util/quantumlens\n  method: post\n  operationId: postApiUtilQuantumlens\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v0.19/auth/zendesk\n  method: get\n  operationId: getApiV0.19AuthZendesk\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0.19/auth/verify\n  method: get\n  operationId: getApiV0.19AuthVerify\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/meta.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/util/version\n  method: get\n  operationId: getApiUtilVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/authgroup/decline\n  method: post\n  operationId: postApiAuthgroupDecline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n \
  \     human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/device/login\n  method: get\n  operationId: getApiDeviceLogin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organization/invite\n  method: post\n  operationId: postApiOrganizationInvite\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /app/login/verify\n  method: get\n  operationId: getAppLoginVerify\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/auth/keys\n\
  \  method: get\n  operationId: getApiAuthKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0.19/account/eula/accept\n  method: post\n  operationId: postApiV0.19AccountEulaAccept\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v0.20/organization/delete\n  method: post\n  operationId: postApiV0.20OrganizationDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /app/devtools/*\n  method: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/account/user/delete\n  method: delete\n  operationId: deleteApiAccountUserDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/password/reset\n  method: post\n  operationId: postApiAuthPasswordReset\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/authgroup/invite\n  method: post\n  operationId: postApiAuthgroupInvite\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/image/user-avatar\n  method: post\n  operationId: postApiImageUser-avatar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v0.20/auth/whoami\n  method: get\n  operationId: getApiV0.20AuthWhoami\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0.20/authgroup/join\n  method: post\n  operationId: postApiV0.20AuthgroupJoin\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v0.20/authgroup/join\n  method: get\n  operationId: getApiV0.20AuthgroupJoin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0.19/organization/update-logo\n  method: post\n  operationId: postApiV0.19OrganizationUpdate-logo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/device/tailscale/authToken\n  method: get\n  operationId: getApiDeviceTailscaleAuthToken\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0.20/auth/verify\n  method: get\n  operationId: getApiV0.20AuthVerify\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0.20/image\n  method: post\n  operationId: postApiV0.20Image\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/organization/decline\n  method: post\n  operationId: postApiOrganizationDecline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/magic-link-login\n  method: get\n  operationId: getApiAuthMagic-link-login\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0.19/auth/register\n  method: post\n  operationId: postApiV0.19AuthRegister\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/api-key/generate\n  method: get\n  operationId: getApiAuthApi-keyGenerate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0.19/account/credentials\n  method: get\n  operationId:\
  \ getApiV0.19AccountCredentials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0.20/auth/keys\n  method: get\n  operationId: getApiV0.20AuthKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0.20/device/register\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v0.20/authgroup/remove/{authGroupID}/{userID}\n  method: post\n  operationId: postApiV0.20AuthgroupRemoveByAuthGroupIDByUserID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/organization/update-image\n  method: post\n  operationId: postApiOrganizationUpdate-image\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v0.19/auth/api-key\n  method: delete\n  operationId: deleteApiV0.19AuthApi-key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/password/reset/change\n  method: post\n  operationId: postApiAuthPasswordResetChange\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v0.20/util/version\n  method: get\n  operationId: getApiV0.20UtilVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/auth/offline\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0.19/datasync\n  method: get\n  operationId: getApiV0.19Datasync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/auth/register/initiate\n\
  \  method: post\n  operationId: postApiAuthRegisterInitiate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v0.19/health/liveness\n  method: get\n  operationId: getApiV0.19HealthLiveness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0.19/util/pl-hardware-info\n  method: get\n  operationId: getApiV0.19UtilPl-hardware-info\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0.20/quantumsync\n  method: get\n  operationId: getApiV0.20Quantumsync\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0.19/account/user/delete\n  method: delete\n  operationId: deleteApiV0.19AccountUserDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/verify\n  method: get\n  operationId: getApiAuthVerify\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/account/eula/accept\n  method: post\n  operationId: postApiAccountEulaAccept\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/api-key/remove\n  method: delete\n  operationId: deleteApiAuthApi-keyRemove\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/api-key/remove\n  method: post\n  operationId: postApiAuthApi-keyRemove\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v0.19/auth/logout\n  method: post\n  operationId: postApiV0.19AuthLogout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n \
  \   audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v0.20/auth/register\n  method: post\n  operationId: postApiV0.20AuthRegister\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/device/register\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v0.20/organization/decline\n  method: post\n  operationId: postApiV0.20OrganizationDecline\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/organization/update-logo\n  method: post\n  operationId: postApiOrganizationUpdate-logo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v0.20/account/user/delete\n  method: delete\n  operationId: deleteApiV0.20AccountUserDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n- path: /api/v0.19/auth/offline\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/health/liveness\n  method: get\n  operationId: getApiHealthLiveness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0.19/organization/invite\n  method: post\n  operationId: postApiV0.19OrganizationInvite\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v0.20/auth/magic-link-generate\n  method: post\n  operationId: postApiV0.20AuthMagic-link-generate\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /app/login/reset\n  method: get\n  operationId: getAppLoginReset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0.20/auth/password/change\n  method: post\n  operationId: postApiV0.20AuthPasswordChange\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v0.20/auth/password/change\n  method: get\n  operationId: getApiV0.20AuthPasswordChange\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0.19/graphqlSubscribe\n  method: get\n  operationId: getApiV0.19GraphqlSubscribe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0.20/site/copy\n  method: post\n  operationId: postApiV0.20SiteCopy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v0.20/device/tailscale/authToken\n  method: get\n  operationId: getApiV0.20DeviceTailscaleAuthToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/image\n  method: post\n  operationId:\
  \ postApiImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /app/qc/**\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app/login/signUp\n  method: get\n  operationId: getAppLoginSignUp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0.19/util/quantumversion\n  method: get\n  operationId: getApiV0.19UtilQuantumversion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0.20/tunnel/{serialNumber}/**\n  method: put\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v0.20/tunnel/{serialNumber}/**\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v0.20/tunnel/{serialNumber}/**\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v0.20/tunnel/{serialNumber}/**\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0.20/util/quantumlens\n  method: post\n  operationId: postApiV0.20UtilQuantumlens\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v0.20/image/{imageID}\n  method: delete\n  operationId: deleteApiV0.20ImageByImageID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v0.19/organization/decline\n  method: post\n  operationId: postApiV0.19OrganizationDecline\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v0.20/graphqlSubscribe\n  method: get\n  operationId: getApiV0.20GraphqlSubscribe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app/login/finish\n  method: get\n  operationId: getAppLoginFinish\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/health/readiness\n  method: get\n  operationId: getApiHealthReadiness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/auth/api-key\n\
  \  method: delete\n  operationId: deleteApiAuthApi-key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v0.20/graphql\n  method: post\n  operationId: postApiV0.20Graphql\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v0.20/graphql\n  method: get\n  operationId: getApiV0.20Graphql\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v0.19/auth/keys\n  method: get\n  operationId: getApiV0.19AuthKeys\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n\n\n# --- truncated at 32 KB (55 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/agentic-access/passivelogic-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/agentic-access/passivelogic-agentic-access.yml
summary_line: 197 operations · 92 acting · 6 human-in-the-loop
tags:
- Company
- digital-twin
- building-automation
- hvac
- smart-buildings
- autonomous-systems
- graphql
- Ontology
- iot
- edge-computing
- physical-ai
- Energy
---
