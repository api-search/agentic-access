---
acting_count: 33
action_class_counts:
  acting: 33
  connected: 32
api_specs:
- filename: 4k-garden-auth-controller-api-openapi.yml
  format: yaml
  label: 4K Garden Auth Controller API
  slug: 4k-garden-auth-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/4k-garden/refs/heads/main/openapi/4k-garden-auth-controller-api-openapi.yml
- filename: 4k-garden-customer-controller-api-openapi.yml
  format: yaml
  label: 4K Garden Customer Controller API
  slug: 4k-garden-customer-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/4k-garden/refs/heads/main/openapi/4k-garden-customer-controller-api-openapi.yml
- filename: 4k-garden-enterprise-controller-api-openapi.yml
  format: yaml
  label: 4K Garden Enterprise Controller API
  slug: 4k-garden-enterprise-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/4k-garden/refs/heads/main/openapi/4k-garden-enterprise-controller-api-openapi.yml
- filename: 4k-garden-frontend-controller-api-openapi.yml
  format: yaml
  label: 4K Garden Frontend Controller API
  slug: 4k-garden-frontend-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/4k-garden/refs/heads/main/openapi/4k-garden-frontend-controller-api-openapi.yml
- filename: 4k-garden-tvc-controller-api-openapi.yml
  format: yaml
  label: 4K Garden Tvc Controller API
  slug: 4k-garden-tvc-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/4k-garden/refs/heads/main/openapi/4k-garden-tvc-controller-api-openapi.yml
