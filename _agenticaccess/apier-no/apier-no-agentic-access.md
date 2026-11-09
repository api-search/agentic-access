---
acting_count: 48
action_class_counts:
  acting: 48
  connected: 108
api_specs:
- filename: apier-no-account-api-openapi.yml
  format: yaml
  label: Apier.no Account API
  slug: apier-no-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apier-no/openapi/apier-no-account-api-openapi.yml
- filename: apier-no-actions-api-openapi.yml
  format: yaml
  label: Apier.no Actions API
  slug: apier-no-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apier-no/openapi/apier-no-actions-api-openapi.yml
- filename: apier-no-admin-api-openapi.yml
  format: yaml
  label: Apier.no Admin API
  slug: apier-no-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apier-no/openapi/apier-no-admin-api-openapi.yml
- filename: apier-no-altinn-api-openapi.yml
  format: yaml
  label: Apier.no Altinn API
  slug: apier-no-altinn-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apier-no/openapi/apier-no-altinn-api-openapi.yml
- filename: apier-no-auth-gateway-api-openapi.yml
  format: yaml
  label: Apier.no Auth Gateway API
  slug: apier-no-auth-gateway-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apier-no/openapi/apier-no-auth-gateway-api-openapi.yml
- filename: apier-no-brreg-api-openapi.yml
  format: yaml
  label: Apier.no Brreg API
  slug: apier-no-brreg-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apier-no/openapi/apier-no-brreg-api-openapi.yml
- filename: apier-no-changes-api-openapi.yml
  format: yaml
  label: Apier.no Changes API
  slug: apier-no-changes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apier-no/openapi/apier-no-changes-api-openapi.yml
- filename: apier-no-company-api-openapi.yml
  format: yaml
  label: Apier.no Company API
  slug: apier-no-company-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apier-no/openapi/apier-no-company-api-openapi.yml
- filename: apier-no-discovery-api-openapi.yml
  format: yaml
  label: Apier.no Discovery API
  slug: apier-no-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apier-no/openapi/apier-no-discovery-api-openapi.yml
- filename: apier-no-fullmakt-api-openapi.yml
  format: yaml
  label: Apier.no Fullmakt API
  slug: apier-no-fullmakt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apier-no/openapi/apier-no-fullmakt-api-openapi.yml
- filename: apier-no-infrastructure-api-openapi.yml
  format: yaml
  label: Apier.no Infrastructure API
  slug: apier-no-infrastructure-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apier-no/openapi/apier-no-infrastructure-api-openapi.yml
- filename: apier-no-knowledge-api-openapi.yml
  format: yaml
  label: Apier.no Knowledge API
  slug: apier-no-knowledge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apier-no/openapi/apier-no-knowledge-api-openapi.yml
- filename: apier-no-privacy-api-openapi.yml
  format: yaml
  label: Apier.no Privacy API
  slug: apier-no-privacy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apier-no/openapi/apier-no-privacy-api-openapi.yml
- filename: apier-no-public-api-openapi.yml
  format: yaml
  label: Apier.no Public API
  slug: apier-no-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apier-no/openapi/apier-no-public-api-openapi.yml
- filename: apier-no-sandbox-api-openapi.yml
  format: yaml
  label: Apier.no Sandbox API
  slug: apier-no-sandbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apier-no/openapi/apier-no-sandbox-api-openapi.yml
- filename: apier-no-subscriptions-api-openapi.yml
  format: yaml
  label: Apier.no Subscriptions API
  slug: apier-no-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apier-no/openapi/apier-no-subscriptions-api-openapi.yml
