---
acting_count: 24
action_class_counts:
  acting: 24
  connected: 5
api_specs:
- filename: 1kosmos-access-code-api-openapi.yml
  format: yaml
  label: 1Kosmos Access Code API
  slug: 1kosmos-access-code-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1kosmos/refs/heads/main/openapi/1kosmos-access-code-api-openapi.yml
- filename: 1kosmos-ial-api-openapi.yml
  format: yaml
  label: 1Kosmos IAL API
  slug: 1kosmos-ial-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1kosmos/refs/heads/main/openapi/1kosmos-ial-api-openapi.yml
- filename: 1kosmos-ial2-api-openapi.yml
  format: yaml
  label: 1Kosmos IAL2 API
  slug: 1kosmos-ial2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1kosmos/refs/heads/main/openapi/1kosmos-ial2-api-openapi.yml
- filename: 1kosmos-id-verification-api-openapi.yml
  format: yaml
  label: 1Kosmos ID Verification API
  slug: 1kosmos-id-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1kosmos/refs/heads/main/openapi/1kosmos-id-verification-api-openapi.yml
- filename: 1kosmos-otp-api-openapi.yml
  format: yaml
  label: 1Kosmos OTP API
  slug: 1kosmos-otp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1kosmos/refs/heads/main/openapi/1kosmos-otp-api-openapi.yml
- filename: 1kosmos-reports-api-openapi.yml
  format: yaml
  label: 1Kosmos Reports API
  slug: 1kosmos-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1kosmos/refs/heads/main/openapi/1kosmos-reports-api-openapi.yml
- filename: 1kosmos-set-up-api-openapi.yml
  format: yaml
  label: 1Kosmos Set up API
  slug: 1kosmos-set-up-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1kosmos/refs/heads/main/openapi/1kosmos-set-up-api-openapi.yml
- filename: 1kosmos-user-management-api-openapi.yml
  format: yaml
  label: 1Kosmos User Management API
  slug: 1kosmos-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1kosmos/refs/heads/main/openapi/1kosmos-user-management-api-openapi.yml
- filename: 1kosmos-verifiable-credentials-api-openapi.yml
  format: yaml
  label: 1Kosmos Verifiable Credentials API
  slug: 1kosmos-verifiable-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1kosmos/refs/heads/main/openapi/1kosmos-verifiable-credentials-api-openapi.yml
- filename: 1kosmos-workflow-api-api-openapi.yml
  format: yaml
  label: 1Kosmos Workflow API API
  slug: 1kosmos-workflow-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1kosmos/refs/heads/main/openapi/1kosmos-workflow-api-api-openapi.yml
consequence_counts:
  read: 5
  write: 24
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: 1Kosmos Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 29
overview: '1Kosmos exposes 29 API operations that an AI agent could call, of which 24 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 24 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: 1Kosmos
provider_slug: 1kosmos
slug: 1kosmos-agentic-access
source_filename: 1kosmos-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: generated\nsource: openapi/1kosmos-blockid-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 29\n  by_action_class:\n    acting: 24\n    connected: 5\n  by_consequence:\n    write: 24\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /api/r1/system/community_info/fetch\n  method: post\n  operationId: setUpGetTenantCommunityInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /caas/sd\n  method: get\n  operationId: setUpFetchSD\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /document_share_session/create\n  method: post\n  operationId: idVerificationCreateIDVerificationSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/document_share_session/result\n  method: post\n  operationId: idVerificationPollIDVerificationSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/r1/community/{communityName}/userid/{userId}/ial\n  method: get\n  operationId:\
  \ ialFetchIALOfAUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/tenant/{tenantID}/community/{communityID}/events\n  method: post\n  operationId: reportsEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reports/tenant/{tenantID}/community/{communityID}/metrics\n  method: post\n  operationId: reportsMetrics\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reports/tenant/{tenantID}/community/{communityID}/application_usage_report\n\
  \  method: post\n  operationId: reportsApplicationUsageReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reports/tenant/{tenantID}/community/{communityID}/audit_log\n  method: post\n  operationId: reportsAuditLogReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reports/tenant/{tenantID}/community/{communityID}/last_seen_report\n  method: post\n  operationId: reportsLastSeenReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reports/tenant/{tenantID}/community/{communityID}/login_activity_report\n  method: post\n  operationId: reportsLoginActivityReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reports/tenant/{tenantID}/community/{communityID}/passwordless_login_activity_report\n  method: post\n  operationId: reportsPasswordlessLoginActivityReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /api/r2/otp/generate\n  method: post\n  operationId: otpGenerateOTPSMS\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/r2/otp/verify\n  method: post\n  operationId: otpVerifyOTPR2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/r3/otp/verify\n  method: post\n  operationId: otpVerifyOTPR3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n  \
  \    triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users-mgmt/tenant/{tenantId}/community/{communityId}/users/create\n  method: put\n  operationId: userManagementCreateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users-mgmt/tenant/{tenantId}/community/{communityId}/users/fetch\n  method: post\n  operationId: userManagementFetchUserDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users-mgmt/tenant/{tenantId}/community/{communityId}/user_properties/update\n  method: post\n\
  \  operationId: userManagementUpdateUsernameAsAlias\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/r2/acr/community/{community}/code\n  method: put\n  operationId: accessCodeCreateAccessCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/r1/acr/community/{community}/{code}/redeem\n  method: post\n  operationId: accessCodeRedeemAccessCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vcs/tenant/{tenantID}/community/{communityID}/vc/from/payload/{vcType}\n  method: post\n  operationId: verifiableCredentialsCreateVerifiableCredentialFromPayload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vcs/tenant/{tenantID}/community/{communityID}/vc/{vcID}/status\n  method: get\n  operationId: verifiableCredentialsGetVerifiableCredentialStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vcs/tenant/{tenantID}/community/{communityID}/vc/verify\n  method: post\n  operationId: verifiableCredentialsVerifyVerifiableCredential\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vcs/tenant/{tenantID}/community/{communityID}/vp/create\n  method: post\n  operationId: verifiableCredentialsIssueVerifiablePresentation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vcs/tenant/{tenantID}/community/{communityID}/vp/verify\n  method: post\n  operationId: verifiableCredentialsVerifyVerifiablePresentation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /idproofingapi/workflow/workflow_instance/create\n  method: post\n  operationId: ial2CreateWorkflow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /idproofingapi/workflow/workflow_instance/{instanceId}/result_summary\n  method: get\n  operationId: ial2ResultSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workflowapi/workflow_instance/tenant/{tenantId}/community/{communityId}/create\n  method: post\n  operationId: workflowAPICreateWorkflowInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workflowapi/workflow_instance/{wfInstanceId}/tenant/{tenantId}/community/{communityId}/node/{nodeId}\n  method: get\n  operationId: workflowAPINodeResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1kosmos/refs/heads/main/agentic-access/1kosmos-agentic-access.yml
summary_line: 29 operations · 24 acting
tags:
- Identity
- Authentication
- Identity Verification
- Passwordless
- Biometrics
- Verifiable Credentials
- FIDO2
- Security
- Company
---