consequence_counts:
  read: 32
  safety-critical: 33
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 33
kind: agentic-access
layout: agentic-access
method: generated
name: 4K Garden Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/auth/login
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/auth/login-sms
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/auth/register
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/auth/reset-password
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/auth/sms-code
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/auth/verificationCode
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/auth/verificationCode
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/auth/verificationCode
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/auth/verificationCode
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/enterprise/invitations/{invitationId}/accept
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/enterprise/invitations/{invitationId}/reject
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/enterprise/upgrade
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/enterprise/{enterpriseId}/invite
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/enterprise/{enterpriseId}/members/{memberUserId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/enterprise/{enterpriseId}/members/{memberUserId}/level
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/tvc/task/cancel
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/tvc/task/confirm
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/tvc/task/create
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/tvc/task/create-cinema
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/tvc/task/detail
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/tvc/task/revise
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/tvc/workspace
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/user/bindSaler
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/user/download/create
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/user/password
operation_count: 65
overview: '4K Garden exposes 65 API operations that an AI agent could call, of which 33 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 32 read and 33 safety-critical.


  33 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: 4K Garden
provider_slug: 4k-garden
slug: 4k-garden-agentic-access
source_filename: 4k-garden-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: generated\nsource: openapi/4k-garden-auth-controller-api-openapi.yml, openapi/4k-garden-customer-controller-api-openapi.yml,\n  openapi/4k-garden-enterprise-controller-api-openapi.yml, openapi/4k-garden-frontend-controller-api-openapi.yml,\n  openapi/4k-garden-tvc-controller-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 65\n  by_action_class:\n    connected: 32\n    acting: 33\n  by_consequence:\n    read: 32\n    safety-critical: 33\n  human_in_the_loop_required: 33\noperations:\n- path: /api/auth/health\n  method: get\n  operationId: healthUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/auth/login\n  method: post\n  operationId: loginUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/auth/login-sms\n  method: post\n  operationId: loginSmsUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/auth/me\n  method: get\n  operationId: meUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/auth/register\n\
  \  method: post\n  operationId: registerUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/auth/register-config\n  method: get\n  operationId: registerConfigUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/auth/reset-password\n  method: post\n  operationId: resetPasswordUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n\
  - path: /api/auth/sms-code\n  method: post\n  operationId: sendCodeUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/auth/verificationCode\n  method: get\n  operationId: verificationCodeUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/auth/verificationCode\n  method: put\n  operationId: verificationCodeUsingPUT\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /api/auth/verificationCode\n  method: post\n  operationId: verificationCodeUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/auth/verificationCode\n  method: delete\n  operationId: verificationCodeUsingDELETE\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/auth/verificationCode\n  method: options\n  operationId: verificationCodeUsingOPTIONS\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/auth/verificationCode\n  method: head\n  operationId: verificationCodeUsingHEAD\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/auth/verificationCode\n  method: patch\n  operationId: verificationCodeUsingPATCH\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/user/balance\n  method: get\n  operationId: getBalanceUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/user/bindSaler\n\
  \  method: post\n  operationId: bindSalerUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/user/consumption\n  method: get\n  operationId: getConsumptionUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/user/credit-packages\n  method: get\n  operationId: listCreditPackagesUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/user/credit-rules\n  method: get\n  operationId: getCreditRulesUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/user/download/create\n  method: post\n  operationId: createDownloadUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/user/download/get\n  method: post\n  operationId: getDownloadUsingPOST\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/user/enterprise-plans\n  method: get\n  operationId: listEnterprisePlansUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/user/member-plans\n  method: get\n  operationId:\
  \ listMemberPlansUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/user/orders\n  method: get\n  operationId: listTasksUsingGET_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/user/password\n  method: put\n  operationId: changePasswordUsingPUT\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/user/phone\n  method: put\n  operationId: changePhoneUsingPUT\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/user/productList\n  method: get\n  operationId: productListUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/user/profile\n  method: put\n  operationId: updateProfileUsingPUT\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/user/stats\n  method: get\n  operationId: getCustomerStatsUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/user/tasks\n  method: get\n  operationId: listTasksUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/user/tasks\n  method: post\n  operationId: createTaskUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/user/tasks/appeal\n  method: post\n  operationId: appealTaskUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /api/user/tasks/upload\n  method: post\n  operationId: createTaskUploadUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/user/tasks/uploadTest\n  method: post\n  operationId: createTaskUploadTestUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/user/tasks/{taskId}\n  method: get\n  operationId: getTaskUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/user/tasks/{taskId}/cancel\n  method: post\n  operationId: cancelTaskUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/user/tasks/{taskId}/retry\n  method: post\n  operationId: retryTaskUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/enterprise/invitations/{invitationId}/accept\n  method: post\n  operationId: acceptInvitationUsingPOST\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/enterprise/invitations/{invitationId}/reject\n  method: post\n  operationId: rejectInvitationUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/enterprise/my\n  method: get\n  operationId: getMyEnterpriseUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/enterprise/upgrade\n\
  \  method: post\n  operationId: upgradeToEnterpriseUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/enterprise/{enterpriseId}/invite\n  method: post\n  operationId: inviteMemberUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/enterprise/{enterpriseId}/members\n  method: get\n  operationId: listMembersUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /api/enterprise/{enterpriseId}/members/{memberUserId}\n  method: delete\n  operationId: removeMemberUsingDELETE\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/enterprise/{enterpriseId}/members/{memberUserId}/level\n  method: put\n  operationId: changeMemberLevelUsingPUT\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/enterprise/{enterpriseId}/stats\n  method: get\n  operationId: enterpriseStatsUsingGET\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/\n  method: get\n  operationId: indexUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/*.html\n  method: get\n  operationId: htmlSuffixUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/css/**\n  method: get\n  operationId: cssFilesUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/dashboard\n  method: get\n  operationId: cleanUrlUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/enterprise\n  method: get\n  operationId: cleanUrlUsingGET_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/images/**\n  method: get\n  operationId: imageFilesUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/js/**\n  method: get\n  operationId: jsFilesUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/landing\n  method: get\n  operationId: cleanUrlUsingGET_2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/login\n  method: get\n  operationId: cleanUrlUsingGET_3\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/{filename}\n  method: get\n  operationId: rootStaticFileUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tvc/task/cancel\n  method: post\n  operationId: cancelTaskUsingPOST_1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/tvc/task/confirm\n  method: post\n  operationId: confirmTaskUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n   \
  \   proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/tvc/task/create\n  method: post\n  operationId: createTaskUsingPOST_1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/tvc/task/create-cinema\n  method: post\n  operationId: createCinemaTaskUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/tvc/task/detail\n  method: post\n  operationId: taskDetailUsingPOST\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/tvc/task/list\n  method: post\n  operationId: listTasksUsingPOST\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tvc/task/revise\n  method: post\n  operationId: reviseTaskUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/tvc/workspace\n  method: post\n  operationId: workspaceUsingPOST\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/4k-garden/refs/heads/main/agentic-access/4k-garden-agentic-access.yml
summary_line: 65 operations · 33 acting · 33 human-in-the-loop
tags:
- Company
- Video
- Ultra High Definition
- Media and Entertainment
- Content Distribution
- Live Streaming
- Artificial Intelligence
- Video Super Resolution
- Virtual Reality
- China
---
