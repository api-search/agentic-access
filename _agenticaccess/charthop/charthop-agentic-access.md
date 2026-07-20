---
acting_count: 430
action_class_counts:
  acting: 430
  connected: 308
api_specs:
- filename: charthop-openapi-original.json
  format: json
  label: ChartHop REST API
  slug: charthop-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charthop/refs/heads/main/openapi/charthop-openapi-original.json
consequence_counts:
  physical: 19
  read: 308
  safety-critical: 11
  write: 400
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 11
kind: agentic-access
layout: agentic-access
method: generated
name: Charthop Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /oauth/org/{orgIdentifier}/app/{appUserId}/oauth/user
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /oauth/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/app/org/{orgId}/install/{appUserId}/connections
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/app/org/{orgId}/install/{appUserId}/disable-sync
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/org/{orgId}/band/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/org/{orgId}/field/remove-overrides
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/org/{orgId}/job-code/match/{processId}/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/org/{orgId}/process/{createIdOverride}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/user/sendreset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/user/token
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/user/{userId}/token
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /oauth/sendLoginToken
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/app/notify
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/customer/{customerId}/billing/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/org/{orgId}/ai/chat/{chatId}/message
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/org/{orgId}/ai/chat/{chatId}/message/{messageId}/feedback
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/org/{orgId}/approval-chain/{approvalChainId}/request/{approvalRequestId}/send-reminder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/org/{orgId}/category-sort
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/org/{orgId}/category-sort
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/org/{orgId}/category-sort
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/org/{orgId}/category-sort
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/org/{orgId}/category-sort/upsert
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/org/{orgId}/comp-review/{compReviewId}/send-reminder-email
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/org/{orgId}/event/{eventId}/notify
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/org/{orgId}/form/{formId}/collect
operation_count: 738
overview: 'Charthop exposes 738 API operations that an AI agent could call, of which 430 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 308 read, 400 write, 19 physical, and 11 safety-critical.


  11 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Charthop
