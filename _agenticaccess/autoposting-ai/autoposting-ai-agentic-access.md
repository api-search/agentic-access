---
acting_count: 125
action_class_counts:
  acting: 125
  connected: 62
api_specs:
- filename: autoposting-ai-agents-api-openapi.yml
  format: yaml
  label: Autoposting.ai Agents API
  slug: autoposting-ai-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autoposting-ai/openapi/autoposting-ai-agents-api-openapi.yml
- filename: autoposting-ai-api-keys-api-openapi.yml
  format: yaml
  label: Autoposting.ai API Keys API
  slug: autoposting-ai-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autoposting-ai/openapi/autoposting-ai-api-keys-api-openapi.yml
- filename: autoposting-ai-auth-api-openapi.yml
  format: yaml
  label: Autoposting.ai Auth API
  slug: autoposting-ai-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autoposting-ai/openapi/autoposting-ai-auth-api-openapi.yml
- filename: autoposting-ai-billing-api-openapi.yml
  format: yaml
  label: Autoposting.ai Billing API
  slug: autoposting-ai-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autoposting-ai/openapi/autoposting-ai-billing-api-openapi.yml
- filename: autoposting-ai-brands-api-openapi.yml
  format: yaml
  label: Autoposting.ai Brands API
  slug: autoposting-ai-brands-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autoposting-ai/openapi/autoposting-ai-brands-api-openapi.yml
- filename: autoposting-ai-carousels-api-openapi.yml
  format: yaml
  label: Autoposting.ai Carousels API
  slug: autoposting-ai-carousels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autoposting-ai/openapi/autoposting-ai-carousels-api-openapi.yml
- filename: autoposting-ai-clips-api-openapi.yml
  format: yaml
  label: Autoposting.ai Clips API
  slug: autoposting-ai-clips-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autoposting-ai/openapi/autoposting-ai-clips-api-openapi.yml
- filename: autoposting-ai-knowledge-base-api-openapi.yml
  format: yaml
  label: Autoposting.ai Knowledge Base API
  slug: autoposting-ai-knowledge-base-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autoposting-ai/openapi/autoposting-ai-knowledge-base-api-openapi.yml
- filename: autoposting-ai-notifications-api-openapi.yml
  format: yaml
  label: Autoposting.ai Notifications API
  slug: autoposting-ai-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autoposting-ai/openapi/autoposting-ai-notifications-api-openapi.yml
- filename: autoposting-ai-organizations-api-openapi.yml
  format: yaml
  label: Autoposting.ai Organizations API
  slug: autoposting-ai-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autoposting-ai/openapi/autoposting-ai-organizations-api-openapi.yml
- filename: autoposting-ai-platform-oauth-api-openapi.yml
  format: yaml
  label: Autoposting.ai Platform OAuth API
  slug: autoposting-ai-platform-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autoposting-ai/openapi/autoposting-ai-platform-oauth-api-openapi.yml
- filename: autoposting-ai-posts-api-openapi.yml
  format: yaml
  label: Autoposting.ai Posts API
  slug: autoposting-ai-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autoposting-ai/openapi/autoposting-ai-posts-api-openapi.yml
- filename: autoposting-ai-teams-api-openapi.yml
  format: yaml
  label: Autoposting.ai Teams API
  slug: autoposting-ai-teams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autoposting-ai/openapi/autoposting-ai-teams-api-openapi.yml
- filename: autoposting-ai-usage-api-openapi.yml
  format: yaml
  label: Autoposting.ai Usage API
  slug: autoposting-ai-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autoposting-ai/openapi/autoposting-ai-usage-api-openapi.yml
- filename: autoposting-ai-webhooks-api-openapi.yml
  format: yaml
  label: Autoposting.ai Webhooks API
  slug: autoposting-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autoposting-ai/openapi/autoposting-ai-webhooks-api-openapi.yml
