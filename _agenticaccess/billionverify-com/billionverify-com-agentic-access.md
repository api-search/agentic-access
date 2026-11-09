---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 6
api_specs:
- filename: billionverify-com-account-api-openapi.yml
  format: yaml
  label: BillionVerify Account API
  slug: billionverify-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/billionverify-com/openapi/billionverify-com-account-api-openapi.yml
- filename: billionverify-com-file-processing-api-openapi.yml
  format: yaml
  label: BillionVerify File Processing API
  slug: billionverify-com-file-processing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/billionverify-com/openapi/billionverify-com-file-processing-api-openapi.yml
- filename: billionverify-com-health-api-openapi.yml
  format: yaml
  label: BillionVerify Health API
  slug: billionverify-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/billionverify-com/openapi/billionverify-com-health-api-openapi.yml
- filename: billionverify-com-verification-api-openapi.yml
  format: yaml
  label: BillionVerify Verification API
  slug: billionverify-com-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/billionverify-com/openapi/billionverify-com-verification-api-openapi.yml
- filename: billionverify-com-webhooks-api-openapi.yml
  format: yaml
  label: BillionVerify Webhooks API
  slug: billionverify-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/billionverify-com/openapi/billionverify-com-webhooks-api-openapi.yml
consequence_counts:
  read: 6
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Billionverify Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'BillionVerify exposes 13 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BillionVerify
provider_slug: billionverify-com
slug: billionverify-com-agentic-access
source_filename: billionverify-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/billionverify-com-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    acting: 7\n    connected: 6\n  by_consequence:\n    write: 7\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/verify/single\n  method: post\n  operationId: verifySingleEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/verify/bulk\n  method: post\n  operationId: verifyBatchEmails\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/verify/disposable\n  method: post\n  operationId: checkDisposable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/verify/disposable\n  method: get\n  operationId: checkDisposableViaQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/verify/file\n  method: post\n  operationId: uploadFileForVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/verify/file/{job_id}\n  method: get\n  operationId: getFileJobStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/verify/file/{job_id}/results\n  method: get\n  operationId: downloadFileResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{job_id}/resume\n  method: post\n  operationId: resumePausedJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v1/credits\n  method: get\n  operationId: getCreditBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks/{webhook_id}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /health\n  method: get\n  operationId: healthCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/billionverify-com/agentic-access/billionverify-com-agentic-access.yml
summary_line: 13 operations · 7 acting
tags:
- Email Verification
- Software-as-a-Service
- Data Quality
- B2B
---