provider_slug: charthop
slug: charthop-agentic-access
source_filename: charthop-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/charthop-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 738\n  by_action_class:\n    connected: 308\n    acting: 430\n  by_consequence:\n    read: 308\n    write: 400\n    safety-critical: 11\n    physical: 19\n  human_in_the_loop_required: 11\noperations:\n- path: /.well-known/oauth-authorization-server\n  method: get\n  operationId: authorizationServerMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-authorization-server/mcp/{agent}\n  method: get\n  operationId: mcpAuthorizationServerMetadataNoOrg\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-authorization-server/mcp/{agent}/{orgId}\n  method: get\n  operationId: mcpAuthorizationServerMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-protected-resource/mcp/{agent}\n  method: get\n  operationId: mcpProtectedResourceMetadataNoOrg\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-protected-resource/mcp/{agent}/{orgId}\n  method: get\n  operationId: mcpProtectedResourceMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/security.txt\n  method: get\n  operationId: getSecurityTxt\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp/{agent}\n  method: post\n  operationId: handleMessageNoOrg\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/{agent}\n  method: get\n  operationId: streamNoOrg\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp/{agent}/{orgId}\n  method: post\n  operationId: handleMessageForOrg\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/{agent}/{orgId}\n  method: get\n  operationId: stream\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/app/{appName}\n  method: get\n  operationId: handleRedirect\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/credentials\n  method: post\n  operationId: issueAccessTokenFromCredentials\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/join\n  method: post\n  operationId: join\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/loginWithToken\n  method: post\n  operationId: issueAccessTokenFromLoginToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/mcp/approve\n  method: post\n  operationId: approveMcpGrant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/mcp/grant-info\n  method: get\n  operationId: getMcpGrantInfo\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/org/{orgIdentifier}/app/{appName}/{appUserId}\n  method: get\n  operationId: getOauthConnectUri\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/org/{orgIdentifier}/app/{appUserId}/oauth/connection\n  method: get\n  operationId: getAppOauthConnection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/org/{orgIdentifier}/app/{appUserId}/oauth/user\n  method: get\n  operationId: listAppOauthUserConnections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/org/{orgIdentifier}/app/{appUserId}/oauth/user\n  method: delete\n\
  \  operationId: revokeAppOauthTokens\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /oauth/revoke\n  method: post\n  operationId: revokeToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /oauth/sendLoginToken\n  method: post\n  operationId: sendLoginToken\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/sso/{idp}/access-token\n  method: get\n  operationId: getIdpAccessTokenResponse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/sso/{idp}/login\n  method: get\n  operationId: ssoAuthLogin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/token\n  method: post\n  operationId: issueAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/token\n  method: delete\n  operationId:\
  \ deleteToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/token/attenuate\n  method: post\n  operationId: attenuateToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/token/sso/{type}\n  method: post\n  operationId: issueSsoToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /oauth/token/view\n  method: post\n  operationId: issueViewToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /org/{slug}\n  method: get\n  operationId: getOrgBySlugNoAuth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /saml/org/{orgId}/xml-cert\n  method: post\n  operationId: uploadXmlCertificate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /saml/org/{orgId}/xml-cert\n  method: get\n  operationId:\
  \ getXmlCertificate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /saml/sso/{org}\n  method: post\n  operationId: sso\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /saml/{org}/login\n  method: post\n  operationId: redirectToIdp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ai-credit-limit\n  method: get\n  operationId: findLimits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ai-credit-limit\n  method: post\n  operationId: createLimit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ai-credit-limit/by-customer-month\n  method: get\n  operationId: getLimitByCustomerMonth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ai-credit-limit/export-report\n  method: post\n  operationId: exportReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n   \
  \   - high-value\n    audit: required\n- path: /v1/ai-credit-limit/{id}\n  method: get\n  operationId: getLimit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ai-credit-limit/{id}\n  method: patch\n  operationId: updateLimit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ai-credit-limit/{id}\n  method: delete\n  operationId: deleteLimit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ai-hint\n  method:\
  \ get\n  operationId: findHints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ai-hint\n  method: post\n  operationId: createHint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ai-hint/generate\n  method: get\n  operationId: generateHint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ai-hint/{id}\n  method: get\n  operationId: getHint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ai-hint/{id}\n  method: patch\n  operationId:\
  \ updateHint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ai-hint/{id}\n  method: delete\n  operationId: deleteHint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ai-prompt\n  method: get\n  operationId: findPrompts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ai-prompt\n  method: post\n  operationId: createPrompt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ai-prompt/test\n  method: post\n  operationId: testPrompt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ai-prompt/types\n  method: get\n  operationId: listPromptTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ai-prompt/{id}\n  method: get\n  operationId: getPrompt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ai-prompt/{id}\n\
  \  method: patch\n  operationId: updatePrompt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ai-prompt/{id}\n  method: delete\n  operationId: deletePrompt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/app\n  method: get\n  operationId: findGlobalApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/app\n  method: post\n  operationId: createApp\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/app-config\n  method: post\n  operationId: createAppConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/app-config/{appId}\n  method: get\n  operationId: getAppConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/app-config/{appId}/{userId}\n  method: get\n  operationId: getCombinedAppConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/app-config/{appId}/{userId}\n  method: patch\n  operationId: updateAppConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/app/install/{appId}\n  method: get\n  operationId: getActiveAppInstalls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/app/name/{appName}\n  method: get\n  operationId: getAppByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/app/notify\n  method: post\n  operationId: sendNotification\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/app/org/{orgId}\n  method: get\n  operationId: findApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/app/org/{orgId}/install\n  method: get\n  operationId: findInstalledApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/app/org/{orgId}/install\n  method: post\n  operationId: installApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /v1/app/org/{orgId}/install/name/{appName}\n  method: get\n  operationId: getInstalledAppByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/app/org/{orgId}/install/validate\n  method: post\n  operationId: validateInstallApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/app/org/{orgId}/install/{appUserId}\n  method: get\n  operationId: getInstalledApp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/app/org/{orgId}/install/{appUserId}\n  method: patch\n  operationId:\
  \ updateInstalledApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/app/org/{orgId}/install/{appUserId}\n  method: delete\n  operationId: uninstallApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/app/org/{orgId}/install/{appUserId}/api-operation/{operation}\n  method: post\n  operationId: testApiOperation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n  \
  \    triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/app/org/{orgId}/install/{appUserId}/code\n  method: post\n  operationId: getAuthorizationCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/app/org/{orgId}/install/{appUserId}/connections\n  method: get\n  operationId: listMcpConnections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/app/org/{orgId}/install/{appUserId}/connections\n  method: delete\n  operationId: revokeMcpConnections\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange:\
  \ true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/app/org/{orgId}/install/{appUserId}/disable-sync\n  method: post\n  operationId: disableSync\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/app/org/{orgId}/install/{appUserId}/installdata/{installDataName}\n  method: get\n  operationId: getAppInstallData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/app/org/{orgId}/install/{appUserId}/oauth-token/refresh\n  method: post\n  operationId: refreshOauthToken\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/app/org/{orgId}/install/{appUserId}/run\n  method: post\n  operationId: runInstalledApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/app/org/{orgId}/install/{appUserId}/token\n  method: get\n  operationId: getAccessToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/app/org/{orgId}/install/{appUserId}/token\n  method: post\n  operationId: generateAccessToken\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/app/{appId}\n  method: get\n  operationId: getApp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/app/{appId}\n  method: patch\n  operationId: updateApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/app/{appId}\n  method: delete\n  operationId: deleteApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customer\n  method: get\n  operationId: findCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customer\n  method: post\n  operationId: createCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customer/{customerId}\n  method: get\n  operationId: getCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customer/{customerId}\n  method: patch\n  operationId: updateCustomer\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customer/{customerId}/billing\n  method: get\n  operationId: getBilling\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customer/{customerId}/billing/cancel\n  method: post\n  operationId: cancelSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customer/{customerId}/billing/checkout\n  method: post\n  operationId: checkout\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customer/{customerId}/invoices\n  method: get\n  operationId: getCustomerInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customer/{customerId}/subscription\n  method: get\n  operationId: getCharthopSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customer/{customerId}/subscription\n  method: patch\n  operationId: updateSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n   \
  \ audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/email-template\n  method: post\n  operationId: createEmailTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/email-template/essential\n  method: get\n  operationId: getEssentialEmailTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/email-template/name/{name}\n  method: get\n  operationId: getEmailTemplateByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/email-template/non-essential\n  method: get\n  operationId: getNonEssentialEmailTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/email-template/{emailTemplateId}\n  method: patch\n  operationId: updateEmailTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/legaldoc\n  method: post\n  operationId: createLegalDoc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/legaldoc/{name}\n\
  \  method: get\n  operationId: getLegalDoc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/media\n  method: post\n  operationId: uploadGlobalMedia\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/media/{mediaId}\n  method: get\n  operationId: getGlobalMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/org\n  method: get\n  operationId: findOrgs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/org\n  method: post\n  operationId:\
  \ createOrg\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/app-install-code/validate\n  method: post\n  operationId: validateAppInstallAuthorizationCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/slug/{slug}\n  method: get\n  operationId: getOrgBySlug\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/org/{orgId}\n  method: get\n  operationId: getOrg\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/org/{orgId}\n  method: patch\n  operationId: updateOrg\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/{orgId}/access\n  method: get\n  operationId: getUserAccess\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/org/{orgId}/access/entity/{type}\n  method: get\n  operationId: getEntityAccess\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/org/{orgId}/access/ui\n  method: get\n  operationId: getUiAccess\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/org/{orgI\n\n# --- truncated at 32 KB (219 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/charthop/refs/heads/main/agentic-access/charthop-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/charthop/refs/heads/main/agentic-access/charthop-agentic-access.yml
summary_line: 738 operations · 430 acting · 11 human-in-the-loop
tags:
- Company
- HR
- People Analytics
- HRIS
- Workforce Planning
- Compensation
- Human Resources
- Org Chart
- MCP
---
