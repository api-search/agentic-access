---
acting_count: 30
action_class_counts:
  acting: 30
  connected: 20
api_specs:
- filename: beatapi-account-api-openapi.yml
  format: yaml
  label: BeatAPI Account API
  slug: beatapi-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatapi/openapi/beatapi-account-api-openapi.yml
- filename: beatapi-capabilities-api-openapi.yml
  format: yaml
  label: BeatAPI Capabilities API
  slug: beatapi-capabilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatapi/openapi/beatapi-capabilities-api-openapi.yml
- filename: beatapi-decisions-api-openapi.yml
  format: yaml
  label: BeatAPI Decisions API
  slug: beatapi-decisions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatapi/openapi/beatapi-decisions-api-openapi.yml
- filename: beatapi-ecommerce-video-api-openapi.yml
  format: yaml
  label: BeatAPI Ecommerce Video API
  slug: beatapi-ecommerce-video-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatapi/openapi/beatapi-ecommerce-video-api-openapi.yml
- filename: beatapi-effects-api-openapi.yml
  format: yaml
  label: BeatAPI Effects API
  slug: beatapi-effects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatapi/openapi/beatapi-effects-api-openapi.yml
- filename: beatapi-files-api-openapi.yml
  format: yaml
  label: BeatAPI Files API
  slug: beatapi-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatapi/openapi/beatapi-files-api-openapi.yml
- filename: beatapi-generation-api-openapi.yml
  format: yaml
  label: BeatAPI Generation API
  slug: beatapi-generation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatapi/openapi/beatapi-generation-api-openapi.yml
- filename: beatapi-music-video-api-openapi.yml
  format: yaml
  label: BeatAPI Music Video API
  slug: beatapi-music-video-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatapi/openapi/beatapi-music-video-api-openapi.yml
- filename: beatapi-realtime-video-api-openapi.yml
  format: yaml
  label: BeatAPI Realtime Video API
  slug: beatapi-realtime-video-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatapi/openapi/beatapi-realtime-video-api-openapi.yml
- filename: beatapi-social-data-api-openapi.yml
  format: yaml
  label: BeatAPI Social Data API
  slug: beatapi-social-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatapi/openapi/beatapi-social-data-api-openapi.yml
- filename: beatapi-tasks-api-openapi.yml
  format: yaml
  label: BeatAPI Tasks API
  slug: beatapi-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatapi/openapi/beatapi-tasks-api-openapi.yml
- filename: beatapi-text-api-openapi.yml
  format: yaml
  label: BeatAPI Text API
  slug: beatapi-text-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatapi/openapi/beatapi-text-api-openapi.yml
- filename: beatapi-usage-api-openapi.yml
  format: yaml
  label: BeatAPI Usage API
  slug: beatapi-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatapi/openapi/beatapi-usage-api-openapi.yml
- filename: beatapi-video-analysis-api-openapi.yml
  format: yaml
  label: BeatAPI Video Analysis API
  slug: beatapi-video-analysis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatapi/openapi/beatapi-video-analysis-api-openapi.yml
- filename: beatapi-web-search-api-openapi.yml
  format: yaml
  label: BeatAPI Web Search API
  slug: beatapi-web-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatapi/openapi/beatapi-web-search-api-openapi.yml
- filename: beatapi-webhooks-api-openapi.yml
  format: yaml
  label: BeatAPI Webhooks API
  slug: beatapi-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatapi/openapi/beatapi-webhooks-api-openapi.yml
- filename: beatapi-workflows-api-openapi.yml
  format: yaml
  label: BeatAPI Workflows API
  slug: beatapi-workflows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatapi/openapi/beatapi-workflows-api-openapi.yml
