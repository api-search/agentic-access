---
acting_count: 20
action_class_counts:
  acting: 20
  connected: 15
api_specs:
- filename: appskyline-com-apps-api-openapi.yml
  format: yaml
  label: AppSkyline Apps API
  slug: appskyline-com-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appskyline-com/openapi/appskyline-com-apps-api-openapi.yml
- filename: appskyline-com-batch-api-openapi.yml
  format: yaml
  label: AppSkyline Batch API
  slug: appskyline-com-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appskyline-com/openapi/appskyline-com-batch-api-openapi.yml
- filename: appskyline-com-google-play-publishing-api-openapi.yml
  format: yaml
  label: AppSkyline Google Play Publishing API
  slug: appskyline-com-google-play-publishing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appskyline-com/openapi/appskyline-com-google-play-publishing-api-openapi.yml
- filename: appskyline-com-keywords-api-openapi.yml
  format: yaml
  label: AppSkyline Keywords API
  slug: appskyline-com-keywords-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appskyline-com/openapi/appskyline-com-keywords-api-openapi.yml
- filename: appskyline-com-metadata-api-openapi.yml
  format: yaml
  label: AppSkyline Metadata API
  slug: appskyline-com-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appskyline-com/openapi/appskyline-com-metadata-api-openapi.yml
- filename: appskyline-com-review-status-api-openapi.yml
  format: yaml
  label: AppSkyline Review Status API
  slug: appskyline-com-review-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appskyline-com/openapi/appskyline-com-review-status-api-openapi.yml
- filename: appskyline-com-sandbox-api-openapi.yml
  format: yaml
  label: AppSkyline Sandbox API
  slug: appskyline-com-sandbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appskyline-com/openapi/appskyline-com-sandbox-api-openapi.yml
- filename: appskyline-com-stats-api-openapi.yml
  format: yaml
  label: AppSkyline Stats API
  slug: appskyline-com-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appskyline-com/openapi/appskyline-com-stats-api-openapi.yml
- filename: appskyline-com-webhook-subscriptions-api-openapi.yml
  format: yaml
  label: AppSkyline Webhook subscriptions API
  slug: appskyline-com-webhook-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appskyline-com/openapi/appskyline-com-webhook-subscriptions-api-openapi.yml
consequence_counts:
  read: 15
  safety-critical: 2
  write: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Appskyline Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/apps/{appId}/google-play/data-safety
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/apps/{appId}/google-play/rollout/{track}
operation_count: 35
overview: 'AppSkyline exposes 35 API operations that an AI agent could call, of which 20 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read, 18 write, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AppSkyline
provider_slug: appskyline-com
slug: appskyline-com-agentic-access
source_filename: appskyline-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/appskyline-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 35\n  by_action_class:\n    connected: 15\n    acting: 20\n  by_consequence:\n    read: 15\n    write: 18\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /api/apple-app-store-engagement\n  method: get\n  operationId: getAppleAppStoreEngagement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/apps\n  method: get\n  operationId: getApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/apps\n  method: post\n  operationId: postApps\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/apps/{appId}\n  method: get\n  operationId: getAppsByAppId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/apps/{appId}\n  method: put\n  operationId: putAppsByAppId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/batch\n  method: post\n  operationId: postBatch\n  x-agentic-access:\n  \
  \  action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/apps/{appId}/google-play/credentials/check\n  method: get\n  operationId: googlePlayPublishingCredentials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/apps/{appId}/google-play/releases\n  method: get\n  operationId: googlePlayPublishingReleases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/apps/{appId}/google-play/release/plan\n  method: post\n  operationId: googlePlayPublishingPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/apps/{appId}/google-play/edits\n  method: post\n  operationId: googlePlayPublishingCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/apps/{appId}/google-play/edits/{editId}\n  method: get\n  operationId: googlePlayPublishingGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/apps/{appId}/google-play/edits/{editId}\n  method: delete\n  operationId: googlePlayPublishingDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/apps/{appId}/google-play/edits/{editId}/validate\n  method: post\n  operationId: googlePlayPublishingValidate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/apps/{appId}/google-play/edits/{editId}/bundles\n  method: get\n  operationId: googlePlayPublishingBundles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/apps/{appId}/google-play/edits/{editId}/bundle-upload\n  method: post\n  operationId: googlePlayPublishingUpload\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/apps/{appId}/google-play/edits/{editId}/listings\n  method: get\n  operationId: googlePlayPublishingMetadataRead\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/apps/{appId}/google-play/edits/{editId}/listings\n  method: put\n  operationId: googlePlayPublishingMetadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/apps/{appId}/google-play/edits/{editId}/tracks/{track}\n\
  \  method: put\n  operationId: googlePlayPublishingTrack\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/apps/{appId}/google-play/edits/{editId}/commit\n  method: post\n  operationId: googlePlayPublishingCommit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/apps/{appId}/google-play/rollout/{track}\n  method: post\n  operationId: googlePlayPublishingRollout\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n\
  \      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/apps/{appId}/google-play/data-safety\n  method: post\n  operationId: googlePlayPublishingDataSafety\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/keywords\n  method: get\n  operationId: getKeywords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/keywords\n  method: post\n  operationId: postKeywords\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/keywords/{keywordId}\n  method: get\n  operationId: getKeywordsByKeywordId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/keywords/{keywordId}\n  method: put\n  operationId: putKeywordsByKeywordId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/keywords/{keywordId}\n  method: delete\n  operationId: deleteKeywordsByKeywordId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n  \
  \    human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/metadatasuggestions\n  method: get\n  operationId: getMetadataSuggestions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/reviewstatuses\n  method: get\n  operationId: getReviewStatuses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/sandbox/keywords\n  method: get\n  operationId: getSandboxKeywords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/sandbox/rankchecks\n  method: post\n  operationId: postSandboxRankchecks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/sandbox/rankchecks/{jobId}\n  method: get\n  operationId: getSandboxRankchecksByJobId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/webhooksubscriptions\n  method: get\n  operationId: getWebhooksubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/webhooksubscriptions\n  method: post\n  operationId: postWebhooksubscriptions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /api/webhooksubscriptions/{webhookSubscriptionId}\n  method: put\n  operationId: putWebhooksubscriptionsByWebhookSubscriptionId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/webhooksubscriptions/{webhookSubscriptionId}\n  method: delete\n  operationId: deleteWebhooksubscriptionsByWebhookSubscriptionId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/appskyline-com/agentic-access/appskyline-com-agentic-access.yml
summary_line: 35 operations · 20 acting · 2 human-in-the-loop
tags:
- App Store Optimization
- Analytics
- Marketing
- Software-as-a-Service
- Developer Tools
- Company
---
