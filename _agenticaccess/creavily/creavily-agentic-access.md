---
acting_count: 155
action_class_counts:
  acting: 155
  connected: 86
api_specs:
- filename: creavily-admin-api-openapi.yml
  format: yaml
  label: Creavily Admin API
  slug: creavily-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creavily/openapi/creavily-admin-api-openapi.yml
- filename: creavily-agent-api-openapi.yml
  format: yaml
  label: Creavily Agent API
  slug: creavily-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creavily/openapi/creavily-agent-api-openapi.yml
- filename: creavily-analytics-api-openapi.yml
  format: yaml
  label: Creavily Analytics API
  slug: creavily-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creavily/openapi/creavily-analytics-api-openapi.yml
- filename: creavily-assets-api-openapi.yml
  format: yaml
  label: Creavily Assets API
  slug: creavily-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creavily/openapi/creavily-assets-api-openapi.yml
- filename: creavily-auth-api-openapi.yml
  format: yaml
  label: Creavily Auth API
  slug: creavily-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creavily/openapi/creavily-auth-api-openapi.yml
- filename: creavily-automations-api-openapi.yml
  format: yaml
  label: Creavily Automations API
  slug: creavily-automations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creavily/openapi/creavily-automations-api-openapi.yml
- filename: creavily-billing-api-openapi.yml
  format: yaml
  label: Creavily Billing API
  slug: creavily-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creavily/openapi/creavily-billing-api-openapi.yml
- filename: creavily-blog-api-openapi.yml
  format: yaml
  label: Creavily Blog API
  slug: creavily-blog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creavily/openapi/creavily-blog-api-openapi.yml
- filename: creavily-brands-api-openapi.yml
  format: yaml
  label: Creavily Brands API
  slug: creavily-brands-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creavily/openapi/creavily-brands-api-openapi.yml
- filename: creavily-bridges-api-openapi.yml
  format: yaml
  label: Creavily Bridges API
  slug: creavily-bridges-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creavily/openapi/creavily-bridges-api-openapi.yml
- filename: creavily-channels-api-openapi.yml
  format: yaml
  label: Creavily Channels API
  slug: creavily-channels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creavily/openapi/creavily-channels-api-openapi.yml
- filename: creavily-developer-api-openapi.yml
  format: yaml
  label: Creavily Developer API
  slug: creavily-developer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creavily/openapi/creavily-developer-api-openapi.yml
- filename: creavily-engagement-api-openapi.yml
  format: yaml
  label: Creavily Engagement API
  slug: creavily-engagement-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creavily/openapi/creavily-engagement-api-openapi.yml
- filename: creavily-inquiries-api-openapi.yml
  format: yaml
  label: Creavily Inquiries API
  slug: creavily-inquiries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creavily/openapi/creavily-inquiries-api-openapi.yml
- filename: creavily-media-api-openapi.yml
  format: yaml
  label: Creavily Media API
  slug: creavily-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creavily/openapi/creavily-media-api-openapi.yml
- filename: creavily-oauth-api-openapi.yml
  format: yaml
  label: Creavily OAuth API
  slug: creavily-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creavily/openapi/creavily-oauth-api-openapi.yml
- filename: creavily-platform-api-openapi.yml
  format: yaml
  label: Creavily Platform API
  slug: creavily-platform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creavily/openapi/creavily-platform-api-openapi.yml
- filename: creavily-provider-tools-api-openapi.yml
  format: yaml
  label: Creavily Provider Tools API
  slug: creavily-provider-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creavily/openapi/creavily-provider-tools-api-openapi.yml
- filename: creavily-publishing-api-openapi.yml
  format: yaml
  label: Creavily Publishing API
  slug: creavily-publishing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creavily/openapi/creavily-publishing-api-openapi.yml
- filename: creavily-system-api-openapi.yml
  format: yaml
  label: Creavily System API
  slug: creavily-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creavily/openapi/creavily-system-api-openapi.yml
