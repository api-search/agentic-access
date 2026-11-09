---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 12
api_specs:
- filename: autoshort-org-account-api-openapi.yml
  format: yaml
  label: AutoShort Account API
  slug: autoshort-org-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autoshort-org/openapi/autoshort-org-account-api-openapi.yml
- filename: autoshort-org-catalog-api-openapi.yml
  format: yaml
  label: AutoShort Catalog API
  slug: autoshort-org-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autoshort-org/openapi/autoshort-org-catalog-api-openapi.yml
- filename: autoshort-org-drafts-api-openapi.yml
  format: yaml
  label: AutoShort Drafts API
  slug: autoshort-org-drafts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autoshort-org/openapi/autoshort-org-drafts-api-openapi.yml
- filename: autoshort-org-motion-api-openapi.yml
  format: yaml
  label: AutoShort Motion API
  slug: autoshort-org-motion-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autoshort-org/openapi/autoshort-org-motion-api-openapi.yml
- filename: autoshort-org-pay-per-call-x402-api-openapi.yml
  format: yaml
  label: AutoShort Pay per call (x402) API
  slug: autoshort-org-pay-per-call-x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autoshort-org/openapi/autoshort-org-pay-per-call-x402-api-openapi.yml
- filename: autoshort-org-series-api-openapi.yml
  format: yaml
  label: AutoShort Series API
  slug: autoshort-org-series-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autoshort-org/openapi/autoshort-org-series-api-openapi.yml
- filename: autoshort-org-videos-api-openapi.yml
  format: yaml
  label: AutoShort Videos API
  slug: autoshort-org-videos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autoshort-org/openapi/autoshort-org-videos-api-openapi.yml
- filename: autoshort-org-webhooks-api-openapi.yml
  format: yaml
  label: AutoShort Webhooks API
  slug: autoshort-org-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autoshort-org/openapi/autoshort-org-webhooks-api-openapi.yml
consequence_counts:
  physical: 4
  read: 12
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Autoshort Org Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/v1/drafts/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/drafts/{id}/render
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/motion-clips
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/x402/videos
operation_count: 22
overview: 'AutoShort exposes 22 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read, 6 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AutoShort
provider_slug: autoshort-org
slug: autoshort-org-agentic-access
source_filename: autoshort-org-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/autoshort-org-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    acting: 10\n    connected: 12\n  by_consequence:\n    write: 6\n    read: 12\n    physical: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/videos/generate\n  method: post\n  operationId: createVideo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/videos\n  method: get\n  operationId: listVideos\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/videos/{id}\n  method: get\n  operationId: getVideo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/videos/{id}\n  method: delete\n  operationId: deleteVideo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/videos/{id}/revise\n  method: post\n  operationId: reviseScene\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /api/v1/drafts\n  method: post\n  operationId: createDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/drafts/{id}\n  method: get\n  operationId: getDraft\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/drafts/{id}\n  method: patch\n  operationId: updateDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/v1/drafts/{id}/render\n  method: post\n  operationId: renderDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/motion-clips\n  method: post\n  operationId: createMotionClip\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/motion-clips/quote\n  method: get\n  operationId: quoteVideo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/series/performance\n  method: get\n  operationId: getSeriesPerformance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/scripts/niches\n  method: get\n  operationId: listOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/credits/balance\n  method: get\n  operationId: getCreditBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/usage/stats\n  method: get\n  operationId: getUsageStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/billing/subscription\n  method: get\n\
  \  operationId: getSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/webhooks/{id}\n  method: get\n  operationId: getWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/webhooks/{id}\n  method:\
  \ delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/x402/videos\n  method: post\n  operationId: buyVideoX402\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/x402/videos/{id}\n  method: get\n  operationId: getX402Job\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/autoshort-org/agentic-access/autoshort-org-agentic-access.yml
summary_line: 22 operations · 10 acting
tags:
- Artificial Intelligence
- Video Generation
- YouTube Shorts
- Automation
- Faceless Content
---
