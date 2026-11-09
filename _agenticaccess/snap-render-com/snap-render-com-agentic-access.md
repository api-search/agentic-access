---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 12
api_specs:
- filename: snap-render-com-extract-api-openapi.yml
  format: yaml
  label: snap-render-com Extract API
  slug: snap-render-com-extract-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snap-render-com/openapi/snap-render-com-extract-api-openapi.yml
- filename: snap-render-com-health-api-openapi.yml
  format: yaml
  label: snap-render-com Health API
  slug: snap-render-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snap-render-com/openapi/snap-render-com-health-api-openapi.yml
- filename: snap-render-com-schedules-api-openapi.yml
  format: yaml
  label: snap-render-com Schedules API
  slug: snap-render-com-schedules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snap-render-com/openapi/snap-render-com-schedules-api-openapi.yml
- filename: snap-render-com-screenshot-api-openapi.yml
  format: yaml
  label: snap-render-com Screenshot API
  slug: snap-render-com-screenshot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snap-render-com/openapi/snap-render-com-screenshot-api-openapi.yml
- filename: snap-render-com-usage-api-openapi.yml
  format: yaml
  label: snap-render-com Usage API
  slug: snap-render-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snap-render-com/openapi/snap-render-com-usage-api-openapi.yml
- filename: snap-render-com-webhooks-api-openapi.yml
  format: yaml
  label: snap-render-com Webhooks API
  slug: snap-render-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snap-render-com/openapi/snap-render-com-webhooks-api-openapi.yml
consequence_counts:
  physical: 1
  read: 12
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Snap Render Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/webhooks/{webhookId}/test
operation_count: 23
overview: 'snap-render-com exposes 23 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read, 10 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: snap-render-com
provider_slug: snap-render-com
slug: snap-render-com-agentic-access
source_filename: snap-render-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/snap-render-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    acting: 11\n    connected: 12\n  by_consequence:\n    write: 10\n    read: 12\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/screenshot\n  method: post\n  operationId: takeScreenshotPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/screenshot\n  method: get\n  operationId: takeScreenshot\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/screenshot/info\n  method: get\n  operationId: getScreenshotInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/screenshot/sign\n  method: post\n  operationId: signScreenshotUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/screenshot/render\n  method: get\n  operationId: renderSignedUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/extract\n  method: get\n  operationId: extractContentGet\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/extract\n  method: post\n  operationId: extractContentPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/usage/daily\n  method: get\n  operationId: getDailyUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/screenshot/batch\n  method: post\n  operationId: createBatchJob\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/screenshot/batch/{jobId}\n  method: get\n  operationId: getBatchJobStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks/{webhookId}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/{webhookId}/test\n  method: post\n  operationId: testWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/schedules\n  method: post\n  operationId: createSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/schedules\n  method: get\n  operationId: listSchedules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/schedules/{scheduleId}\n  method: get\n  operationId: getSchedule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/schedules/{scheduleId}\n  method: patch\n  operationId: updateSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/schedules/{scheduleId}\n\
  \  method: delete\n  operationId: deleteSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/schedules/{scheduleId}/run\n  method: post\n  operationId: runScheduleNow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/schedules/{scheduleId}/captures\n  method: get\n  operationId: listScheduleCaptures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: healthCheck\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/snap-render-com/agentic-access/snap-render-com-agentic-access.yml
summary_line: 23 operations · 11 acting
tags:
- Company
- Screenshots
- Rendering
- Automation
- Cloud
---
