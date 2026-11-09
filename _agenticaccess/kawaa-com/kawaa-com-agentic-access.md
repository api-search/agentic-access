---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 24
api_specs:
- filename: kawaa-com-account-api-openapi.yml
  format: yaml
  label: kawaa-com Account API
  slug: kawaa-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kawaa-com/openapi/kawaa-com-account-api-openapi.yml
- filename: kawaa-com-activity-api-openapi.yml
  format: yaml
  label: kawaa-com Activity API
  slug: kawaa-com-activity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kawaa-com/openapi/kawaa-com-activity-api-openapi.yml
- filename: kawaa-com-api-keys-api-openapi.yml
  format: yaml
  label: kawaa-com API keys API
  slug: kawaa-com-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kawaa-com/openapi/kawaa-com-api-keys-api-openapi.yml
- filename: kawaa-com-catalogue-api-openapi.yml
  format: yaml
  label: kawaa-com Catalogue API
  slug: kawaa-com-catalogue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kawaa-com/openapi/kawaa-com-catalogue-api-openapi.yml
- filename: kawaa-com-deliverability-api-openapi.yml
  format: yaml
  label: kawaa-com Deliverability API
  slug: kawaa-com-deliverability-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kawaa-com/openapi/kawaa-com-deliverability-api-openapi.yml
- filename: kawaa-com-exports-api-openapi.yml
  format: yaml
  label: kawaa-com Exports API
  slug: kawaa-com-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kawaa-com/openapi/kawaa-com-exports-api-openapi.yml
- filename: kawaa-com-health-api-openapi.yml
  format: yaml
  label: kawaa-com Health API
  slug: kawaa-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kawaa-com/openapi/kawaa-com-health-api-openapi.yml
- filename: kawaa-com-jobs-api-openapi.yml
  format: yaml
  label: kawaa-com Jobs API
  slug: kawaa-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kawaa-com/openapi/kawaa-com-jobs-api-openapi.yml
- filename: kawaa-com-search-api-openapi.yml
  format: yaml
  label: kawaa-com Search API
  slug: kawaa-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kawaa-com/openapi/kawaa-com-search-api-openapi.yml
- filename: kawaa-com-verification-api-openapi.yml
  format: yaml
  label: kawaa-com Verification API
  slug: kawaa-com-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kawaa-com/openapi/kawaa-com-verification-api-openapi.yml
- filename: kawaa-com-webhooks-api-openapi.yml
  format: yaml
  label: kawaa-com Webhooks API
  slug: kawaa-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kawaa-com/openapi/kawaa-com-webhooks-api-openapi.yml
consequence_counts:
  physical: 2
  read: 24
  safety-critical: 1
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Kawaa Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/api-keys/{keyId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/webhooks/{id}/logs/{logId}/retry
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/webhooks/{id}/test
operation_count: 38
overview: 'kawaa-com exposes 38 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 24 read, 11 write, 2 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: kawaa-com
provider_slug: kawaa-com
slug: kawaa-com-agentic-access
source_filename: kawaa-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/kawaa-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 38\n  by_action_class:\n    connected: 24\n    acting: 14\n  by_consequence:\n    read: 24\n    write: 11\n    safety-critical: 1\n    physical: 2\n  human_in_the_loop_required: 1\noperations:\n- path: /health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/verify\n  method: post\n  operationId: verifyEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - verification:write\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/verify/batch\n  method: post\n  operationId: verifyEmailBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - verification:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/verify/file\n  method: post\n  operationId: verifyFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - verification:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/jobs\n  method: get\n  operationId: listJobs\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - verification:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{id}\n  method: get\n  operationId: getJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - verification:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{id}/download\n  method: get\n  operationId: downloadJobResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - verification:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{id}/cancel\n  method: post\n  operationId: cancelJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - verification:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/find\n  method: post\n  operationId: findEmail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - verification:write\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/find/bulk\n  method: post\n  operationId: findEmailBulk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - verification:write\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domain/{domain}\n  method: get\n  operationId: searchDomain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - verification:write\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/activity/{email}\n  method: get\n  operationId: getEmailActivity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n\
  \    - verification:write\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/activity/batch\n  method: post\n  operationId: getEmailActivityBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - verification:write\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/deliverability/check\n  method: post\n  operationId: checkDeliverability\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - deliverability:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/deliverability/checks\n  method: get\n  operationId: listDeliverabilityChecks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - deliverability:read\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/deliverability/checks/{id}\n  method: get\n  operationId: getDeliverabilityCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - deliverability:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - account:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - analytics:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/usage/summary\n  method: get\n  operationId: getUsageSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - analytics:read\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/usage/credits/transactions\n  method: get\n  operationId: listCreditTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - analytics:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api-keys\n  method: get\n  operationId: listApiKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - security:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api-keys\n  method: post\n  operationId: createApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api-keys/{keyId}\n  method: delete\n  operationId: revokeApiKey\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - webhooks:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - webhooks:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/events\n  method: get\n  operationId: listWebhookEvents\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - webhooks:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks/{id}\n  method: get\n  operationId: getWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - webhooks:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks/{id}\n  method: put\n  operationId: updateWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - webhooks:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/{id}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - webhooks:write\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/{id}/secret\n  method: post\n  operationId: regenerateWebhookSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - webhooks:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/{id}/logs\n  method: get\n  operationId: listWebhookDeliveryLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - webhooks:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks/{id}/logs/{logId}/retry\n  method: post\n  operationId: retryWebhookDelivery\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    scope:\n    - webhooks:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/{id}/test\n  method: post\n  operationId: testWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - webhooks:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/plans\n  method: get\n  operationId: listPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - billing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/billing/credit-packages\n  method: get\n  operationId: listCreditPackages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - billing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/exports/schedules\n  method: get\n  operationId: listExportSchedules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - exports:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/exports/schedules/{scheduleId}/run\n  method: post\n  operationId: runExportSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - exports:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account/export/download\n  method: get\n  operationId: downloadProfileExport\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - account:read\n    - security:read\n    - verification:read\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/kawaa-com/agentic-access/kawaa-com-agentic-access.yml
summary_line: 38 operations · 14 acting · 1 human-in-the-loop
tags:
- Company
- Email Verification
- Software-as-a-Service
- Marketing
---
