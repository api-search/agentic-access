---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 15
api_specs:
- filename: classifier-dev-account-api-openapi.yml
  format: yaml
  label: classifier-dev Account API
  slug: classifier-dev-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/classifier-dev/openapi/classifier-dev-account-api-openapi.yml
- filename: classifier-dev-classifier-dev-api-openapi.yml
  format: yaml
  label: classifier-dev Classifier.dev API
  slug: classifier-dev-classifier-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/classifier-dev/openapi/classifier-dev-classifier-dev-api-openapi.yml
- filename: classifier-dev-classify-api-openapi.yml
  format: yaml
  label: classifier-dev Classify API
  slug: classifier-dev-classify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/classifier-dev/openapi/classifier-dev-classify-api-openapi.yml
- filename: classifier-dev-docs-api-openapi.yml
  format: yaml
  label: classifier-dev Docs API
  slug: classifier-dev-docs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/classifier-dev/openapi/classifier-dev-docs-api-openapi.yml
- filename: classifier-dev-feedback-api-openapi.yml
  format: yaml
  label: classifier-dev Feedback API
  slug: classifier-dev-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/classifier-dev/openapi/classifier-dev-feedback-api-openapi.yml
- filename: classifier-dev-subscribe-api-openapi.yml
  format: yaml
  label: classifier-dev Subscribe API
  slug: classifier-dev-subscribe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/classifier-dev/openapi/classifier-dev-subscribe-api-openapi.yml
consequence_counts:
  physical: 3
  read: 15
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Classifier Dev Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /subscribe/confirm
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/long-context/jobs/{id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/long-context/jobs/{id}/finish
operation_count: 30
overview: 'classifier-dev exposes 30 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read, 12 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: classifier-dev
provider_slug: classifier-dev
slug: classifier-dev-agentic-access
source_filename: classifier-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/classifier-dev-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 30\n  by_action_class:\n    connected: 15\n    acting: 15\n  by_consequence:\n    read: 15\n    write: 12\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/account/balance\n  method: get\n  operationId: getAccountBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account/usage/summary\n  method: get\n  operationId: getAccountUsageSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /v1/account/usage/timeseries\n  method: get\n  operationId: getAccountUsageTimeseries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account/usage/breakdown\n  method: get\n  operationId: getAccountUsageBreakdown\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account/activity\n  method: get\n  operationId: getAccountActivity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscribe\n  method: post\n  operationId: subscribeToUpdates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n     \
  \ triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscribe/confirm\n  method: post\n  operationId: confirmSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/docs\n  method: get\n  operationId: listDocSections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sandbox/classify\n  method: post\n  operationId: classifySandbox\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api\n  method: get\n  operationId: getAgentIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/feedback\n  method: post\n  operationId: submitFeedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/observations\n  method: post\n  operationId: submitObservation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/policy\n  method: get\n  operationId: getFeedbackPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/feedback/{id}/attachments\n  method: post\n  operationId: addFeedbackAttachments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/receipts/{id}\n  method: get\n  operationId: getReceipt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/systemone\n\
  \  method: post\n  operationId: typeSafeSystemOne\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/models\n  method: get\n  operationId: listTypeSafeModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/long-context/jobs/{id}/create\n  method: put\n  operationId: createLongContextJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/long-context/jobs/{id}/parts/{sequence}\n  method: put\n  operationId: uploadLongContextPart\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/long-context/jobs/{id}/status\n  method: get\n  operationId: getLongContextJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/long-context/jobs/{id}/finish\n  method: post\n  operationId: finishLongContextJob\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/long-context/jobs/{id}/cancel\n  method: post\n\
  \  operationId: cancelLongContextJob\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/market/compare\n  method: post\n  operationId: marketCompare\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/classify\n  method: post\n  operationId: classifyV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/classify/batch\n  method: post\n  operationId: classifyBatchV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /\n  method: get\n  operationId: getDocs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: post\n  operationId: classify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{labels}/{text}\n  method: get\n  operationId: classifyByPath\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /benchmark\n  method: get\n  operationId: getBenchmark\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/classifier-dev/agentic-access/classifier-dev-agentic-access.yml
summary_line: 30 operations · 15 acting
tags:
- Company
- Machine Learning
- Natural Language Processing
- Classification
- OpenAPI
---
