---
acting_count: 83
action_class_counts:
  acting: 83
  connected: 40
api_specs:
- filename: dropto-run-abuse-api-openapi.yml
  format: yaml
  label: Dropto Abuse API
  slug: dropto-run-abuse-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dropto-run/openapi/dropto-run-abuse-api-openapi.yml
- filename: dropto-run-account-api-openapi.yml
  format: yaml
  label: Dropto Account API
  slug: dropto-run-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dropto-run/openapi/dropto-run-account-api-openapi.yml
- filename: dropto-run-announcements-api-openapi.yml
  format: yaml
  label: Dropto Announcements API
  slug: dropto-run-announcements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dropto-run/openapi/dropto-run-announcements-api-openapi.yml
- filename: dropto-run-auth-api-openapi.yml
  format: yaml
  label: Dropto Auth API
  slug: dropto-run-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dropto-run/openapi/dropto-run-auth-api-openapi.yml
- filename: dropto-run-billing-api-openapi.yml
  format: yaml
  label: Dropto Billing API
  slug: dropto-run-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dropto-run/openapi/dropto-run-billing-api-openapi.yml
- filename: dropto-run-deploys-api-openapi.yml
  format: yaml
  label: Dropto Deploys API
  slug: dropto-run-deploys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dropto-run/openapi/dropto-run-deploys-api-openapi.yml
- filename: dropto-run-health-api-openapi.yml
  format: yaml
  label: Dropto Health API
  slug: dropto-run-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dropto-run/openapi/dropto-run-health-api-openapi.yml
- filename: dropto-run-plans-api-openapi.yml
  format: yaml
  label: Dropto Plans API
  slug: dropto-run-plans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dropto-run/openapi/dropto-run-plans-api-openapi.yml
- filename: dropto-run-promotions-api-openapi.yml
  format: yaml
  label: Dropto Promotions API
  slug: dropto-run-promotions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dropto-run/openapi/dropto-run-promotions-api-openapi.yml
- filename: dropto-run-site-folders-api-openapi.yml
  format: yaml
  label: Dropto Site folders API
  slug: dropto-run-site-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dropto-run/openapi/dropto-run-site-folders-api-openapi.yml
- filename: dropto-run-sites-api-openapi.yml
  format: yaml
  label: Dropto Sites API
  slug: dropto-run-sites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dropto-run/openapi/dropto-run-sites-api-openapi.yml
- filename: dropto-run-support-api-openapi.yml
  format: yaml
  label: Dropto Support API
  slug: dropto-run-support-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dropto-run/openapi/dropto-run-support-api-openapi.yml
- filename: dropto-run-tokens-api-openapi.yml
  format: yaml
  label: Dropto Tokens API
  slug: dropto-run-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dropto-run/openapi/dropto-run-tokens-api-openapi.yml
