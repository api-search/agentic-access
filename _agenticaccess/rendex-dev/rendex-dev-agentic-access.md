---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 10
api_specs:
- filename: rendex-dev-account-api-openapi.yml
  format: yaml
  label: rendex-dev Account API
  slug: rendex-dev-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendex-dev/openapi/rendex-dev-account-api-openapi.yml
- filename: rendex-dev-batch-api-openapi.yml
  format: yaml
  label: rendex-dev Batch API
  slug: rendex-dev-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendex-dev/openapi/rendex-dev-batch-api-openapi.yml
- filename: rendex-dev-health-api-openapi.yml
  format: yaml
  label: rendex-dev Health API
  slug: rendex-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendex-dev/openapi/rendex-dev-health-api-openapi.yml
- filename: rendex-dev-jobs-api-openapi.yml
  format: yaml
  label: rendex-dev Jobs API
  slug: rendex-dev-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendex-dev/openapi/rendex-dev-jobs-api-openapi.yml
- filename: rendex-dev-screenshot-api-openapi.yml
  format: yaml
  label: rendex-dev Screenshot API
  slug: rendex-dev-screenshot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendex-dev/openapi/rendex-dev-screenshot-api-openapi.yml
- filename: rendex-dev-watch-api-openapi.yml
  format: yaml
  label: rendex-dev Watch API
  slug: rendex-dev-watch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendex-dev/openapi/rendex-dev-watch-api-openapi.yml
consequence_counts:
  read: 10
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Rendex Dev Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 21
overview: 'rendex-dev exposes 21 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 11 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: rendex-dev
provider_slug: rendex-dev
slug: rendex-dev-agentic-access
source_filename: rendex-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/rendex-dev-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    connected: 10\n    acting: 11\n  by_consequence:\n    read: 10\n    write: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/screenshot\n  method: get\n  operationId: getScreenshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/screenshot\n  method: post\n  operationId: postScreenshot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/screenshot/json\n  method: post\n  operationId: postScreenshotJson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/screenshot/batch\n  method: post\n  operationId: postScreenshotBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/jobs/{jobId}\n  method: get\n  operationId: getJobStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/batches/{batchId}\n  method: get\n  operationId: getBatchStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: healthCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health/deep\n  method: get\n  operationId: deepHealthCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/render/link\n  method: post\n  operationId: createRenderLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/render\n  method: get\n  operationId: serveRenderLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/extract\n  method: post\n  operationId: extractContent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/artifact\n  method: post\n  operationId: renderArtifact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/watches\n  method: post\n  operationId: createWatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/watches\n  method: get\n  operationId: listWatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/watches/{id}\n  method: get\n  operationId: getWatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/watches/{id}\n  method: patch\n  operationId: updateWatch\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/watches/{id}\n  method: delete\n  operationId: deleteWatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/watches/{id}/runs\n  method: get\n  operationId: listWatchRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/watches/{id}/run\n  method: post\n  operationId: runWatchNow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/watches/test\n  method: post\n  operationId: testWatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/rendex-dev/agentic-access/rendex-dev-agentic-access.yml
summary_line: 21 operations · 11 acting
tags:
- Rendering
- Screenshots
- PDF
- Automation
---
