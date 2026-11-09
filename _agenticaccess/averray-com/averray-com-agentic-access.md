---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 55
api_specs:
- filename: averray-com-accounts-api-openapi.yml
  format: yaml
  label: Averray Accounts API
  slug: averray-com-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/averray-com/openapi/averray-com-accounts-api-openapi.yml
- filename: averray-com-auth-api-openapi.yml
  format: yaml
  label: Averray Auth API
  slug: averray-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/averray-com/openapi/averray-com-auth-api-openapi.yml
- filename: averray-com-discovery-api-openapi.yml
  format: yaml
  label: Averray Discovery API
  slug: averray-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/averray-com/openapi/averray-com-discovery-api-openapi.yml
- filename: averray-com-health-api-openapi.yml
  format: yaml
  label: Averray Health API
  slug: averray-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/averray-com/openapi/averray-com-health-api-openapi.yml
- filename: averray-com-jobs-api-openapi.yml
  format: yaml
  label: Averray Jobs API
  slug: averray-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/averray-com/openapi/averray-com-jobs-api-openapi.yml
- filename: averray-com-pool-api-openapi.yml
  format: yaml
  label: Averray Pool API
  slug: averray-com-pool-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/averray-com/openapi/averray-com-pool-api-openapi.yml
- filename: averray-com-receipts-api-openapi.yml
  format: yaml
  label: Averray Receipts API
  slug: averray-com-receipts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/averray-com/openapi/averray-com-receipts-api-openapi.yml
- filename: averray-com-schemas-api-openapi.yml
  format: yaml
  label: Averray Schemas API
  slug: averray-com-schemas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/averray-com/openapi/averray-com-schemas-api-openapi.yml
- filename: averray-com-sessions-api-openapi.yml
  format: yaml
  label: Averray Sessions API
  slug: averray-com-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/averray-com/openapi/averray-com-sessions-api-openapi.yml
- filename: averray-com-verify-api-openapi.yml
  format: yaml
  label: Averray Verify API
  slug: averray-com-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/averray-com/openapi/averray-com-verify-api-openapi.yml
consequence_counts:
  physical: 3
  read: 55
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Averray Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /account/deposit/transactions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /account/withdraw/transactions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pool/transactions
operation_count: 68
overview: 'Averray exposes 68 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 55 read, 10 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Averray
provider_slug: averray-com
slug: averray-com-agentic-access
source_filename: averray-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/averray-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 68\n  by_action_class:\n    connected: 55\n    acting: 13\n  by_consequence:\n    read: 55\n    write: 10\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /robots.txt\n  method: get\n  operationId: getRobots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /terms\n  method: get\n  operationId: getVerifyTerms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pricing\n  method: get\n\
  \  operationId: getPricing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/nonce\n  method: post\n  operationId: requestSiweNonce\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/verify\n  method: post\n  operationId: verifySiweSignature\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs/x402\n  method: post\n  operationId: postJobWithX402\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs\n  method: get\n  operationId: listJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/definition\n  method: get\n  operationId: getJobDefinition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/recommendations\n  method: get\n  operationId: recommendJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/claim\n  method: post\n  operationId: claimJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs/preflight\n  method: get\n  operationId: preflightJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/submit\n  method: post\n  operationId: submitJobWork\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account\n  method: get\n  operationId:\
  \ getAccountSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions\n  method: get\n  operationId: listWalletSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /session\n  method: get\n  operationId: getWalletSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schemas/jobs\n  method: get\n  operationId: listJobSchemas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: getApiInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /openapi.json\n  method: get\n  operationId: getPublicOpenApi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp\n  method: get\n  operationId: getMcpInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp\n  method: post\n  operationId: callMcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent-tools.json\n  method: get\n  operationId: getAgentTools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/agent-tools.json\n\
  \  method: get\n  operationId: getWellKnownAgentTools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/ai-agent.json\n  method: get\n  operationId: getAiAgentDiscovery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/agent-card.json\n  method: get\n  operationId: getAgentCardDiscovery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms.txt\n  method: get\n  operationId: getLlmsText\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/x402\n  method: get\n  operationId: getX402Discovery\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /onboarding\n  method: get\n  operationId: getOnboarding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /poster/onboarding\n  method: get\n  operationId: getPosterOnboarding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status/providers\n  method: get\n  operationId: getPublicProviderStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transparency\n  method: get\n  operationId: getTransparency\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pool\n  method:\
  \ get\n  operationId: getDepositPool\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /verify/profiles\n  method: get\n  operationId: listVerificationProfiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /verify/runs\n  method: get\n  operationId: verifyRunCreationMethod\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /verify/runs\n  method: post\n  operationId: createVerificationRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verify/runs/{runId}\n\
  \  method: get\n  operationId: getVerificationRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{id}\n  method: get\n  operationId: getListedJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/open\n  method: get\n  operationId: redirectOpenJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/tiers\n  method: get\n  operationId: getJobTiers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/validate-submission\n  method: post\n  operationId: validateJobSubmission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs/explain-eligibility\n  method: get\n  operationId: explainJobEligibility\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/estimate-reward\n  method: get\n  operationId: estimateJobReward\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{id}/estimate\n  method: get\n  operationId: estimateJobRewardById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/draft\n  method: post\n  operationId: draftJob\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs/draft/{draftId}\n  method: get\n  operationId: getJobDraft\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/draft/{draftId}/transactions\n  method: post\n  operationId: buildPostJobTransactions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /poster/jobs\n  method: get\n  operationId: listPosterJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /session/state-machine\n  method: get\n  operationId: getSessionStateMachine\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/position\n  method: get\n  operationId: getAccountPosition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/borrow-capacity\n  method: get\n  operationId: getBorrowCapacity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me\n  method: get\n  operationId: getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reputation\n  method: get\n  operationId: getReputation\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /receipts\n  method: get\n  operationId: listOwnReceipts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /receipts/{receiptId}\n  method: get\n  operationId: getReceipt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /badges\n  method: get\n  operationId: listBadges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /badges/{sessionId}\n  method: get\n  operationId: getBadge\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /badges/{sessionId}/run\n  method:\
  \ get\n  operationId: getRunReceipt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/badge-receipt-jwks.json\n  method: get\n  operationId: getReceiptJwks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents\n  method: get\n  operationId: listPublicAgents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/{wallet}\n  method: get\n  operationId: getPublicAgent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shares/{token}\n  method: get\n  operationId: getSharedSnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gas/health\n  method: get\n  operationId: getGasHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gas/capabilities\n  method: get\n  operationId: getGasCapabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schemas/jobs/{name}.json\n  method: get\n  operationId: getJobSchema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/{path}\n  method: get\n  operationId: getAccountSubresource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pool/transactions\n  method: post\n\
  \  operationId: buildDepositPoolTransactions\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/deposit/transactions\n  method: post\n  operationId: buildAccountDepositTransactions\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/withdraw/transactions\n  method: post\n  operationId: buildWithdrawTransactions\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/averray-com/agentic-access/averray-com-agentic-access.yml
summary_line: 68 operations · 13 acting
tags:
- Payments
- Blockchain
- Verification
- Agents
- USDC
---