consequence_counts:
  physical: 10
  read: 40
  safety-critical: 10
  write: 63
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 10
kind: agentic-access
layout: agentic-access
method: generated
name: Dropto Run Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/account/invites/{inviteId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/account/security
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/auth/password/forgot
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/auth/password/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/billing/resume
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/me/2fa
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/me/sessions/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/sites/{siteId}/domains/{domainId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/sites/{siteId}/upstreams/{upstreamId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/tokens/{tokenId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/auth/deletion/resend
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/auth/verify/resend
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/billing/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/billing/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/me/product-email
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/sites/{siteId}/deploys/prepare
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/sites/{siteId}/deploys/{deployId}/complete
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/sites/{siteId}/deploys/{deployId}/preview-ticket
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/sites/{siteId}/deploys/{deployId}/promote
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/sites/{siteId}/viewers/resend
operation_count: 123
overview: 'Dropto exposes 123 API operations that an AI agent could call, of which 83 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 40 read, 63 write, 10 physical, and 10 safety-critical.


  10 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Dropto
provider_slug: dropto-run
slug: dropto-run-agentic-access
source_filename: dropto-run-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: generated\nsource: openapi/dropto-run-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 123\n  by_action_class:\n    acting: 83\n    connected: 40\n  by_consequence:\n    write: 63\n    safety-critical: 10\n    read: 40\n    physical: 10\n  human_in_the_loop_required: 10\noperations:\n- path: /api/abuse\n  method: post\n  operationId: ReportAbuse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/account\n  method: patch\n  operationId: RenameAccount\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/account/invites\n  method: post\n  operationId: InviteAccountMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/account/invites/{inviteId}\n  method: delete\n  operationId: RevokeAccountInvite\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n\
  \    audit: required\n- path: /api/account/members\n  method: get\n  operationId: ListAccountMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/account/members/{userId}\n  method: delete\n  operationId: RemoveAccountMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/account/members/{userId}\n  method: patch\n  operationId: ChangeAccountMemberRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/account/security\n\
  \  method: patch\n  operationId: SetAccountSecurity\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/accounts\n  method: get\n  operationId: ListAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/announcement\n  method: get\n  operationId: GetAnnouncement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/auth/2fa\n  method: get\n  operationId: ReadTwoFactorChallenge\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/auth/2fa/recovery\n  method: post\n  operationId: RecoverTwoFactor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/2fa/verify\n  method: post\n  operationId: VerifyTwoFactor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/cli/authorize\n  method: post\n  operationId: AuthorizeCli\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/cli/device\n  method: post\n  operationId: StartCliDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/cli/device/approve\n  method: post\n  operationId: ApproveCliDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/cli/device/find\n  method: post\n  operationId: FindCliDevice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /api/auth/cli/device/token\n  method: post\n  operationId: PollCliDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/cli/token\n  method: post\n  operationId: ExchangeCliCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/config\n  method: get\n  operationId: AuthConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/auth/deletion/cancel\n\
  \  method: post\n  operationId: CancelDeletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/deletion/resend\n  method: post\n  operationId: ResendDeletionLink\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/google\n  method: get\n  operationId: GoogleSignIn\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/auth/google/one-tap\n  method:\
  \ post\n  operationId: GoogleOneTapSignIn\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/link\n  method: post\n  operationId: InspectAccountLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/login\n  method: post\n  operationId: PasswordSignIn\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/auth/logout\n  method: post\n  operationId: Logout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/password/forgot\n  method: post\n  operationId: ForgotPassword\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/auth/password/reset\n  method: post\n  operationId: ResetPassword\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n   \
  \   exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/auth/signup\n  method: post\n  operationId: SignUp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/verify\n  method: post\n  operationId: VerifyEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/verify/resend\n  method: post\n  operationId: ResendVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/billing/cancel\n  method: post\n  operationId: CancelSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/billing/checkout\n  method: post\n  operationId: StartCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/billing/invoices\n  method: get\n  operationId: GetInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/billing/plan\n  method: post\n  operationId: ChangePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/billing/plan-history\n  method: get\n  operationId: GetPlanHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/billing/portal\n  method: get\n  operationId: GetBillingPortal\n  x-agentic-access:\n    action-class: connected\n \
  \   consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/billing/resume\n  method: post\n  operationId: ResumeSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/billing/seats\n  method: post\n  operationId: ChangeSeats\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/billing/subscription\n  method: get\n  operationId: GetSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/health\n  method: get\n  operationId: Health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/health/client\n  method: get\n  operationId: ClientAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/invites/accept\n  method: post\n  operationId: AcceptAccountInvite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/me\n  method: delete\n  operationId: DeleteMe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n \
  \   audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/me\n  method: get\n  operationId: Me\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/me\n  method: patch\n  operationId: UpdateName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/me/2fa\n  method: delete\n  operationId: DisableTwoFactor\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n \
  \     proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/me/2fa/enable\n  method: post\n  operationId: EnableTwoFactor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/me/2fa/recovery-codes\n  method: post\n  operationId: RegenerateRecoveryCodes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/me/2fa/start\n  method: post\n  operationId: StartTwoFactor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n   \
  \ audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/me/devices\n  method: delete\n  operationId: ForgetAllTrustedDevices\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/me/devices\n  method: get\n  operationId: ListTrustedDevices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/me/devices/{id}\n  method: delete\n  operationId: ForgetTrustedDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/me/email\n  method: post\n  operationId: StartEmailChange\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/me/email/pending\n  method: delete\n  operationId: CancelEmailChange\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/me/export\n  method: get\n  operationId: ExportMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /api/me/google\n  method: delete\n  operationId: DisconnectGoogle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/me/onboarding\n  method: put\n  operationId: SaveOnboarding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/me/password\n  method: post\n  operationId: ChangePassword\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/me/product-email\n  method: put\n  operationId: SetProductEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/me/profile\n  method: get\n  operationId: Profile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/me/sessions/revoke\n  method: post\n  operationId: RevokeSessions\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n\
  \      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/plans\n  method: get\n  operationId: GetPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/plans/mine\n  method: get\n  operationId: GetMyPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/promotions\n  method: get\n  operationId: GetOfferedPromotions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/promotions/preview\n  method: post\n  operationId: PreviewPromotion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n     \
  \ human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/promotions/redeem\n  method: post\n  operationId: RedeemPromotion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/site-folders\n  method: get\n  operationId: ListSiteFolders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/site-folders\n  method: post\n  operationId: CreateSiteFolder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/site-folders/move\n  method: post\n  operationId: MoveSiteFolderItems\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/site-folders/{folderId}\n  method: delete\n  operationId: DeleteSiteFolder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/site-folders/{folderId}\n  method: patch\n  operationId: UpdateSiteFolder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/sites\n  method: get\n  operationId: ListSites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/sites\n  method: post\n  operationId: CreateSite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/sites/claim\n  method: post\n  operationId: ClaimSites\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/sites/subdomain-availability\n  method: get\n  operationId: CheckSubdomainAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/sites/{siteId}\n  method: delete\n  operationId: DeleteSite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/sites/{siteId}\n  method: get\n  operationId: GetSite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/sites/{siteId}\n  method: patch\n  operationId: UpdateSiteSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/sites/{siteId}/deploys/prepare\n  method: post\n  operationId: PrepareDeploy\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/sites/{siteId}/deploys/{deployId}\n  method: get\n  operationId: GetDeploy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/sites/{siteId}/deploys/{deployId}/complete\n  method: post\n  operationId: CompleteDeploy\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/sites/{siteId}/deploys/{deployId}/file\n  method: get\n  operationId: GetDeployFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/sites/{siteId}/deploys/{deployId}/manifest\n  method: get\n  operationId: GetDeployManifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/sites/{siteId}/deploys/{deployId}/preview-ticket\n  method: post\n  operationId: IssuePreviewTicket\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n  \
  \  token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/sites/{siteId}/deploys/{deployId}/promote\n  method: post\n  operationId: PromoteDeploy\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/sites/{siteId}/domains\n  method: get\n  operationId: ListSiteDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/sites/{siteId}/domains\n  method: post\n  operationId: AddSiteDomain\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/sites/{siteId}/domains/{domainId}\n  method: delete\n  operationId: RemoveSiteDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/sites/{siteId}/domains/{domainId}/recheck\n  method: post\n  operationId: RecheckSiteDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    \
  \  - high-value\n    audit: required\n- path: /api/sites/{siteId}/env\n  method: get\n  operationId: ListSiteEnv\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/sites/{siteId}/env/{name}\n  method: delete\n  operationId: RemoveSiteEnvVar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/sites/{siteId}/env/{name}\n  method: put\n  operationId: SetSiteEnvVar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/sites/{siteId}/feedback\n\
  \  method: get\n  operationId: ListSiteFeedback\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/sites/{siteId}/feedback/blocked\n  method: get\n  operationId: ListSiteCommentBlocks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/sites/{siteId}/feedback/blocked\n  method: post\n  operationId: BlockSiteCommenter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/sites/{siteId}/feedback/blocked/{userId}\n  method: delete\n  operationId: UnblockSiteCommenter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/sites/{siteId}/feedback/threads\n  method: get\n  operationId: ListSiteFeedbackThreads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/sites/{siteId}/feedback/threads/{threadId}/comments\n  method: post\n  operationId: ReplyToSiteFeedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/sites/{siteId}/feedback/threads/{threadId}/reopen\n  method: post\n  operationId: ReopenSiteFeedback\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/sites/{siteId}/feedback/threads/{threadId}/resolve\n  method: post\n  operationId: ResolveSiteFeedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/sites/{siteId}/forms\n  method: get\n  operationId: ListSiteForms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/sites/{siteId}/forms/{formName}/submissions\n  method: get\n  operationId: ListFormSubmissions\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\n\n# --- truncated at 32 KB (37 KB total) ---\n# Full source: https://artifacts.apis.io/dropto-run/agentic-access/dropto-run-agentic-access.yml\n"
source_yaml_url: https://artifacts.apis.io/dropto-run/agentic-access/dropto-run-agentic-access.yml
summary_line: 123 operations · 83 acting · 10 human-in-the-loop
tags:
- Hosting
- Artificial Intelligence
- Static Sites
- Developer Tools
- Cloud
---