consequence_counts:
  physical: 10
  read: 62
  safety-critical: 10
  write: 105
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 10
kind: agentic-access
layout: agentic-access
method: generated
name: Autoposting Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /agents/{agentId}/toggle
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api-keys/{keyId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /auth/forgot-password
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /auth/reset-password
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /auth/sessions/revoke-all
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /auth/sessions/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /teams/invite-links/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /teams/members/{id}/brand-overrides/{brandId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /teams/members/{id}/brand-overrides/{brandId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /teams/members/{id}/brand-overrides/{brandId}/accounts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /auth/resend-verification
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /billing/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /billing/credits/purchase
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /billing/verify-checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /brands/reorder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /teams/invite
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /teams/ownership/accept/{token}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /teams/ownership/transfer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /teams/ownership/transfer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /webhooks/{webhookId}/test
operation_count: 187
overview: 'Autoposting.ai exposes 187 API operations that an AI agent could call, of which 125 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 62 read, 105 write, 10 physical, and 10 safety-critical.


  10 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Autoposting.ai
provider_slug: autoposting-ai
slug: autoposting-ai-agentic-access
source_filename: autoposting-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/autoposting-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 187\n  by_action_class:\n    acting: 125\n    connected: 62\n  by_consequence:\n    write: 105\n    read: 62\n    safety-critical: 10\n    physical: 10\n  human_in_the_loop_required: 10\noperations:\n- path: /agents\n  method: post\n  operationId: createAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents\n  method: get\n  operationId: listAgents\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/{agentId}\n  method: get\n  operationId: getAgent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/{agentId}\n  method: patch\n  operationId: updateAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents/{agentId}\n  method: delete\n  operationId: deleteAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n  \
  \    - high-value\n    audit: required\n- path: /agents/{agentId}/toggle\n  method: post\n  operationId: toggleAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /agents/{agentId}/run\n  method: post\n  operationId: runAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents/{agentId}/runs\n  method: get\n  operationId: listAgentRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /agents/{agentId}/runs/{runId}\n  method: get\n  operationId: getAgentRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/{agentId}/outputs\n  method: get\n  operationId: listAgentOutputs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/{agentId}/stats\n  method: get\n  operationId: getAgentStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api-keys\n  method: post\n  operationId: createApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api-keys\n  method: get\n  operationId: listApiKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api-keys/{keyId}\n  method: patch\n  operationId: updateApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api-keys/{keyId}\n  method: delete\n  operationId: revokeApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /auth/signup\n  method:\
  \ post\n  operationId: signup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/login\n  method: post\n  operationId: loginWithPassword\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/logout\n  method: post\n  operationId: logout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /auth/verify-email\n  method: post\n  operationId: verifyEmailWithOtp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/verify-email\n  method: get\n  operationId: verifyEmailWithToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /verify-email\n  method: get\n  operationId: verifyEmailWithTokenAlias\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/resend-verification\n  method: post\n  operationId: resendVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/forgot-password\n  method: post\n  operationId: forgotPassword\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /auth/reset-password\n  method: post\n  operationId: resetPassword\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n-\
  \ path: /auth/change-password\n  method: post\n  operationId: changePassword\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/social/{provider}\n  method: get\n  operationId: initiateSocialLogin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/social/exchange\n  method: post\n  operationId: exchangeSocialCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/social/complete\n  method: post\n  operationId:\
  \ completeSocialLogin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/profile\n  method: get\n  operationId: getProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/profile\n  method: patch\n  operationId: updateProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/email-change/initiate\n  method: post\n  operationId: initiateEmailChange\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/email-change/verify-current\n  method: post\n  operationId: verifyCurrentEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/email-change/verify-new\n  method: post\n  operationId: verifyNewEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/sessions\n  method: get\n  operationId:\
  \ listSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/sessions/{id}\n  method: delete\n  operationId: revokeSession\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /auth/sessions/revoke-all\n  method: post\n  operationId: revokeAllSessions\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /billing/checkout\n  method: post\n  operationId:\
  \ createBillingCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/verify-checkout\n  method: post\n  operationId: verifyBillingCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/status\n  method: get\n  operationId: getBillingStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /billing/change-plan\n  method: post\n  operationId: changeBillingPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/change-plan\n  method: delete\n  operationId: cancelBillingPlanChange\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/portal-session\n  method: post\n  operationId: createBillingPortalSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/history\n  method: get\n  operationId: getBillingHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/credits/purchase\n  method: post\n  operationId: purchaseCredits\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/credits\n  method: get\n  operationId: getCreditBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/credit-summary\n  method: get\n  operationId: getCreditSummary\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /brands\n  method: post\n  operationId: createBrand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /brands\n  method: get\n  operationId: listBrands\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /brands/{brandSlug}\n  method: get\n  operationId: getBrand\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /brands/{brandSlug}\n  method: patch\n  operationId: updateBrand\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /brands/{brandSlug}\n  method: delete\n  operationId: deleteBrand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /brands/reorder\n  method: put\n  operationId: reorderBrands\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /carousels\n  method: post\n  operationId: createCarousel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /carousels\n  method: get\n  operationId: listCarousels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /carousels/{id}\n  method: get\n  operationId: getCarousel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /carousels/{id}\n  method: patch\n  operationId: updateCarousel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /carousels/{id}\n  method: delete\n  operationId: deleteCarousel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /carousels/generate\n  method: post\n  operationId: generateCarousel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /carousels/{id}/generate-design\n  method: post\n  operationId: generateCarouselDesign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /carousels/{id}/refine-design\n  method: post\n  operationId: refineCarouselDesign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /carousels/{carouselId}/assets\n  method: post\n  operationId: uploadCarouselAssets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /carousels/{carouselId}/create-draft\n  method:\
  \ post\n  operationId: createCarouselDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clips/upload/init\n  method: post\n  operationId: initClipUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clips/upload/presign\n  method: post\n  operationId: presignClipUpload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clips/upload/complete\n  method: post\n  operationId: completeClipUpload\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clips/upload/abort\n  method: post\n  operationId: abortClipUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clips/import-url\n  method: post\n  operationId: importClipFromUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clips\n  method: get\n  operationId:\
  \ listClips\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clips/{clipId}\n  method: get\n  operationId: getClip\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clips/{clipId}\n  method: put\n  operationId: updateClip\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clips/{clipId}\n  method: delete\n  operationId: deleteClip\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /clips/{clipId}/regenerate\n  method: post\n  operationId: regenerateClipCandidates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clips/{clipId}/specific-moments\n  method: post\n  operationId: generateSpecificMoments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clips/{clipId}/generate-caption\n  method: post\n  operationId: generateClipCaption\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clips/{clipId}/render\n  method: post\n  operationId: renderClip\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clips/{clipId}/download\n  method: get\n  operationId: downloadClip\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clips/{clipId}/retry\n  method: post\n  operationId: retryClipDownload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clips/{clipId}/publish\n  method: post\n  operationId: publishClip\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clips/{clipId}/create-draft\n  method: post\n  operationId: createClipDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clips/{clipId}/jobs/{jobId}/retry\n  method: post\n  operationId: retryClipJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clips/{clipId}/jobs\n  method: get\n  operationId: getClipJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clips/jobs\n  method: get\n  operationId: listClipJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clips/billing/check\n  method: post\n  operationId: checkClipBilling\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clips/estimate-cost\n  method: post\n\
  \  operationId: estimateClipCost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /kbs\n  method: post\n  operationId: createKnowledgeBase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /kbs\n  method: get\n  operationId: listKnowledgeBases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /kbs/{kbId}\n  method: get\n  operationId: getKnowledgeBase\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /kbs/{kbId}\n  method: patch\n  operationId: updateKnowledgeBase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /kbs/{kbId}\n  method: delete\n  operationId: deleteKnowledgeBase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /kbs/{kbId}/search\n  method: post\n  operationId: searchKnowledgeBase\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /kbs/{kbId}/graph\n  method: get\n  operationId: getKnowledgeBaseGraph\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /kbs/{kbId}/docs/upload\n  method: post\n  operationId: uploadDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /kbs/{kbId}/docs/ingest-url\n  method: post\n  operationId: ingestDocumentFromUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /kbs/{kbId}/docs\n  method: get\n\
  \  operationId: listDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /kbs/{kbId}/docs/{docId}\n  method: get\n  operationId: getDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /kbs/{kbId}/docs/{docId}\n  method: delete\n  operationId: deleteDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /kbs/{kbId}/docs/{docId}/file-access\n  method: get\n  operationId: getDocumentFileAccess\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /kbs/{kbId}/docs/{docId}/chunks\n  method: post\n  operationId: searchDocumentChunks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /kbs/{kbId}/generate-ideas\n  method: post\n  operationId: generateIdeasFromKb\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ideas/generate-topic\n  method: post\n  operationId: generateIdeasFromTopic\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ideas/enrich\n  method:\
  \ post\n  operationId: enrichIdea\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ideas/enrich/{jobId}\n  method: get\n  operationId: getEnrichmentResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ideas\n  method: get\n  operationId: listIdeas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ideas/{ideaId}\n  method: patch\n  operationId: updateIdea\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ideas/{ideaId}\n  method: delete\n  operationId: deleteIdea\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/notifications\n  method: get\n  operationId: listNotifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/notifications/unread-count\n  method: get\n  operationId: getUnreadNotificationCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\n\n# --- truncated at 32 KB (55 KB total) ---\n# Full source: https://artifacts.apis.io/autoposting-ai/agentic-access/autoposting-ai-agentic-access.yml\n"
source_yaml_url: https://artifacts.apis.io/autoposting-ai/agentic-access/autoposting-ai-agentic-access.yml
summary_line: 187 operations · 125 acting · 10 human-in-the-loop
tags:
- Artificial Intelligence
- Social Media
- Automation
- Marketing
- Developer Tools
- Company
---