consequence_counts:
  physical: 9
  read: 108
  safety-critical: 6
  write: 33
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 6
kind: agentic-access
layout: agentic-access
method: generated
name: Apier No Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/account/issuance-tokens/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/account/keys/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/account/keys/{id}/subkeys/{subkeyId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/account/oauth/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/admin/keys/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/fullmakt/revoke
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/actions/execute
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/actions/pending/{id}/approve
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/actions/pending/{id}/reject
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/auth/system-user/delegate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/fullmakt/principals
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/fullmakt/request
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/payments/topups
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/sandbox/altinn/list-acting-capacity
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/sandbox/rehearsal/execute
operation_count: 156
overview: 'Apier.no exposes 156 API operations that an AI agent could call, of which 48 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 108 read, 33 write, 9 physical, and 6 safety-critical.


  6 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Apier.no
provider_slug: apier-no
slug: apier-no-agentic-access
source_filename: apier-no-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/apier-no-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 156\n  by_action_class:\n    connected: 108\n    acting: 48\n  by_consequence:\n    read: 108\n    write: 33\n    physical: 9\n    safety-critical: 6\n  human_in_the_loop_required: 6\noperations:\n- path: /api/knowledge\n  method: get\n  operationId: getKnowledgeIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/knowledge/{slug}\n  method: get\n  operationId: getKnowledgeTopic\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api/v1/sandbox/company/{org}/verify\n  method: get\n  operationId: sandboxCompanyVerify\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sandbox/company/{org}/verify\n  method: options\n  operationId: sandboxCompanyVerifyOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sandbox/public/company/{org}/verify\n  method: get\n  operationId: publicSandboxCompanyVerify\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sandbox/public/company/{org}/verify\n  method: options\n  operationId: publicSandboxCompanyVerifyOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/v1/sandbox/company/{org}/authority\n  method: get\n  operationId: sandboxCompanyAuthority\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sandbox/company/{org}/authority\n  method: options\n  operationId: sandboxCompanyAuthorityOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sandbox/public/company/{org}/authority\n  method: get\n  operationId: publicSandboxCompanyAuthority\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sandbox/public/company/{org}/authority\n  method: options\n  operationId: publicSandboxCompanyAuthorityOptions\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sandbox/company/{org}/accounts\n  method: get\n  operationId: sandboxCompanyAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sandbox/company/{org}/accounts\n  method: options\n  operationId: sandboxCompanyAccountsOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sandbox/public/company/{org}/accounts\n  method: get\n  operationId: publicSandboxCompanyAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sandbox/public/company/{org}/accounts\n  method: options\n  operationId: publicSandboxCompanyAccountsOptions\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/health\n  method: get\n  operationId: healthCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/webhooks/stripe\n  method: post\n  operationId: stripeBillingWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sandbox/sessions/{suffix}/log\n  method: get\n  operationId: sandboxRequestLog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sandbox/subscriptions/test\n  method: post\n  operationId:\
  \ sandboxWebhookTest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sandbox/rehearsal/execute\n  method: post\n  operationId: rehearseMvaWriteLoop\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/actions/execute\n  method: post\n  operationId: dryRunExecuteAction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/account\n  method: delete\n  operationId: consumerAccountErase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/account/signup\n  method: post\n  operationId: accountSignup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/account/me\n  method: get\n  operationId: consumerMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/notary/records\n  method: post\n  operationId: createNotaryRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/notary/records/{id}\n  method: get\n  operationId: getNotaryRecord\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/billing/topup-requests\n  method: post\n  operationId: createAgentTopupRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/billing/topup-requests/{id}/resolve\n  method: post\n  operationId: resolveAgentTopupRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/account/credits/balance\n  method: get\n  operationId: getAccountCreditBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/account/keys\n  method: get\n  operationId: consumerKeysList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/account/keys\n  method: post\n  operationId: consumerKeysCreate\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/account/keys/{id}\n  method: delete\n  operationId: consumerKeysRevoke\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/account/keys/{id}\n  method: patch\n  operationId: consumerKeysSetSpendCaps\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/v1/account/keys/{id}/subkeys\n  method: get\n  operationId: consumerSubKeysList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/account/keys/{id}/subkeys\n  method: post\n  operationId: consumerSubKeysMint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/account/keys/{id}/subkeys/{subkeyId}\n  method: delete\n  operationId: consumerSubKeysRevoke\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /api/v1/account/oauth/{id}\n  method: delete\n  operationId: consumerOAuthConnectionRevoke\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/account/issuance-tokens\n  method: post\n  operationId: consumerIssuanceTokenMint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/account/issuance-tokens/{id}\n  method: delete\n  operationId: consumerIssuanceTokenRevoke\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/account/issuance-tokens/redeem\n  method: post\n  operationId: accountIssuanceTokenRedeem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/account/usage\n  method: get\n  operationId: consumerUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/account/profiles\n  method: get\n  operationId: consumerProfilesList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/account/profiles\n  method: post\n  operationId: consumerProfilesCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/account/profiles/{id}\n  method: patch\n  operationId: consumerProfileUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/account/profiles/{id}\n  method: delete\n  operationId: consumerProfileDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/account/preview\n  method: post\n  operationId: consumerDryRunPreview\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/account/audit\n  method: get\n  operationId: consumerAuditHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/account/receipts\n  method: get\n  operationId: consumerReceipts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/v1/admin/keys\n  method: post\n  operationId: createApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/admin/keys\n  method: get\n  operationId: listApiKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/admin/telemetry\n  method: get\n  operationId: getTelemetryAnalysis\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/admin/keys/{id}\n  method: delete\n  operationId: revokeApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/fullmakt/principals\n  method: post\n  operationId: createFullmaktPrincipal\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/fullmakt/receipts\n  method: get\n  operationId: listFullmaktReceipts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/fullmakt/request\n  method: post\n  operationId: requestFullmaktDelegation\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/fullmakt/revoke\n  method: post\n  operationId: revokeFullmaktDelegation\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/fullmakt/{org}\n  method: get\n  operationId: getFullmaktState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/auth/system-user/delegate\n  method: post\n  operationId: createSystemUserDelegation\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/company/{org}/audit\n  method: get\n  operationId: readCompanyAuditTrail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/company/{org}/accounts\n  method: get\n  operationId: getCompanyAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/company/{org}/filing-history\n  method: get\n  operationId: getCompanyFilingHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/showcase/company/{org}/verify\n  method: get\n  operationId: getShowcaseCompanyVerification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/company/{org}/snapshot\n  method: get\n  operationId: getCompanySnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/company/{org}/verify\n  method: get\n  operationId: getCompanyVerification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/company/{org}/authority\n  method: get\n  operationId: getCompanyAuthority\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api/v1/company/{org}/context\n  method: get\n  operationId: getCompanyContext\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/company/{org}/obligations\n  method: get\n  operationId: getCompanyObligations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/company/search\n  method: get\n  operationId: searchCompanies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/company/{org}/summary\n  method: get\n  operationId: getCompanySummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/company/{org}/deadlines\n  method:\
  \ get\n  operationId: getCompanyDeadlines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/altinn/list-acting-capacity\n  method: post\n  operationId: listActingCapacity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/auth/approval-token\n  method: post\n  operationId: mintApprovalToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/auth/permissions/{org}\n  method: get\n  operationId: getPermissionState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/v1/brreg/company-profile\n  method: post\n  operationId: getCompanyProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/public/company-status\n  method: get\n  operationId: getPublicCompanyStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/public/deadlines\n  method: get\n  operationId: getPublicDeadlines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/public/obligations\n  method: get\n  operationId: getPublicObligations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/public/requirements\n\
  \  method: get\n  operationId: getPublicRequirements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tools/exchange-rate\n  method: get\n  operationId: getExchangeRate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tools/altinn-migration\n  method: get\n  operationId: getAltinnMigration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/capabilities\n  method: get\n  operationId: getCapabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms.txt\n  method: get\n  operationId: getLlmsTxt\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms-full.txt\n  method: get\n  operationId: getLlmsFullTxt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workflows.json\n  method: get\n  operationId: getWorkflowsJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents.json\n  method: get\n  operationId: getAgentsJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recipes\n  method: get\n  operationId: getRecipesPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/comparison/direct-integration\n\
  \  method: get\n  operationId: getComparisonDirectIntegration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/health/agent-readiness\n  method: get\n  operationId: getAgentReadiness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/explain\n  method: post\n  operationId: explainComplianceError\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/changes\n  method: get\n  operationId: queryChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api/v1/pricing\n  method: get\n  operationId: getPricing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/privacy/dsr\n  method: post\n  operationId: submitDsrRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/actions/pending/{id}\n  method: get\n  operationId: getPendingActionStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/actions/pending/{id}/approve\n  method: post\n  operationId: approvePendingAction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n  \
  \  subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/actions/pending/{id}/reject\n  method: post\n  operationId: rejectPendingAction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/subscriptions\n  method: post\n  operationId: createSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/v1/subscriptions\n  method: get\n  operationId: listSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/subscriptions/{id}\n  method: delete\n  operationId: deleteSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sandbox/company/{org}/context\n  method: get\n  operationId: sandboxCompanyContext\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sandbox/company/{org}/context\n  method: options\n  operationId: sandboxCompanyContextOptions\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sandbox/company/{org}/obligations\n  method: get\n  operationId: sandboxCompanyObligations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sandbox/company/{org}/obligations\n  method: options\n  operationId: sandboxCompanyObligationsOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sandbox/company/{org}/deadlines\n  method: get\n  operationId: sandboxCompanyDeadlines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sandbox/company/{org}/deadlines\n  method: options\n  operationId: sandboxCompanyDeadlinesOptions\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sandbox/company/{org}/summary\n  method: get\n  operationId: sandboxCompanySummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sandbox/company/{org}/summary\n  method: options\n  operationId: sandboxCompanySummaryOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sandbox/company/{org}/audit\n  method: get\n  operationId: sandboxCompanyAudit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sandbox/company/{org}/audit\n  method: options\n  operationId: sandboxCompanyAuditOptions\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sandbox/company/{org}/filing-history\n  method: get\n  operationId: sandboxCompanyFilingHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sandbox/company/{org}/filing-history\n  method: options\n  operationId: sandboxCompanyFilingHistoryOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sandbox/auth/approval-token\n  method: post\n  operationId: sandboxAuthApprovalToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sandbox/auth/approval-token\n  method: options\n  operationId: sandboxAuthApprovalTokenOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sandbox/actions/plan\n  method: post\n  operationId: sandboxActionsPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sandbox/actions/plan\n  method: options\n  operationId: sandboxActionsPlanOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sandbox/fixtures\n  method: get\n  operationId: sandboxFixtures\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sandbox/actions/execute\n  method: post\n  operationId: sandboxActionsExecute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sandbox/actions/execute\n  method: options\n  operationId: sandboxActionsExecuteOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sandbox/public/company/{org}/context\n  method: get\n  operationId: publicSandboxCompanyContext\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n\n\n# --- truncated at 32 KB (42 KB total) ---\n# Full source: https://artifacts.apis.io/apier-no/agentic-access/apier-no-agentic-access.yml\n"
source_yaml_url: https://artifacts.apis.io/apier-no/agentic-access/apier-no-agentic-access.yml
summary_line: 156 operations · 48 acting · 6 human-in-the-loop
tags:
- Norwegian
- Company Data
- MCP
- Verification
---
