---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 15
api_specs:
- filename: verifly-email-account-api-openapi.yml
  format: yaml
  label: verifly-email Account API
  slug: verifly-email-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/verifly-email/openapi/verifly-email-account-api-openapi.yml
- filename: verifly-email-billing-api-openapi.yml
  format: yaml
  label: verifly-email Billing API
  slug: verifly-email-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/verifly-email/openapi/verifly-email-billing-api-openapi.yml
- filename: verifly-email-clean-api-openapi.yml
  format: yaml
  label: verifly-email Clean API
  slug: verifly-email-clean-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/verifly-email/openapi/verifly-email-clean-api-openapi.yml
- filename: verifly-email-extract-api-openapi.yml
  format: yaml
  label: verifly-email Extract API
  slug: verifly-email-extract-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/verifly-email/openapi/verifly-email-extract-api-openapi.yml
- filename: verifly-email-files-api-openapi.yml
  format: yaml
  label: verifly-email Files API
  slug: verifly-email-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/verifly-email/openapi/verifly-email-files-api-openapi.yml
- filename: verifly-email-jobs-api-openapi.yml
  format: yaml
  label: verifly-email Jobs API
  slug: verifly-email-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/verifly-email/openapi/verifly-email-jobs-api-openapi.yml
- filename: verifly-email-list-cleaning-api-openapi.yml
  format: yaml
  label: verifly-email List Cleaning API
  slug: verifly-email-list-cleaning-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/verifly-email/openapi/verifly-email-list-cleaning-api-openapi.yml
- filename: verifly-email-onboarding-api-openapi.yml
  format: yaml
  label: verifly-email Onboarding API
  slug: verifly-email-onboarding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/verifly-email/openapi/verifly-email-onboarding-api-openapi.yml
- filename: verifly-email-tools-api-openapi.yml
  format: yaml
  label: verifly-email Tools API
  slug: verifly-email-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/verifly-email/openapi/verifly-email-tools-api-openapi.yml
- filename: verifly-email-verification-api-openapi.yml
  format: yaml
  label: verifly-email Verification API
  slug: verifly-email-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/verifly-email/openapi/verifly-email-verification-api-openapi.yml
- filename: verifly-email-verify-api-openapi.yml
  format: yaml
  label: verifly-email Verify API
  slug: verifly-email-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/verifly-email/openapi/verifly-email-verify-api-openapi.yml
consequence_counts:
  physical: 3
  read: 15
  safety-critical: 1
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Verifly Email Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/keys/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/checkout/crypto
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/billing
operation_count: 30
overview: 'verifly-email exposes 30 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read, 11 write, 3 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: verifly-email
provider_slug: verifly-email
slug: verifly-email-agentic-access
source_filename: verifly-email-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/verifly-email-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 30\n  by_action_class:\n    acting: 15\n    connected: 15\n  by_consequence:\n    write: 11\n    read: 15\n    safety-critical: 1\n    physical: 3\n  human_in_the_loop_required: 1\noperations:\n- path: /api/v1/autonomous/register\n  method: post\n  operationId: autonomousRegister\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/verify\n  method: get\n  operationId: verifyEmail\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/verify/batch\n  method: post\n  operationId: verifyEmailBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/verify/bulk\n  method: post\n  operationId: createBulkVerificationJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/jobs\n  method: get\n  operationId: listJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/jobs/{id}\n  method: get\n  operationId: getJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/jobs/{id}/process\n  method: post\n  operationId: processJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/jobs/{id}/results\n  method: get\n  operationId: getJobResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/jobs/{id}/download\n  method: get\n  operationId: downloadJobResults\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/files\n  method: get\n  operationId: listFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/files\n  method: post\n  operationId: processFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/files/{id}\n  method: get\n  operationId: getFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/files/{id}\n  method: delete\n  operationId: deleteFile\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/files/{id}/download\n  method: get\n  operationId: downloadFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/clean\n  method: post\n  operationId: cleanEmailList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/extract\n  method: post\n  operationId: extractEmails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/credits\n  method: get\n  operationId: getCreditBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/usage\n  method: get\n  operationId: getUsageSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/account\n  method: get\n  operationId: getAccountProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/account\n  method: patch\n  operationId: updateAccountProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/keys\n  method: get\n  operationId: listApiKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/keys\n  method: post\n  operationId: createApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/keys/{id}\n  method: get\n  operationId: getApiKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/keys/{id}\n  method: patch\n  operationId: renameApiKey\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/keys/{id}\n  method: delete\n  operationId: deleteApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/billing\n  method: get\n  operationId: getBilling\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/billing\n  method: post\n  operationId: createCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/checkout\n  method: post\n  operationId: createStripeCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/checkout/crypto\n  method: post\n  operationId: createCryptoCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/tools/domain-health\n  method: get\n  operationId: domainHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/verifly-email/agentic-access/verifly-email-agentic-access.yml
summary_line: 30 operations · 15 acting · 1 human-in-the-loop
tags:
- Email Verification
- MCP
- Developer Tools
- Verification
- Company
---
