---
acting_count: 24
action_class_counts:
  acting: 24
  connected: 18
api_specs:
- filename: transcriptdock-com-app-api-openapi.yml
  format: yaml
  label: transcriptdock-com App API
  slug: transcriptdock-com-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcriptdock-com/openapi/transcriptdock-com-app-api-openapi.yml
- filename: transcriptdock-com-batches-api-openapi.yml
  format: yaml
  label: transcriptdock-com Batches API
  slug: transcriptdock-com-batches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcriptdock-com/openapi/transcriptdock-com-batches-api-openapi.yml
- filename: transcriptdock-com-capabilities-api-openapi.yml
  format: yaml
  label: transcriptdock-com Capabilities API
  slug: transcriptdock-com-capabilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcriptdock-com/openapi/transcriptdock-com-capabilities-api-openapi.yml
- filename: transcriptdock-com-jobs-api-openapi.yml
  format: yaml
  label: transcriptdock-com Jobs API
  slug: transcriptdock-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcriptdock-com/openapi/transcriptdock-com-jobs-api-openapi.yml
- filename: transcriptdock-com-language-discoveries-api-openapi.yml
  format: yaml
  label: transcriptdock-com Language Discoveries API
  slug: transcriptdock-com-language-discoveries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcriptdock-com/openapi/transcriptdock-com-language-discoveries-api-openapi.yml
- filename: transcriptdock-com-llms-api-openapi.yml
  format: yaml
  label: transcriptdock-com Llms API
  slug: transcriptdock-com-llms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcriptdock-com/openapi/transcriptdock-com-llms-api-openapi.yml
- filename: transcriptdock-com-llms-full-api-openapi.yml
  format: yaml
  label: transcriptdock-com Llms Full API
  slug: transcriptdock-com-llms-full-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcriptdock-com/openapi/transcriptdock-com-llms-full-api-openapi.yml
- filename: transcriptdock-com-transcripts-api-openapi.yml
  format: yaml
  label: transcriptdock-com Transcripts API
  slug: transcriptdock-com-transcripts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcriptdock-com/openapi/transcriptdock-com-transcripts-api-openapi.yml
- filename: transcriptdock-com-uploads-api-openapi.yml
  format: yaml
  label: transcriptdock-com Uploads API
  slug: transcriptdock-com-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcriptdock-com/openapi/transcriptdock-com-uploads-api-openapi.yml
- filename: transcriptdock-com-usage-api-openapi.yml
  format: yaml
  label: transcriptdock-com Usage API
  slug: transcriptdock-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcriptdock-com/openapi/transcriptdock-com-usage-api-openapi.yml
- filename: transcriptdock-com-video-discoveries-api-openapi.yml
  format: yaml
  label: transcriptdock-com Video Discoveries API
  slug: transcriptdock-com-video-discoveries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcriptdock-com/openapi/transcriptdock-com-video-discoveries-api-openapi.yml
- filename: transcriptdock-com-webhook-endpoints-api-openapi.yml
  format: yaml
  label: transcriptdock-com Webhook Endpoints API
  slug: transcriptdock-com-webhook-endpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcriptdock-com/openapi/transcriptdock-com-webhook-endpoints-api-openapi.yml
- filename: transcriptdock-com-webhooks-api-openapi.yml
  format: yaml
  label: transcriptdock-com Webhooks API
  slug: transcriptdock-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcriptdock-com/openapi/transcriptdock-com-webhooks-api-openapi.yml
consequence_counts:
  physical: 1
  read: 18
  safety-critical: 2
  write: 21
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Transcriptdock Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /app/keys/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/webhook-endpoints/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /app/billing/checkout
operation_count: 42
overview: 'transcriptdock-com exposes 42 API operations that an AI agent could call, of which 24 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read, 21 write, 1 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: transcriptdock-com
provider_slug: transcriptdock-com
slug: transcriptdock-com-agentic-access
source_filename: transcriptdock-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/transcriptdock-com-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 42\n  by_action_class:\n    connected: 18\n    acting: 24\n  by_consequence:\n    read: 18\n    write: 21\n    safety-critical: 2\n    physical: 1\n  human_in_the_loop_required: 2\noperations:\n- path: /v1/capabilities\n  method: get\n  operationId: getCapabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs\n  method: post\n  operationId: createJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/jobs\n  method: get\n  operationId: listJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/language-discoveries\n  method: post\n  operationId: createLanguageDiscovery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/language-discoveries/{id}\n  method: get\n  operationId: getLanguageDiscovery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/video-discoveries\n  method: post\n  operationId:\
  \ createVideoDiscovery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/video-discoveries/{id}\n  method: get\n  operationId: getVideoDiscovery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{id}\n  method: get\n  operationId: getJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{id}/cancel\n  method: post\n  operationId: cancelJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/jobs/{id}/retry\n  method: post\n  operationId: retryJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/batches\n  method: post\n  operationId: createBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/batches/{id}\n  method: get\n  operationId: getBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transcripts/{id}\n\
  \  method: get\n  operationId: getTranscript\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transcripts/{id}\n  method: delete\n  operationId: deleteTranscript\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transcripts/{id}/export\n  method: get\n  operationId: exportTranscript\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/uploads\n  method: post\n  operationId: createUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/uploads/{id}/complete\n  method: post\n  operationId: completeUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhook-endpoints\n  method: get\n  operationId: listWebhookEndpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhook-endpoints\n  method: post\n  operationId: createWebhookEndpoint\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhook-endpoints/{id}\n  method: delete\n  operationId: deleteWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /app/keys\n  method: get\n  operationId: listApiKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app/keys\n  method: post\n  operationId: createApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /app/keys/{id}\n  method: delete\n  operationId: revokeApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /app/billing/checkout\n  method: post\n  operationId: billingCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /app/billing/quote\n  method: get\n  operationId: billingQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app/billing/portal\n  method: post\n  operationId: billingPortal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /app/billing/cancel-feedback\n  method: post\n  operationId: cancelFeedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /app/onboarding\n  method: get\n  operationId: getOnboarding\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app/onboarding\n  method: post\n  operationId: saveOnboarding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /app/profile\n  method: get\n  operationId: getProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app/profile\n  method: patch\n  operationId: updateProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /app/account\n  method: delete\n  operationId: deleteAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /app/webhooks/deliveries\n  method: get\n  operationId: listWebhookDeliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app/webhooks/{event}/redeliver\n  method: post\n  operationId: redeliverWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /app/ops/status\n  method: get\n  operationId: opsStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/callback\n  method: get\n  operationId: authCallback\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/signout\n  method: post\n  operationId: signOut\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /callbacks/assemblyai\n  method: post\n  operationId: assemblyaiCallback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /callbacks/revenuecat\n  method: post\n  operationId: revenuecatCallback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /callbacks/stripe\n  method: post\n  operationId: stripeCallback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /health\n  method: get\n  operationId: health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/transcriptdock-com/agentic-access/transcriptdock-com-agentic-access.yml
summary_line: 42 operations · 24 acting · 2 human-in-the-loop
tags:
- Company
- Video
- Transcript
- YouTube
- TikTok
---