- filename: creavily-webhooks-api-openapi.yml
  format: yaml
  label: Creavily Webhooks API
  slug: creavily-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creavily/openapi/creavily-webhooks-api-openapi.yml
consequence_counts:
  physical: 9
  read: 86
  safety-critical: 16
  write: 130
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 16
kind: agentic-access
layout: agentic-access
method: generated
name: Creavily Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/auth/forgot-password
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/auth/logout
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/auth/logout-all
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/auth/reset-password
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/channel-accounts/{channelAccountId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/developer/api-keys/{apiKeyId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/developer/oauth-apps/{oauthAppId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/developer/oauth-authorizations/{authorizationId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/platform/admins/{userId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/platform/billing/promotion-codes/{codeId}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/platform/billing/redeem-codes/{codeId}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/platform/billing/workspaces/{organizationId}/manual-plan
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/platform/switches/{key}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/platform/users/{userId}/mark-email-verified
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/platform/users/{userId}/suspend
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/webhooks/deliveries/queued/enqueue
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/admin/provider-comment-webhooks/provision
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/auth/resend-verification
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/auth/sign-up
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/billing/checkout-sessions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/billing/redeem-code
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/platform/users/{userId}/verification-email
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/public/contact-requests
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/public/social-comment-automation/jobs/{jobId}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/social-comment-automation/jobs/{jobId}/cancel
operation_count: 241
overview: 'Creavily exposes 241 API operations that an AI agent could call, of which 155 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 86 read, 130 write, 9 physical, and 16 safety-critical.


  16 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Creavily
provider_slug: creavily
slug: creavily-agentic-access
source_filename: creavily-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/creavily-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 241\n  by_action_class:\n    connected: 86\n    acting: 155\n  by_consequence:\n    read: 86\n    write: 130\n    physical: 9\n    safety-critical: 16\n  human_in_the_loop_required: 16\noperations:\n- path: /v1/public/publishing-profiles/{profileId}/comment-automation\n  method: get\n  operationId: publicGetCommentReplyAutomationPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public/publishing-profiles/{profileId}/comment-automation\n  method: put\n  operationId: publicSaveCommentReplyAutomationPolicy\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public/publishing-profiles/{profileId}/comment-automation/sync-comments\n  method: post\n  operationId: publicSyncCommentReplyAutomationComments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public/social-comment-automation/jobs\n  method: get\n  operationId: publicListCommentReplyAutomationJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public/social-comment-automation/jobs/{jobId}\n\
  \  method: get\n  operationId: publicGetCommentReplyAutomationJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public/social-comment-automation/jobs/{jobId}/approve\n  method: post\n  operationId: publicApproveCommentReplyAutomationJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public/social-comment-automation/jobs/{jobId}/cancel\n  method: post\n  operationId: publicCancelCommentReplyAutomationJob\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/publishing-profiles/{profileId}/comment-automation\n  method: get\n  operationId: dashboardGetCommentReplyAutomationPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/publishing-profiles/{profileId}/comment-automation\n  method: put\n  operationId: dashboardSaveCommentReplyAutomationPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/publishing-profiles/{profileId}/comment-automation/sync-comments\n  method: post\n  operationId: dashboardSyncCommentReplyAutomationComments\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/social-comment-automation/jobs\n  method: get\n  operationId: dashboardListCommentReplyAutomationJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/social-comment-automation/jobs/{jobId}\n  method: get\n  operationId: dashboardGetCommentReplyAutomationJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/social-comment-automation/jobs/{jobId}/approve\n  method: post\n  operationId: dashboardApproveCommentReplyAutomationJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/social-comment-automation/jobs/{jobId}/cancel\n  method: post\n  operationId: dashboardCancelCommentReplyAutomationJob\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public/social-comment-reply-runs\n  method: post\n  operationId: publicCreateCommentReplyRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/public/social-comment-reply-runs/{runId}\n  method: get\n  operationId: publicGetCommentReplyRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/social-comment-reply-runs\n  method: post\n  operationId: dashboardCreateCommentReplyRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/social-comment-reply-runs/{runId}\n  method: get\n  operationId: dashboardGetCommentReplyRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billing/summary\n  method: get\n  operationId: getWorkspaceBillingSummary\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billing/checkout-sessions\n  method: post\n  operationId: createWorkspaceBillingCheckoutSession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/portal-sessions\n  method: post\n  operationId: createWorkspaceBillingPortalSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/redeem-code\n  method: post\n  operationId: redeemWorkspaceBillingCode\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/platform/billing/redeem-codes\n  method: get\n  operationId: listPlatformRedeemCodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/platform/billing/redeem-codes\n  method: post\n  operationId: addPlatformRedeemCodes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/platform/billing/redeem-codes/replenish\n\
  \  method: post\n  operationId: replenishPlatformRedeemCodes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/platform/billing/redeem-code-pools/{planId}\n  method: patch\n  operationId: updatePlatformRedeemPool\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/platform/billing/redeem-codes/{codeId}/disable\n  method: post\n  operationId: disablePlatformRedeemCode\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/auth/sign-up\n  method: post\n  operationId: signUpWithPassword\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/verify-email\n  method: post\n  operationId: verifyEmailAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/resend-verification\n  method: post\n  operationId:\
  \ resendEmailVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/forgot-password\n  method: post\n  operationId: requestPasswordReset\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/auth/reset-password\n  method: post\n  operationId: resetPasswordWithToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n\
  \      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/auth/set-password\n  method: post\n  operationId: setAccountPassword\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/sign-in-methods\n  method: get\n  operationId: listSignInMethods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/auth/google/link\n  method: post\n  operationId: startGoogleLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/google/link\n  method: delete\n  operationId: unlinkGoogle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/platform/billing/overview\n  method: get\n  operationId: getPlatformBillingOverview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/platform/billing/workspaces\n  method: get\n  operationId: listPlatformBillingWorkspaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/platform/billing/workspaces/{organizationId}\n  method:\
  \ get\n  operationId: getPlatformBillingWorkspace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/platform/billing/workspaces/{organizationId}/manual-plan\n  method: put\n  operationId: grantPlatformManualPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/platform/billing/workspaces/{organizationId}/manual-plan\n  method: patch\n  operationId: updatePlatformManualPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/platform/billing/workspaces/{organizationId}/manual-plan\n  method: delete\n  operationId: revokePlatformManualPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/platform/billing/workspaces/{organizationId}/plan-history\n  method: get\n  operationId: getPlatformPlanHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/platform/billing/promotion-batches\n  method: get\n  operationId: listPlatformPromotionBatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/platform/billing/promotion-batches\n\
  \  method: post\n  operationId: createPlatformPromotionBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/platform/billing/promotion-batches/{batchId}/codes\n  method: get\n  operationId: listPlatformPromotionCodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/platform/billing/promotion-batches/{batchId}/sync\n  method: post\n  operationId: syncPlatformPromotionBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/platform/billing/promotion-codes/{codeId}/disable\n  method: post\n  operationId: disablePlatformPromotionCode\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/platform/admins\n  method: get\n  operationId: listPlatformAdmins\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/platform/admins\n  method: post\n  operationId: grantPlatformAdmin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/platform/admins/{userId}\n  method: delete\n  operationId: revokePlatformAdmin\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/platform/users\n  method: get\n  operationId: listPlatformUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/platform/users/{userId}\n  method: get\n  operationId: getPlatformUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/platform/users/{userId}/suspend\n  method: post\n  operationId: suspendPlatformUser\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/platform/users/{userId}/reactivate\n  method: post\n  operationId: reactivatePlatformUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/platform/users/{userId}/sign-out-everywhere\n  method: post\n  operationId: signOutPlatformUserEverywhere\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n     \
  \ triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/platform/users/{userId}/verification-email\n  method: post\n  operationId: resendPlatformUserVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/platform/users/{userId}/mark-email-verified\n  method: post\n  operationId: markPlatformUserEmailVerified\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/platform/activity\n  method: get\n\
  \  operationId: listPlatformActivity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/platform/activity/sign-ins\n  method: get\n  operationId: listPlatformSignIns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/platform/activity/metrics\n  method: get\n  operationId: getPlatformActivityMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/platform/switches\n  method: get\n  operationId: listPlatformSwitches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/platform/switches/{key}\n  method: put\n  operationId: updatePlatformSwitch\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/platform/blog/posts\n  method: get\n  operationId: listPlatformBlogPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/platform/blog/posts\n  method: post\n  operationId: createPlatformBlogPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/platform/blog/posts/{postId}\n  method: get\n  operationId: getPlatformBlogPost\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/platform/blog/posts/{postId}\n  method: patch\n  operationId: updatePlatformBlogPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/platform/blog/preview\n  method: post\n  operationId: previewPlatformBlogMarkdown\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/platform/blog/posts/{postId}/publish\n  method: post\n  operationId: publishPlatformBlogPost\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/platform/blog/posts/{postId}/unpublish\n  method: post\n  operationId: unpublishPlatformBlogPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/platform/blog/posts/{postId}/archive\n  method: post\n  operationId: archivePlatformBlogPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/platform/blog/posts/{postId}/revisions\n  method: get\n  operationId: listPlatformBlogRevisions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/platform/blog/posts/{postId}/revisions/{revisionNumber}\n  method: get\n  operationId: getPlatformBlogRevision\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public/blog/posts\n  method: get\n  operationId: listBlogPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public/blog/posts\n  method: post\n  operationId: createBlogDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public/blog/posts/{postId}\n  method: get\n  operationId: getBlogPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public/blog/posts/{postId}\n  method: patch\n  operationId: updateBlogDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public/blog/posts/{postId}/preview\n  method: post\n  operationId: previewBlogPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public/blog/posts/{postId}/publish\n  method: post\n  operationId: publishBlogPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public/blog/published\n  method: get\n  operationId: listPublishedBlogPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public/blog/published/{slug}\n  method: get\n  operationId: getPublishedBlogPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public/contact-requests\n  method: post\n  operationId: createContactRequest\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/platform/contact-requests\n  method: get\n  operationId: listPlatformContactRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/platform/contact-requests/{requestId}/handled\n  method: post\n  operationId: setPlatformContactRequestHandled\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /health\n  method:\
  \ get\n  operationId: routeContractGETHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health/live\n  method: get\n  operationId: routeContractGETHealthLive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health/ready\n  method: get\n  operationId: routeContractGETHealthReady\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ready\n  method: get\n  operationId: routeContractGETReady\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/auth/google/start\n  method: get\n  operationId: startGoogleSignIn\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/auth/google/callback\n  method: get\n  operationId: completeGoogleSignInBrowser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/auth/google/callback\n  method: post\n  operationId: completeGoogleSignInJson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/browser-session/start\n  method: post\n  operationId: startDashboardBrowserSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/browser-session/exchange\n  method: post\n  operationId: exchangeDashboardBrowserSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/login\n  method: post\n  operationId: loginDashboardSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/brands/first\n  method: post\n  operationId: initializeFirstWorkspaceBrand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/brands\n  method: post\n  operationId: createWorkspaceBrand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/composer-drafts/current\n  method: get\n  operationId: getCurrentComposerDraft\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/composer-drafts/current\n  method: put\n  operationId: saveCurrentComposerDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/composer-drafts/current\n  method: delete\n  operationId: deleteCurrentComposerDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/me\n  method: get\n  operationId: getDashboardBrowserSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\n\n# --- truncated at 32 KB (76 KB total) ---\n# Full source: https://artifacts.apis.io/creavily/agentic-access/creavily-agentic-access.yml\n"
source_yaml_url: https://artifacts.apis.io/creavily/agentic-access/creavily-agentic-access.yml
summary_line: 241 operations · 155 acting · 16 human-in-the-loop
tags:
- Social Media
- E-Commerce
- Publishing
- Automation
---