consequence_counts:
  read: 20
  write: 30
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Beatapi Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 50
overview: 'BeatAPI exposes 50 API operations that an AI agent could call, of which 30 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read and 30 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BeatAPI
provider_slug: beatapi
slug: beatapi-agentic-access
source_filename: beatapi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/beatapi-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 50\n  by_action_class:\n    acting: 30\n    connected: 20\n  by_consequence:\n    write: 30\n    read: 20\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/systemone\n  method: post\n  operationId: createDecision\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/models\n  method: get\n  operationId: listTextModels\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/responses\n  method: post\n  operationId: createTextResponse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chat/completions\n  method: post\n  operationId: createChatCompletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/messages\n  method: post\n  operationId: createMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1beta/models/{model}:{action}\n  method: post\n  operationId: generateGeminiCompatibleContent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/workflows\n  method: get\n  operationId: listWorkflows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/media/models\n  method: get\n  operationId: listGenerationModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/images/tasks\n  method: post\n\
  \  operationId: createImageGenerationTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos/tasks\n  method: post\n  operationId: createVideoGenerationTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/effects\n  method: get\n  operationId: listEffects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/effects/{effect_id}\n  method: get\n  operationId: getEffect\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/effects/tasks\n  method: post\n  operationId: createEffectTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/video-analysis/tasks\n  method: post\n  operationId: createVideoAnalysisTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/music-video/tasks\n  method: post\n  operationId: createMusicVideoTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/music-video/tasks/{task_id}/shots/{shot_id}/edit\n  method: post\n  operationId: editMusicVideoShot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/music-video/tasks/{task_id}/shots/{shot_id}/media\n  method: post\n  operationId: getMusicVideoShotMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/music-video/tasks/{task_id}/compose\n  method: post\n  operationId: composeMusicVideoTask\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ecommerce-video/tasks\n  method: post\n  operationId: createEcommerceVideoTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/capabilities/search\n  method: post\n  operationId: searchCapabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/capabilities/inspect\n  method: post\n  operationId: inspectCapability\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/capabilities/run\n  method: post\n  operationId: runCapability\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/social-data/call\n  method: post\n  operationId: callSocialData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/web/search\n  method: post\n  operationId: searchWeb\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/web/read\n  method: post\n  operationId: readWebPages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/web/map\n  method: post\n  operationId: mapWebsite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/web/research\n  method: post\n  operationId: researchWeb\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tasks/{task_id}\n  method: get\n  operationId: getTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/realtime/sessions\n  method: post\n  operationId: createRealtimeSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/realtime/sessions/{session_id}\n  method: get\n  operationId: getRealtimeSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/realtime/sessions/{session_id}\n  method: delete\n  operationId:\
  \ closeRealtimeSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account/usage/records\n  method: get\n  operationId: listUsageRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account/usage/records/{id}\n  method: get\n  operationId: getUsageRecord\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account\n  method: get\n\
  \  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account/notifications\n  method: get\n  operationId: getAccountNotifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account/notifications\n  method: patch\n  operationId: updateAccountNotifications\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account/payments\n  method: get\n  operationId: listAccountPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/account/keys\n  method: get\n  operationId: listAccountApiKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account/keys\n  method: post\n  operationId: createAccountApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account/keys/{id}\n  method: get\n  operationId: getAccountApiKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account/keys/{id}\n  method: patch\n  operationId: updateAccountApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account/keys/{id}\n  method: delete\n  operationId: deleteAccountApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account/keys/{id}/reveal\n  method: post\n  operationId: revealAccountApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/files\n  method: post\n  operationId: uploadFile\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks\n  method: get\n  operationId: listWebhookEndpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks\n  method: post\n  operationId: createWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/{id}\n  method: get\n  operationId: getWebhookEndpoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /v1/webhooks/{id}\n  method: patch\n  operationId: updateWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/{id}\n  method: delete\n  operationId: deleteWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/beatapi/agentic-access/beatapi-agentic-access.yml
summary_line: 50 operations · 30 acting
tags:
- Company
- Artificial Intelligence
- Platform
- Unified API
- Data Integration
---
